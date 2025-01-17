# DNN+NeuroSim V1.0

The DNN+NeuroSim framework was developed by [Prof. Shimeng Yu's group](https://shimeng.ece.gatech.edu/) (Georgia Institute of Technology). The model is made publicly available on a non-commercial basis. Copyright of the model is maintained by the developers, and the model is distributed under the terms of the [Creative Commons Attribution-NonCommercial 4.0 International Public License](http://creativecommons.org/licenses/by-nc/4.0/legalcode)

This is the released version 1.0 (June 1st, 2019) for the tool, and this version is an integrated framework developed in C++ and wrapped by Pytorch and Tensorflow, it supports **_digital SRAM, eNVM (STT-MRAM, RRAM and PCM) and FeFET_** based architectures, for deep neural networks (DNNs) inference performance estimation.

In Pytorch/Tensorflow wrapper, users are able to define **_network structures, precision of synaptic weight and neural activation_**. With the integrated NeuroSim which takes real traces from wrapper, the framework can support hierarchical organization from device level to circuit level, to chip level and to algorithm level, enabling **_instruction-accurate evaluation on both accuracy and hardware performance of inference_**.

If you use the tool or adapt the tool in your work or publication, you are required to cite the following reference:

X. Peng, S. Huang, Y. Luo, X. Sun and S. Yu, ※DNN+NeuroSim: An End-to-End Benchmarking Framework for Compute-in-Memory Accelerators with Versatile Device Technologies, *§ IEEE International Electron Devices Meeting (IEDM)*, 2019.

If you have logistic questions or comments on the model, please contact [Prof. Shimeng Yu](mailto:shimeng.yu@ece.gatech.edu), and if you have technical questions or comments, please contact [Xiaochen Peng](mailto:xpeng76@gatech.edu) or [Shanshi Huang](mailto:shuang406@gatech.edu).


## File lists
1. Manual: `Documents/DNNNeuroSim_Manual.pdf`
2. DNN_NeuroSim wrapped by Pytorch: 'Inference_pytorch'
3. DNN_NeuroSim wrapped by Tensorflow: 'Inference_tensorflow'
4. NeuroSim under Pytorch Inference: 'Inference_pytorch/NeuroSIM'
5. NeuroSim under Tensorflow Inference: 'Inference_tensorflow/source/NeuroSIM'


## Installation steps (Linux)
1. Get the tool from GitHub
```
git clone https://github.com/neurosim/DNN_NeuroSim_V1.0.git
```

2. Train the network to get the model for inference

3. Compile the NeuroSim codes
```
make
```

4. Run Pytorch/Tensorflow wrapper (integrated with NeuroSim)


For the usage of this tool, please refer to the manual.


## References related to this tool 
1. X. Peng, S. Huang, Y. Luo, X. Sun and S. Yu, ※DNN+NeuroSim: An End-to-End Benchmarking Framework for Compute-in-Memory Accelerators with Versatile Device Technologies, *§ IEEE International Electron Devices Meeting (IEDM)*, 2019.
2. X. Peng, R. Liu, S. Yu, ※Optimizing weight mapping and data flow for convolutional neural networks on RRAM based processing-in-memory architecture, *§ IEEE International Symposium on Circuits and Systems (ISCAS)*, 2019.
3. P.-Y. Chen, S. Yu, ※Technological benchmark of analog synaptic devices for neuro-inspired architectures, *§ IEEE Design & Test*, 2019.
4. P.-Y. Chen, X. Peng, S. Yu, ※NeuroSim: A circuit-level macro model for benchmarking neuro-inspired architectures in online learning, *§ IEEE Trans. CAD*, 2018.
5. X. Sun, S. Yin, X. Peng, R. Liu, J.-S. Seo, S. Yu, ※XNOR-RRAM: A scalable and parallel resistive synaptic architecture for binary neural networks,*§ ACM/IEEE Design, Automation & Test in Europe Conference (DATE)*, 2018.
6. P.-Y. Chen, X. Peng, S. Yu, ※NeuroSim+: An integrated device-to-algorithm framework for benchmarking synaptic devices and array architectures, *§ IEEE International Electron Devices Meeting (IEDM)*, 2017.
7. P.-Y. Chen, S. Yu, ※Partition SRAM and RRAM based synaptic arrays for neuro-inspired computing,*§ IEEE International Symposium on Circuits and Systems (ISCAS)*, 2016.
8. P.-Y. Chen, D. Kadetotad, Z. Xu, A. Mohanty, B. Lin, J. Ye, S. Vrudhula, J.-S. Seo, Y. Cao, S. Yu, ※Technology-design co-optimization of resistive cross-point array for accelerating learning algorithms on chip,*§ IEEE Design, Automation & Test in Europe (DATE)*, 2015.
9. S. Wu, et al., ※Training and inference with integers in deep neural networks,*§ arXiv: 1802.04680*, 2018.
10. github.com/boluoweifenda/WAGE
11. github.com/stevenygd/WAGE.pytorch
12. github.com/aaron-xichen/pytorch-playground
