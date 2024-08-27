
# 🌀 ControlNeXt



##   [📝 Project Page](https://pbihao.github.io/projects/controlnext/index.html)  |  [📚 Paper](https://arxiv.org/abs/2408.06070) | [🗂️ Demo (SDXL)](https://huggingface.co/spaces/Eugeoter/ControlNeXt)


**ControlNeXt** is our official implementation for controllable generation, supporting both images and videos while incorporating diverse forms of control information. In this project, we propose a new method that reduces trainable parameters by up to 90% compared with ControlNet, achieving faster convergence and outstanding efficiency. This method can be directly combined with other LoRA techniques to alter style and ensure more stable generation. Please refer to the examples for more details.

We provide an online demo of [ControlNeXt-SDXL](./ControlNeXt-SDXL/). Due to the high resource requirements of SVD, we are unable to offer it online.

> This project is still undergoing iterative development. The code and model may be updated at any time. More information will be provided later.

# Experiences
We share more training experiences [there](./experiences.md) and in the [Issue](https://github.com/dvlab-research/ControlNeXt/issues/14#issuecomment-2290450333).
We spent a lot of time to find these. Now share with all of you. May these will help you!

# Model Zoo

- **ControlNeXt-SDXL** [ [Link](ControlNeXt-SDXL) ] : Controllable image generation. Our model is built upon [Stable Diffusion XL ](stabilityai/stable-diffusion-xl-base-1.0). Fewer trainable parameters, faster convergence, improved efficiency, and can be integrated with LoRA.

- **ControlNeXt-SDXL-Training** [ [Link](ControlNeXt-SDXL-Training) ] :  The training scripts for our `ControlNeXt-SDXL` [ [Link](ControlNeXt-SDXL) ].

- **ControlNeXt-SVD-v2** [ [Link](ControlNeXt-SVD-v2) ] :  Generate the video controlled by the sequence of human poses. In the v2 version, we implement several improvements: a higher-quality collected training dataset, larger training and inference batch frames, higher generation resolution, enhanced human-related video generation through continual training, and pose alignment for inference to improve overall performance.

- **ControlNeXt-SVD-v2-Training** [ [Link](ControlNeXt-SVD-v2-Training) ] :  The training scripts for our `ControlNeXt-SVD-v2` [ [Link](ControlNeXt-SVD-v2) ].

- **ControlNeXt-SVD** [ [Link](ControlNeXt-SVD) ] :  Generate the video controlled by the sequence of human poses. This can be seen as an attempt to replicate the implementation of [AnimateAnyone](https://github.com/HumanAIGC/AnimateAnyone). However, our model is built upon [Stable Video Diffusion](https://stability.ai/stable-video), employing a more concise architecture.

- **ControlNeXt-SD1.5** [ [Link](ControlNeXt-SD1.5) ] : Controllable image generation. Our model is built upon [Stable Diffusion 1.5](https://huggingface.co/runwayml/stable-diffusion-v1-5). Fewer trainable parameters, faster convergence, improved efficiency, and can be integrated with LoRA.

- **ControlNeXt-SD1.5-Training** [ [Link](ControlNeXt-SD1.5-Training) ] : The training scripts for our `ControlNeXt-SD1.5` [ [Link](ControlNeXt-SD1.5) ].

- **ControlNeXt-SD3** [ [Link](ControlNeXt-SD3) ] :  We are regret to inform that ControlNeXt-SD3 is trained with protected and private data and code, and therefore cannot be released.


### If you find this work useful, please consider citing:
```
@article{peng2024controlnext,
  title={ControlNeXt: Powerful and Efficient Control for Image and Video Generation},
  author={Peng, Bohao and Wang, Jian and Zhang, Yuechen and Li, Wenbo and Yang, Ming-Chang and Jia, Jiaya},
  journal={arXiv preprint arXiv:2408.06070},
  year={2024}
}
```
