# Synergistic Efficiency 

Parameter-efficient tuning and decreasing the computational demands are two branches of work after the Vision Transformer came out. In this project, my teammate and I try to merge these two branches together by leveraging the prompt-tuning method of Visual-Prompt Tuning (VPT) and incorporating three token reduction techniques. Besides Token Merging (ToMe) and EViT, one of my teammates introduce a new prototype-driven token reduction technique called ProtoCut, which addresses information redundancy by examining the prototypicality of tokens. The Zach branch of this repository focuses on the portion of my work, which utilize ToMe as the token reduction technique. EViT is implemented by @Longday0923 and the ProtoCut is implemented by @EuronZhang. Here is the original repository (https://github.com/EuronZhang/SynergisticEfficiency)

![teaser](https://github.com/ChuiZhao/EECS_553_Project/blob/Zach/imgs/pipeline.png)

## Acknowledgements

This repository is built on [VPT](https://github.com/kmnp/vpt), and portions of [ToMe](https://github.com/facebookresearch/ToMe) and [EViT](https://github.com/youweiliang/evit). All setting is following [VPT](https://github.com/kmnp/vpt) and [ToMe](https://github.com/facebookresearch/ToMe).

