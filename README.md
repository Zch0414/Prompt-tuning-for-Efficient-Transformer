# Synergistic Efficiency 

This is the repository of my EECS 553 project, it is forked from https://github.com/EuronZhang/SynergisticEfficiency

----

Parameter-efficient tuning and decreasing the computational demands are two branches of work after the Vision Transformer came out. In this project, my teammate and I try to merge these two branches together by leveraging the prompt-tuning method of Visual-Prompt Tuning (VPT) and incorporating three token reduction techniques. Besides Token Merging (ToMe) and EViT, one of my teammates introduce a new prototype-driven token reduction technique called ProtoCut, which addresses information redundancy by examining the prototypicality of tokens. The Zach branch of this repository focuses on the portion of my work, which utilize ToMe as the token reduction technique. EViT is implemented by [@Longday0923](https://github.com/Longday0923) and the ProtoCut is implemented by [@EuronZhang](https://github.com/EuronZhang). For more details, I refer you to the different branches of this repository or the original repository.

![teaser](https://github.com/Zch0414/EECS_553_Project/blob/Zach/imgs/pipeline.png)

----

We apply the token reduction technology not only to image tokens but also to prompt tokens. Since ToMe merges tokens by measuring the cosine similarity of their key, there is a natural insight to find out which image token a learnable prompt is similar to. This insight gives a possible interpretation of the visual prompt. We highlight the most similar tokens in relation to the learned prompt in the input image for ToMe. We observe that the most learned prompts tend to point to the background of the image, which corresponds to one of the prompt settings mentioned in the Segment Anything Model. We hope this discovery can attract more researchers to explore prompt engineering and its potential applications in various tasks and domains.

![result](https://github.com/Zch0414/EECS_553_Project/blob/Zach/imgs/qualitative_result.png)

## Acknowledgements

This repository is built on [VPT](https://github.com/kmnp/vpt), and portions of [ToMe](https://github.com/facebookresearch/ToMe) and [EViT](https://github.com/youweiliang/evit). All setting is following [VPT](https://github.com/kmnp/vpt) and [ToMe](https://github.com/facebookresearch/ToMe).

