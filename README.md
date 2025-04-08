# Awesome-LLM-Robustness-papers

A curated list of awesome LLM Robustness papers for the survey paper '**Evaluating and Improving Robustness in Large Language Models: A Survey and Future Directions**'. 

#### Why LLM Robustness?
LLM robustness requires that models should not only generate consistent contents, but also ensure the correctness and stability of generated content when dealing with *unexpeted application scenarios* (e.g., toxic prompts, limited noise domain data, out-of-distribution (OOD) applications, etc).

- LLMs have been applied to various domains and scenarios;
- LLMs should be able to deal with the complex real-world situations; 
- LLMs should generate reliable contents for decision making; 
- LLMs should gain the trust of humans. 

## Contributing 
Please help contribute this list by [pull request](https://github.com/zhangkunzk/Awesome-LLM-Robustness-papers/pulls)

Markdown format: 

```markdown
- Paper Name. 
  [[pdf]](link) 
  [[code]](link)
  - Author 1, Author 2, and Author 3. *Conference Year*
```

## Table of Contents
- [Summarization](#summarization)
- [Adversarial Robustness](#adversarial-robustness)
  - [Noise Prompt](#noise-prompt)
  - [Long Context](#long-context)
  - [Attack and Defense](#attack-defense)
  - [Noise Decoding](#noise-decoding)
  - [Causal Inspired Methods](#causal-inspired-methods)
- [OOD Robustness](#ood-robustness)
  - [Domain Transfer and Generalization](#domain-transfer-and-generalization)
  - [OOD Detection](#ood-detection)
  - [Tuning Method](#tuning-method)
  - [Hallucination](#hallucination)
  - [Causal Enhanced Solution](#causal-enhanced-solution)
- [Robustness Evaluation](#robustness-evaluation)
  - [Dataset Construction](#dataset-construction)
  - [Robustness Evaluation](#robustness-evaluation)
  - [Causal Related Evaluation](#causal-related-evaluation)

## Summarization
- Bias and fairness in large language models: A survey.
  [pdf](https://aclanthology.org/2024.cl-3.8/)
  - Isabel O Gallegos, Ryan A Rossi, Joe Barrow, Md Mehrab Tanjim, Sungchul Kim, Franck Dernoncourt, Tong Yu, Ruiyi Zhang, and Nesreen K Ahmed. *Computational Linguistics 2024*

- Revisiting out-of-distribution robustness in nlp: Benchmarks, analysis, and LLMs evaluations.
  [pdf](https://proceedings.neurips.cc/paper_files/paper/2023/file/b6b5f50a2001ad1cbccca96e693c4ab4-Paper-Datasets_and_Benchmarks.pdf)
  - Lifan Yuan, Yangyi Chen, Ganqu Cui, Hongcheng Gao, Fangyuan Zou, Xingyi Cheng, Heng Ji, Zhiyuan Liu, and Maosong Sun. *Advances in Neural Information Processing Systems 2023*

- A survey of adversarial defenses and robustness in nlp.
  [pdf](https://dl.acm.org/doi/10.1145/3593042)
  - Shreya Goyal, Sumanth Doddapaneni, Mitesh M Khapra, and Balaraman Ravindran. *ACM Computing Surveys 2023*

- How robust is gpt-3.5 to predecessors? a comprehensive study on language understanding tasks.
  [pdf](https://arxiv.org/abs/2303.00293)
  - Xuanting Chen, Junjie Ye, Can Zu, Nuo Xu, Rui Zheng, Minlong Peng, Jie Zhou, Tao Gui, Qi Zhang, and Xuanjing Huang. *arXiv preprint arXiv:2303.00293 2023*

- On the robustness of chatgpt: An adversarial and out-of-distribution perspective.
  [pdf](https://arxiv.org/abs/2302.12095)
  - Jindong Wang, Xixu Hu, Wenxin Hou, Hao Chen, Runkai Zheng, Yidong Wang, Linyi Yang, Haojun Huang, Wei Ye, Xiubo Geng, and others. *arXiv preprint arXiv:2302.12095 2023*

- A survey on efficient inference for large language models.
  [pdf](https://arxiv.org/abs/2404.14294)
  - Zixuan Zhou, Xuefei Ning, Ke Hong, Tianyu Fu, Jiaming Xu, Shiyao Li, Yuming Lou, Luning Wang, Zhihang Yuan, Xiuhong Li, and others. *arXiv preprint arXiv:2404.14294 2024*

- Trustworthy LLMs: A survey and guideline for evaluating large language models' alignment.
  [pdf](https://arxiv.org/abs/2404.14294)
  - Yang Liu, Yuanshun Yao, Jean-Francois Ton, Xiaoying Zhang, Ruocheng Guo Hao Cheng, Yegor Klochkov, Muhammad Faaiz Taufiq, and Hang Li. *arXiv preprint arXiv:2308.05374 2023*

- Measure and improve robustness in NLP models: A survey.
  [pdf](https://aclanthology.org/2022.naacl-main.339/)
  - Xuezhi Wang, Haohan Wang, and Diyi Yang. *arXiv preprint arXiv:2112.08313 2021*

- Methods for Estimating and improving robustness of language models.
  [pdf](https://aclanthology.org/2022.naacl-srw.6/)
  - Michal {}tefanik. *arXiv preprint arXiv:2206.08446 2022*

- A survey on evaluation of large language models.
  [pdf](https://dl.acm.org/doi/10.1145/3641289)
  - Yupeng Chang, Xu Wang, Jindong Wang, Yuan Wu, Linyi Yang, Kaijie Zhu, Hao Chen, Xiaoyuan Yi, Cunxiang Wang, Yidong Wang, and others. *ACM Transactions on Intelligent Systems and Technology 2024*

- A survey of large language models.
  [pdf](https://arxiv.org/abs/2303.18223)
  - Wayne Xin Zhao, Kun Zhou, Junyi Li, Tianyi Tang, Xiaolei Wang, Yupeng Hou, Yingqian Min, Beichen Zhang, Junjie Zhang, Zican Dong, and others. *arXiv preprint arXiv:2303.18223 2023*

- A comprehensive overview of large language models.
  [pdf](https://arxiv.org/abs/2307.06435)
  - Humza Naveed, Asad Ullah Khan, Shi Qiu, Muhammad Saqib, Saeed Anwar, Muhammad Usman, Naveed Akhtar, Nick Barnes, and Ajmal Mian. *arXiv preprint arXiv:2307.06435 2023*

- Large language models: A survey.
  [pdf](https://arxiv.org/abs/2402.06196)
  - Shervin Minaee, Tomas Mikolov, Narjes Nikzad, Meysam Chenaghlu, Richard Socher, Xavier Amatriain, and Jianfeng Gao. *arXiv preprint arXiv:2402.06196 2024*

- Gpt-4 technical report.
  [pdf](https://arxiv.org/abs/2303.08774)
  - Josh Achiam, Steven Adler, Sandhini Agarwal, Lama Ahmad, Ilge Akkaya, Florencia Leoni Aleman, Diogo Almeida, Janko Altenschmidt, Sam Altman, Shyamal Anadkat, and others. *arXiv preprint arXiv:2303.08774 2023*

- Llama: Open and efficient foundation language models.
  [pdf](https://arxiv.org/abs/2302.13971)
  - Hugo Touvron, Thibaut Lavril, Gautier Izacard, Xavier Martinet, Marie-Anne Lachaux, Timothee Lacroix, Baptiste Roziere, Naman Goyal, Eric Hambro, Faisal Azhar, and others. *arXiv preprint arXiv:2302.13971 2023*

- Emergent abilities of large language models.
  [pdf](https://openreview.net/forum?id=yzkSU5zdwD)
  - Jason Wei, Yi Tay, Rishi Bommasani, Colin Raffel, Barret Zoph, Sebastian Borgeaud, Dani Yogatama, Maarten Bosma, Denny Zhou, Donald Metzler, and others. *arXiv preprint arXiv:2206.07682 2022*

- On Robustness: An Undervalued Dimension of Human Rationality..
  [pdf](https://iccm-conference.neocities.org/2019/proceedings/papers/ICCM2019_paper_21.pdf)
  - Ardavan Salehi Nobandegani, Kevin da Silva Castanheira, Timothy O'Donnell, and Thomas R Shultz. *CogSci 2019*

- Interpreting and improving adversarial robustness of deep neural networks with neuron sensitivity.
  [pdf](https://dl.acm.org/doi/10.1109/TIP.2020.3042083)
  - Chongzhi Zhang, Aishan Liu, Xianglong Liu, Yitao Xu, Hang Yu, Yuqing Ma, and Tianlin Li. *IEEE Transactions on Image Processing 2020*

- Revolutionizing finance with llms: An overview of applications and insights.
  [pdf](https://arxiv.org/abs/2401.11641)
  - Huaqin Zhao, Zhengliang Liu, Zihao Wu, Yiwei Li, Tianze Yang, Peng Shu, Shaochen Xu, Haixing Dai, Lin Zhao, Gengchen Mai, and others. *arXiv preprint arXiv:2401.11641 2024*

- AI curriculum for European high schools: An embedded intelligence approach.
  [pdf](https://link.springer.com/article/10.1007/s40593-022-00315-0)
  - Francisco Bellas, Sara Guerreiro-Santalla, Martin Naya, and Richard J Duro. *International Journal of Artificial Intelligence in Education 2023*

- Evaluating the Zero-shot Robustness of Instruction-tuned Language Models.
  [pdf](https://arxiv.org/abs/2306.11270)
  - Jiuding Sun, Chantal Shaib, and Byron C Wallace. *ICLR 2024*

## Adversarial Robustness
### Noise Prompt
- “was it “stated” or was it “claimed”?: How linguistic bias affects generative language models.
  [pdf]()
  - Roma Patel and Ellie Pavlick. *EMNLP 2021*

 - Quantifying Language Models' Sensitivity to Spurious Features in Prompt Design or: How I learned to start worrying about prompt formatting.
    [pdf]()
  - Melanie Sclar, Yejin Choi, Yulia Tsvetkov, and Alane Suhr. *ICLR 2024*

 - Generating Novel Leads for Drug Discovery using LLMs with Logical Feedback.
    [pdf]()
  - Shreyas Bhat Brahmavar, Ashwin Srinivasan, Tirtharaj Dash, Sowmya Ramaswamy Krishnan, Lovekesh Vig, Arijit Roy, and Raviprasad Aduri. *AAAI 2024*

 - Towards robust in-context learning for machine translation with large language models.
    [pdf]()
  - Shaolin Zhu, Menglong Cui, and Deyi Xiong. *LREC-COLING 2024*

- Combining Discourse Coherence with Large Language Models for More Inclusive, Equitable, and Robust Task-Oriented Dialogue.
  [pdf]()
  - Katherine Atwell, Mert Inan, Anthony B Sicilia, and Malihe Alikhani. *LREC-COLING 2024*

- Evaluating the Zero-shot Robustness of Instruction-tuned Language Models.
  [pdf]()
  - Jiuding Sun, Chantal Shaib, and Byron C Wallace. *The Twelfth International Conference on Learning Representations 2024*

- Towards robust in-context learning for machine translation with large language models.
  [pdf]()
  - Shaolin Zhu, Menglong Cui, and Deyi Xiong. *LREC-COLING 2024*

- InterFair: Debiasing with Natural Language Feedback for Fair Interpretable Predictions.
  [pdf]()
  - Bodhisattwa Prasad Majumder, Zexue He, and Julian McAuley. *arXiv e-prints 2022*

- Correcting Language Model Bias for Text Classification in True Zero-Shot Learning.
  [pdf]()
  - Feng Zhao, Wan Xianlin, Cheng Yan, and Chu Kiong Loo. *LREC-COLING 2024*

- Projective Methods for Mitigating Gender Bias in Pre-trained Language Models.
  [pdf]()
  - Hillary Dawkins, Isar Nejadgholi, Daniel Gillis, and Judi McCuaig. *arXiv:2403.18803 2024*

- Identifying and mitigating spurious correlations for improving robustness in nlp models.
  [pdf]()
  - Tianlu Wang, Rohit Sridhar, Diyi Yang, and Xuezhi Wang. *arXiv preprint arXiv:2110.07736 2021*

- Measuring Inductive Biases of In-Context Learning with Underspecified Demonstrations.
  [pdf]()
  - Chenglei Si, Dan Friedman, Nitish Joshi, Shi Feng, Danqi Chen, and He He. *Unknown Venue 2023*

- Mitigating Label Biases for In-context Learning.
  [pdf]()
  - Yu Fei, Yifan Hou, Zeming Chen, and Antoine Bosselut. *ACL 2023*


### Long Context
-   Benchmarking large language models in retrieval-augmented generation.
    [[pdf]](https://arxiv.org/pdf)
    -   Chen Jiawei, Lin Hongyu, Han Xianpei, and Sun Le. *Arxiv 2024*

-   Benchmarking large language models in retrieval-augmented generation.
    [[pdf]](https://arxiv.org/pdf)
    -   Chen Jiawei, Lin Hongyu, Han Xianpei, and Sun Le. *Arxiv 2024*

### Attack and Defense
-   Benchmarking large language models in retrieval-augmented generation.
    [[pdf]](https://arxiv.org/pdf)
    -   Chen Jiawei, Lin Hongyu, Han Xianpei, and Sun Le. *Arxiv 2024*

### Noise Decoding
-   Benchmarking large language models in retrieval-augmented generation.
    [[pdf]](https://arxiv.org/pdf)
    -   Chen Jiawei, Lin Hongyu, Han Xianpei, and Sun Le. *Arxiv 2024*

### Causal Inspired Methods
-   Benchmarking large language models in retrieval-augmented generation.
    [[pdf]](https://arxiv.org/pdf)
    -   Chen Jiawei, Lin Hongyu, Han Xianpei, and Sun Le. *Arxiv 2024*

## OOD Robustness
### Domain Transfer and Generalization
-   Benchmarking large language models in retrieval-augmented generation.
    [[pdf]](https://arxiv.org/pdf)
    -   Chen Jiawei, Lin Hongyu, Han Xianpei, and Sun Le. *Arxiv 2024*

### OOD Detection
-   Benchmarking large language models in retrieval-augmented generation.
    [[pdf]](https://arxiv.org/pdf)
    -   Chen Jiawei, Lin Hongyu, Han Xianpei, and Sun Le. *Arxiv 2024*

### Tuning Method
-   Benchmarking large language models in retrieval-augmented generation.
    [[pdf]](https://arxiv.org/pdf)
    -   Chen Jiawei, Lin Hongyu, Han Xianpei, and Sun Le. *Arxiv 2024*

### Hallucination
-   Benchmarking large language models in retrieval-augmented generation.
    [[pdf]](https://arxiv.org/pdf)
    -   Chen Jiawei, Lin Hongyu, Han Xianpei, and Sun Le. *Arxiv 2024*

### Causal Enhanced Solution
-   Benchmarking large language models in retrieval-augmented generation.
    [[pdf]](https://arxiv.org/pdf)
    -   Chen Jiawei, Lin Hongyu, Han Xianpei, and Sun Le. *Arxiv 2024*


## Robustness Evaluation
### Dataset Construction
-   Benchmarking large language models in retrieval-augmented generation.
    [[pdf]](https://arxiv.org/pdf)
    -   Chen Jiawei, Lin Hongyu, Han Xianpei, and Sun Le. *Arxiv 2024*

### Robustness Evaluation
-   Benchmarking large language models in retrieval-augmented generation.
    [[pdf]](https://arxiv.org/pdf)
    -   Chen Jiawei, Lin Hongyu, Han Xianpei, and Sun Le. *Arxiv 2024*


### Causal Related Evaluation
-   Benchmarking large language models in retrieval-augmented generation.
    [[pdf]](https://arxiv.org/pdf)
    -   Chen Jiawei, Lin Hongyu, Han Xianpei, and Sun Le. *Arxiv 2024*

#### If you find our survey useful for your research, please cite the following paper:
```
@article{llmrobust-survey,
    title={Evaluating and Improving Robustness in Large Language Models: A Survey and Future Directions},
    author={},
    year={2025},
    journal={arXiv preprint},
    url={http://arxiv.org}
}
```