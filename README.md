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
    - [Attack and Defense](#attack-and-defense)
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
  [pdf](https://aclanthology.org/2021.emnlp-main.790.pdf)
    - Roma Patel and Ellie Pavlick. *EMNLP 2021*

 - Quantifying Language Models' Sensitivity to Spurious Features in Prompt Design or: How I learned to start worrying about prompt formatting.
    [pdf](https://arxiv.org/pdf/2310.11324)
    - Melanie Sclar, Yejin Choi, Yulia Tsvetkov, and Alane Suhr. *ICLR 2024*

 - Generating Novel Leads for Drug Discovery using LLMs with Logical Feedback.
    [pdf](https://www.biorxiv.org/content/10.1101/2023.09.14.557698v1.full.pdf)
    - Shreyas Bhat Brahmavar, Ashwin Srinivasan, Tirtharaj Dash, Sowmya Ramaswamy Krishnan, Lovekesh Vig, Arijit Roy, and Raviprasad Aduri. *AAAI 2024*

 - Towards robust in-context learning for machine translation with large language models.
    [pdf](https://aclanthology.org/2024.lrec-main.1444.pdf)
    - Shaolin Zhu, Menglong Cui, and Deyi Xiong. *LREC-COLING 2024*

- Combining Discourse Coherence with Large Language Models for More Inclusive, Equitable, and Robust Task-Oriented Dialogue.
  [pdf](https://aclanthology.org/2024.lrec-main.314.pdf)
    - Katherine Atwell, Mert Inan, Anthony B Sicilia, and Malihe Alikhani. *LREC-COLING 2024*

- Evaluating the Zero-shot Robustness of Instruction-tuned Language Models.
  [pdf](https://arxiv.org/pdf/2306.11270)
    - Jiuding Sun, Chantal Shaib, and Byron C Wallace. *The Twelfth International Conference on Learning Representations 2024*

- Towards robust in-context learning for machine translation with large language models.
  [pdf](https://aclanthology.org/2024.lrec-main.1444.pdf)
    - Shaolin Zhu, Menglong Cui, and Deyi Xiong. *LREC-COLING 2024*

- InterFair: Debiasing with Natural Language Feedback for Fair Interpretable Predictions.
  [pdf](https://arxiv.org/pdf/2210.07440)
    - Bodhisattwa Prasad Majumder, Zexue He, and Julian McAuley. *arXiv e-prints 2022*

- Correcting Language Model Bias for Text Classification in True Zero-Shot Learning.
  [pdf](https://aclanthology.org/2024.lrec-main.359.pdf)
    - Feng Zhao, Wan Xianlin, Cheng Yan, and Chu Kiong Loo. *LREC-COLING 2024*

- Projective Methods for Mitigating Gender Bias in Pre-trained Language Models.
  [pdf](https://arxiv.org/pdf/2403.18803)
    - Hillary Dawkins, Isar Nejadgholi, Daniel Gillis, and Judi McCuaig. *arXiv:2403.18803 2024*

- Identifying and mitigating spurious correlations for improving robustness in nlp models.
  [pdf](https://aclanthology.org/2022.findings-naacl.130.pdf)
    - Tianlu Wang, Rohit Sridhar, Diyi Yang, and Xuezhi Wang. *arXiv preprint arXiv:2110.07736 2021*

- Measuring Inductive Biases of In-Context Learning with Underspecified Demonstrations.
  [pdf](https://aclanthology.org/2023.acl-long.632.pdf)
    - Chenglei Si, Dan Friedman, Nitish Joshi, Shi Feng, Danqi Chen, and He He. *Unknown Venue 2023*

- Mitigating Label Biases for In-context Learning.
  [pdf](https://arxiv.org/pdf/2305.19148)
    - Yu Fei, Yifan Hou, Zeming Chen, and Antoine Bosselut. *ACL 2023*

<!-- begin table -->

 - Quantifying Language Models' Sensitivity to Spurious Features in Prompt Design or: How I learned to start worrying about prompt formatting.
    [pdf](https://arxiv.org/pdf/2310.11324)
    - Melanie Sclar, Yejin Choi, Yulia Tsvetkov, and Alane Suhr. *ICLR 2024*

 - Generating Novel Leads for Drug Discovery using LLMs with Logical Feedback.
    [pdf](https://www.biorxiv.org/content/10.1101/2023.09.14.557698v1.full.pdf)
    - Shreyas Bhat Brahmavar, Ashwin Srinivasan, Tirtharaj Dash, Sowmya Ramaswamy Krishnan, Lovekesh Vig, Arijit Roy, and Raviprasad Aduri. *AAAI 2024*

- Towards robust in-context learning for machine translation with large language models.
  [pdf](https://aclanthology.org/2024.lrec-main.1444.pdf)
    - Shaolin Zhu, Menglong Cui, and Deyi Xiong. *LREC-COLING 2024*

- Evaluating the Zero-shot Robustness of Instruction-tuned Language Models.
  [pdf](https://arxiv.org/pdf/2306.11270)
    - Jiuding Sun, Chantal Shaib, and Byron C Wallace. *The Twelfth International Conference on Learning Representations 2024*

- Towards robust in-context learning for machine translation with large language models.
  [pdf](https://aclanthology.org/2024.lrec-main.1444.pdf)
    - Shaolin Zhu, Menglong Cui, and Deyi Xiong. *LREC-COLING 2024*

- InterFair: Debiasing with Natural Language Feedback for Fair Interpretable Predictions.
  [pdf](https://arxiv.org/pdf/2210.07440)
    - Bodhisattwa Prasad Majumder, Zexue He, and Julian McAuley. *arXiv e-prints 2022*

- Projective Methods for Mitigating Gender Bias in Pre-trained Language Models.
  [pdf](https://arxiv.org/pdf/2403.18803)
    - Hillary Dawkins, Isar Nejadgholi, Daniel Gillis, and Judi McCuaig. *arXiv:2403.18803 2024*

 - Revisiting non-English Text Simplification: A Unified Multilingual Benchmark.
    [pdf](https://arxiv.org/pdf/2305.15678)
    - Michael Ryan, Tarek Naous, and Wei Xu. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - Native Sparse Attention: Hardware-Aligned and Natively Trainable Sparse Attention.
    [pdf](https://arxiv.org/pdf/2502.11089)
    - Jingyang Yuan, Huazuo Gao, Damai Dai, Junyu Luo, Liang Zhao, Zhengyan Zhang, Zhenda Xie, YX Wei, Lean Wang, Zhiping Xiao, and others. *arXiv preprint arXiv:2502.11089 2025*

 - LongLoRA: Efficient Fine-tuning of Long-Context Large Language Models.
    [pdf](https://arxiv.org/pdf/2309.12307)
    - Yukang Chen, Shengju Qian, Haotian Tang, Xin Lai, Zhijian Liu, Song Han, and Jiaya Jia. *The Twelfth International Conference on Learning Representations 2024*

 - MoBA: Mixture of Block Attention for Long-Context LLMs.
    [pdf](https://arxiv.org/pdf/2502.13189)
    - Enzhe Lu, Zhejun Jiang, Jingyuan Liu, Yulun Du, Tao Jiang, Chao Hong, Shaowei Liu, Weiran He, Enming Yuan, Yuzhi Wang, and others. *arXiv preprint arXiv:2502.13189 2025*

 - A Length-Extrapolatable Transformer.
    [pdf](https://arxiv.org/pdf/2212.10554)
    - Yutao Sun, Li Dong, Barun Patra, Shuming Ma, Shaohan Huang, Alon Benhaim, Vishrav Chaudhary, Xia Song, and Furu Wei. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - A Length-Extrapolatable Transformer.
    [pdf](https://arxiv.org/pdf/2212.10554)
    - Yutao Sun, Li Dong, Barun Patra, Shuming Ma, Shaohan Huang, Alon Benhaim, Vishrav Chaudhary, Xia Song, and Furu Wei. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - Found in the Middle: Calibrating Positional Attention Bias Improves Long Context Utilization.
    [pdf](https://arxiv.org/pdf/2406.16008)
    - Cheng-Yu Hsieh, Yung-Sung Chuang, Chun-Liang Li, Zifeng Wang, Long T Le, Abhishek Kumar, James Glass, Alexander Ratner, Chen-Yu Lee, Ranjay Krishna, and others. *arXiv preprint arXiv:2406.16008 2024*

 - Make Your LLM Fully Utilize the Context.
    [pdf](https://arxiv.org/pdf/2404.16811)
    - Shengnan An, Zexiong Ma, Zeqi Lin, Nanning Zheng, and Jian-Guang Lou. *arXiv preprint arXiv:2404.16811 2024*

 - Longllmlingua: Accelerating and enhancing llms in long context scenarios via prompt compression.
    [pdf](https://aclanthology.org/2024.acl-long.91.pdf)
    - Huiqiang Jiang, Qianhui Wu, Xufang Luo, Dongsheng Li, Chin-Yew Lin, Yuqing Yang, and Lili Qiu. *arXiv preprint arXiv:2310.06839 2023*

 - Adapting Language Models to Compress Contexts.
    [pdf](https://arxiv.org/pdf/2305.14788)
    - Alexis Chevalier, Alexander Wettig, Anirudh Ajith, and Danqi Chen. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - ProPILE: Probing Privacy Leakage in Large Language Models.
    [pdf](https://arxiv.org/pdf/2307.01881)
    - Siwon Kim, Sangdoo Yun, Hwaran Lee, Martin Gubri, Sungroh Yoon, and Seong Joon Oh. *Thirty-seventh Conference on Neural Information Processing Systems 2023*

 - TrojLLM: A Black-box Trojan Prompt Attack on Large Language Models.
    [pdf](https://arxiv.org/pdf/2306.06815)
    - Jiaqi Xue, Mengxin Zheng, Ting Hua, Yilin Shen, Yepeng Liu, Ladislau Boloni, and Qian Lou. *Thirty-seventh Conference on Neural Information Processing Systems 2023*

 - On Evaluating Adversarial Robustness of Large Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2305.16934)
    - Yunqing Zhao, Tianyu Pang, Chao Du, Xiao Yang, Chongxuan Li, Ngai-man Cheung, and Min Lin. *Thirty-seventh Conference on Neural Information Processing Systems 2023*

 - Boosting Adversarial Transferability using Dynamic Cues.
    [pdf](https://arxiv.org/pdf/2302.12252)
    - Muzammal Naseer, Ahmad Mahmood, Salman Khan, and Fahad Khan. *The Eleventh International Conference on Learning Representations 2023*

 - Set-level guidance attack: Boosting adversarial transferability of vision-language pre-training models.
    [pdf](https://arxiv.org/pdf/2307.14061)
    - Dong Lu, Zhiqiang Wang, Teng Wang, Weili Guan, Hongchang Gao, and Feng Zheng. *Proceedings of the IEEE/CVF International Conference on Computer Vision 2023*

 - Jailbroken: How Does LLM Safety Training Fail?.
    [pdf](https://arxiv.org/pdf/2307.02483)
    - Alexander Wei, Nika Haghtalab, and Jacob Steinhardt. *Thirty-seventh Conference on Neural Information Processing Systems 2023*

 - Jailbreak in pieces: Compositional Adversarial Attacks on Multi-Modal Language Models.
    [pdf](https://arxiv.org/pdf/2307.14539)
    - Erfan Shayegani, Yue Dong, and Nael Abu-Ghazaleh. *The Twelfth International Conference on Learning Representations 2024*

 - Poisoning language models during instruction tuning.
    [pdf](https://arxiv.org/pdf/2305.00944)
    - Alexander Wan, Eric Wallace, Sheng Shen, and Dan Klein. *International Conference on Machine Learning 2023*

 - BadChain: Backdoor Chain-of-Thought Prompting for Large Language Models.
    [pdf](https://arxiv.org/pdf/2401.12242)
    - Zhen Xiang, Fengqing Jiang, Zidi Xiong, Bhaskar Ramasubramanian, Radha Poovendran, and Bo Li. *The Twelfth International Conference on Learning Representations 2024*

 - Unveiling the Implicit Toxicity in Large Language Models.
    [pdf](https://aclanthology.org/2023.emnlp-main.84.pdf)
    - Jiaxin Wen, Pei Ke, Hao Sun, Zhexin Zhang, Chengfei Li, Jinfeng Bai, and Minlie Huang. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Mathattack: Attacking large language models towards math solving ability.
    [pdf](https://arxiv.org/pdf/2309.01686)
    - Zihao Zhou, Qiufeng Wang, Mingyu Jin, Jie Yao, Jianan Ye, Wei Liu, Wei Wang, Xiaowei Huang, and Kaizhu Huang. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - VQAttack: Transferable Adversarial Attacks on Visual Question Answering via Pre-trained Models.
    [pdf](https://arxiv.org/pdf/2402.11083)
    - Ziyi Yin, Muchao Ye, Tianrong Zhang, Jiaqi Wang, Han Liu, Jinghui Chen, Ting Wang, and Fenglong Ma. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Visual adversarial examples jailbreak aligned large language models.
    [pdf](https://arxiv.org/pdf/2306.13213)
    - Xiangyu Qi, Kaixuan Huang, Ashwinee Panda, Peter Henderson, Mengdi Wang, and Prateek Mittal. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Codeattack: Code-based adversarial attacks for pre-trained programming language models.
    [pdf](https://arxiv.org/pdf/2206.00052)
    - Akshita Jha and Chandan K Reddy. *Proceedings of the AAAI Conference on Artificial Intelligence 2023*

 - A context aware approach for generating natural language attacks.
    [pdf](https://arxiv.org/pdf/2012.13339v1)
    - Rishabh Maheshwary, Saket Maheshwary, and Vikram Pudi. *Proceedings of the AAAI conference on artificial intelligence 2021*

 - Learn2weight: Parameter adaptation against similar-domain adversarial attacks.
    [pdf](https://arxiv.org/pdf/2205.07315)
    - Siddhartha Datta. *arXiv preprint arXiv:2205.07315 2022*

 - Enhance Robustness of Language Models Against Variation Attack through Graph Integration.
    [pdf](https://arxiv.org/pdf/2404.12014)
    - Zi Xiong, Lizhi Qing, Yangyang Kang, Jiawei Liu, Hongsong Li, Changlong Sun, Xiaozhong Liu, and Wei Lu. *arXiv preprint arXiv:2404.12014 2024*

 - One prompt word is enough to boost adversarial robustness for pre-trained vision-language models.
    [pdf](https://arxiv.org/pdf/2403.01849)
    - Lin Li, Haoyan Guan, Jianing Qiu, and Michael Spratling. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2024*

 - ORTicket: Let One Robust BERT Ticket Transfer across Different Tasks.
    [pdf](https://aclanthology.org/2024.lrec-main.1096.pdf)
    - Yuhao Zhou, Wenxiang Chen, Rui Zheng, Zhiheng Xi, Tao Gui, Qi Zhang, and Xuan-Jing Huang. *Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024) 2024*

 - TaiChi: Improving the Robustness of NLP Models by Seeking Common Ground While Reserving Differences.
    [pdf](https://aclanthology.org/2024.lrec-main.1351.pdf)
    - Huimin Chen, Chengyu Wang, Yanhao Wang, Cen Chen, and Yinggui Wang. *Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024) 2024*

 - PAD: A Robustness Enhancement Ensemble Method via Promoting Attention Diversity.
    [pdf](https://aclanthology.org/2024.lrec-main.1100.pdf)
    - Yuting Yang, Pei Huang, Feifei Ma, Juan Cao, and Jintao Li. *Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024) 2024*

 - Learn2weight: Parameter adaptation against similar-domain adversarial attacks.
    [pdf](https://arxiv.org/pdf/2205.07315)
    - Siddhartha Datta. *arXiv preprint arXiv:2205.07315 2022*

 - Preserving privacy through dememorization: An unlearning technique for mitigating memorization risks in language models.
    [pdf](https://aclanthology.org/2023.emnlp-main.265.pdf)
    - Aly Kassem, Omar Mahmoud, and Sherif Saad. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Flocks of Stochastic Parrots: Differentially Private Prompt Learning for Large Language Models.
    [pdf](https://arxiv.org/pdf/2305.15594)
    - Haonan Duan, Adam Dziedzic, Nicolas Papernot, and Franziska Boenisch. *Thirty-seventh Conference on Neural Information Processing Systems 2023*

 - Causality Based Front-door Defense Against Backdoor Attack on Language Models.
    [pdf](https://openreview.net/pdf?id=dmHHVcHFdM)
    - Yiran Liu, Xiaoang Xu, Zhiyi Hou, and Yang Yu. *Forty-first International Conference on Machine Learning 2024*

<!-- end table -->

 - Crosslingual Generalization through Multitask Finetuning.
    [pdf](https://aclanthology.org/2023.acl-long.891.pdf)
    - Niklas Muennighoff, Thomas Wang, Lintang Sutawika, Adam Roberts, Stella Biderman, Teven Le Scao, M Saiful Bari, Sheng Shen, Zheng Xin Yong, Hailey Schoelkopf, and others. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - Revisiting non-English Text Simplification: A Unified Multilingual Benchmark.
    [pdf](https://arxiv.org/pdf/2305.15678)
    - Michael Ryan, Tarek Naous, and Wei Xu. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - Gendered Grammar or Ingrained Bias? Exploring Gender Bias in Icelandic Language Models.
    [pdf](https://aclanthology.org/2024.lrec-main.671.pdf)
    - Steinunn Rut Fri and Hafsteinn Einarsson. *Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024) 2024*

<!-- begin subsubsection{Long Context Noise Prompt} -->

 - Train Short, Test Long: Attention with Linear Biases Enables Input Length Extrapolation.
    [pdf](https://arxiv.org/pdf/2108.12409)
    - Ofir Press, Noah Smith, and Mike Lewis. *International Conference on Learning Representations 2022*

 - A Length-Extrapolatable Transformer.
    [pdf](https://arxiv.org/pdf/2212.10554)
    - Yutao Sun, Li Dong, Barun Patra, Shuming Ma, Shaohan Huang, Alon Benhaim, Vishrav Chaudhary, Xia Song, and Furu Wei. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - Roformer: Enhanced transformer with rotary position embedding.
    [pdf](https://arxiv.org/pdf/2104.09864)
    - Jianlin Su, Murtadha Ahmed, Yu Lu, Shengfeng Pan, Wen Bo, and Yunfeng Liu. *Neurocomputing 2024*

 - Functional Interpolation for Relative Positions improves Long Context Transformers.
    [pdf](https://openreview.net/pdf?id=rR03qFesqk)
    - Shanda Li, Chong You, Guru Guruganesh, Joshua Ainslie, Santiago Ontanon, Manzil Zaheer, Sumit Sanghai, Yiming Yang, Sanjiv Kumar, and Srinadh Bhojanapalli. *The Twelfth International Conference on Learning Representations 2024*

 - MoBA: Mixture of Block Attention for Long-Context LLMs.
    [pdf](https://arxiv.org/pdf/2502.13189)
    - Enzhe Lu, Zhejun Jiang, Jingyuan Liu, Yulun Du, Tao Jiang, Chao Hong, Shaowei Liu, Weiran He, Enming Yuan, Yuzhi Wang, and others. *arXiv preprint arXiv:2502.13189 2025*

 - Native Sparse Attention: Hardware-Aligned and Natively Trainable Sparse Attention.
    [pdf](https://arxiv.org/pdf/2502.11089)
    - Jingyang Yuan, Huazuo Gao, Damai Dai, Junyu Luo, Liang Zhao, Zhengyan Zhang, Zhenda Xie, YX Wei, Lean Wang, Zhiping Xiao, and others. *arXiv preprint arXiv:2502.11089 2025*

 - LongLoRA: Efficient Fine-tuning of Long-Context Large Language Models.
    [pdf](https://arxiv.org/pdf/2309.12307)
    - Yukang Chen, Shengju Qian, Haotian Tang, Xin Lai, Zhijian Liu, Song Han, and Jiaya Jia. *The Twelfth International Conference on Learning Representations 2024*

 - Flatten transformer: Vision transformer using focused linear attention.
    [pdf](https://arxiv.org/pdf/2308.00442)
    - Dongchen Han, Xuran Pan, Yizeng Han, Shiji Song, and Gao Huang. *Proceedings of the IEEE/CVF international conference on computer vision 2023*

 - PolaFormer: Polarity-aware Linear Attention for Vision Transformers.
    [pdf](https://arxiv.org/pdf/2501.15061)
    - Weikang Meng, Yadan Luo, Xin Li, Dongmei Jiang, and Zheng Zhang. *The Thirteenth International Conference on Learning Representations 2025*

 - Mamba: Linear-time sequence modeling with selective state spaces.
    [pdf](https://arxiv.org/pdf/2312.00752)
    - Albert Gu and Tri Dao. *arXiv preprint arXiv:2312.00752 2023*

 - RWKV: Reinventing RNNs for the Transformer Era.
    [pdf](https://arxiv.org/pdf/2305.13048)
    -  Bo Peng, Eric Alcaide, Quentin Anthony, Alon  Albalak, Samuel Arcadinho, Stella Biderman, Huanqi Cao, Xin Cheng, Michael Chung, Leon Derczynski, Xingjian Du, Matteo Grella, Kranthi Gv, Xuzheng He, Haowen Hou, Przemyslaw Kazienko, Jan Kocon, Jiaming Kong,  Bartłomiej Koptyra, Hayden Lau, Jiaju Lin, Krishna Sri Ipsit Mantri, Ferdinand Mom, Atsushi Saito, Guangyu Song, Xiangru Tang, Johan Wind, Stanisław Woźniak, Zhenyuan Zhang, Qinghua Zhou, Jian Zhu, and Rui-Jie Zhu. *Findings of the Association for Computational Linguistics: EMNLP 2023*

 - Retentive network: A successor to transformer for large language models.
    [pdf](https://arxiv.org/pdf/2307.08621)
    - Yutao Sun, Li Dong, Shaohan Huang, Shuming Ma, Yuqing Xia, Jilong Xue, Jianyong Wang, and Furu Wei. *arXiv preprint arXiv:2307.08621 2023*

 - Lost in the Middle: How Language Models Use Long Contexts.
    [pdf](https://arxiv.org/pdf/2307.03172)
    - Nelson F Liu, Kevin Lin, John Hewitt, Ashwin Paranjape, Michele Bevilacqua, Fabio Petroni, and Percy Liang. *Transactions of the Association for Computational Linguistics Transactions of the Association for Computational Linguistics*

 - Train Short, Test Long: Attention with Linear Biases Enables Input Length Extrapolation.
    [pdf](https://arxiv.org/pdf/2108.12409)
    - Ofir Press, Noah Smith, and Mike Lewis. *International Conference on Learning Representations 2022*

 - A Length-Extrapolatable Transformer.
    [pdf](https://arxiv.org/pdf/2212.10554)
    - Yutao Sun, Li Dong, Barun Patra, Shuming Ma, Shaohan Huang, Alon Benhaim, Vishrav Chaudhary, Xia Song, and Furu Wei. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - A Length-Extrapolatable Transformer.
    [pdf](https://arxiv.org/pdf/2212.10554)
    - Yutao Sun, Li Dong, Barun Patra, Shuming Ma, Shaohan Huang, Alon Benhaim, Vishrav Chaudhary, Xia Song, and Furu Wei. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - Make Your LLM Fully Utilize the Context.
    [pdf](https://arxiv.org/pdf/2404.16811)
    - Shengnan An, Zexiong Ma, Zeqi Lin, Nanning Zheng, and Jian-Guang Lou. *arXiv preprint arXiv:2404.16811 2024*

 - Longllmlingua: Accelerating and enhancing llms in long context scenarios via prompt compression.
    [pdf](https://aclanthology.org/2024.acl-long.91.pdf)
    - Huiqiang Jiang, Qianhui Wu, Xufang Luo, Dongsheng Li, Chin-Yew Lin, Yuqing Yang, and Lili Qiu. *arXiv preprint arXiv:2310.06839 2023*

 - Adapting Language Models to Compress Contexts.
    [pdf](https://arxiv.org/pdf/2305.14788)
    - Alexis Chevalier, Alexander Wettig, Anirudh Ajith, and Danqi Chen. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

<!-- end subsubsection{Long Context Noise Prompt} -->

<!-- begin comment 174 -->

 - SLOG: A Structural Generalization Benchmark for Semantic Parsing.
    [pdf](https://aclanthology.org/2023.emnlp-main.194.pdf)
    - Bingzhi Li, Lucia Donatelli, Alexander Koller, Tal Linzen, Yuekun Yao, and Najoung Kim. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Lost in the Middle: How Language Models Use Long Contexts.
    [pdf](https://arxiv.org/pdf/2307.03172)
    - Nelson F Liu, Kevin Lin, John Hewitt, Ashwin Paranjape, Michele Bevilacqua, Fabio Petroni, and Percy Liang. *Transactions of the Association for Computational Linguistics Transactions of the Association for Computational Linguistics*

 - Lost in the Middle: How Language Models Use Long Contexts.
    [pdf](https://arxiv.org/pdf/2307.03172)
    - Nelson F Liu, Kevin Lin, John Hewitt, Ashwin Paranjape, Michele Bevilacqua, Fabio Petroni, and Percy Liang. *Transactions of the Association for Computational Linguistics Transactions of the Association for Computational Linguistics*

 - Found in the Middle: Calibrating Positional Attention Bias Improves Long Context Utilization.
    [pdf](https://arxiv.org/pdf/2406.16008)
    - Cheng-Yu Hsieh, Yung-Sung Chuang, Chun-Liang Li, Zifeng Wang, Long T Le, Abhishek Kumar, James Glass, Alexander Ratner, Chen-Yu Lee, Ranjay Krishna, and others. *arXiv preprint arXiv:2406.16008 2024*

 - Found in the Middle: Calibrating Positional Attention Bias Improves Long Context Utilization.
    [pdf](https://arxiv.org/pdf/2406.16008)
    - Cheng-Yu Hsieh, Yung-Sung Chuang, Chun-Liang Li, Zifeng Wang, Long T Le, Abhishek Kumar, James Glass, Alexander Ratner, Chen-Yu Lee, Ranjay Krishna, and others. *arXiv preprint arXiv:2406.16008 2024*

 - Make Your LLM Fully Utilize the Context.
    [pdf](https://arxiv.org/pdf/2404.16811)
    - Shengnan An, Zexiong Ma, Zeqi Lin, Nanning Zheng, and Jian-Guang Lou. *arXiv preprint arXiv:2404.16811 2024*

- Gpt-4 technical report.
  [pdf](https://arxiv.org/abs/2303.08774)
    - Josh Achiam, Steven Adler, Sandhini Agarwal, Lama Ahmad, Ilge Akkaya, Florencia Leoni Aleman, Diogo Almeida, Janko Altenschmidt, Sam Altman, Shyamal Anadkat, and others. *arXiv preprint arXiv:2303.08774 2023*

 - LongAgent: Scaling Language Models to 128k Context through Multi-Agent Collaboration.
    [pdf](https://arxiv.org/pdf/2402.11550)
    - Jun Zhao, Can Zu, Hao Xu, Yi Lu, Wei He, Yiwen Ding, Tao Gui, Qi Zhang, and Xuanjing Huang. *arXiv preprint arXiv:2402.11550 2024*

 - LongLoRA: Efficient Fine-tuning of Long-Context Large Language Models.
    [pdf](https://arxiv.org/pdf/2309.12307)
    - Yukang Chen, Shengju Qian, Haotian Tang, Xin Lai, Zhijian Liu, Song Han, and Jiaya Jia. *The Twelfth International Conference on Learning Representations 2024*

 - Train Short, Test Long: Attention with Linear Biases Enables Input Length Extrapolation.
    [pdf](https://arxiv.org/pdf/2108.12409)
    - Ofir Press, Noah Smith, and Mike Lewis. *International Conference on Learning Representations 2022*

 - A Length-Extrapolatable Transformer.
    [pdf](https://arxiv.org/pdf/2212.10554)
    - Yutao Sun, Li Dong, Barun Patra, Shuming Ma, Shaohan Huang, Alon Benhaim, Vishrav Chaudhary, Xia Song, and Furu Wei. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - Roformer: Enhanced transformer with rotary position embedding.
    [pdf](https://arxiv.org/pdf/2104.09864)
    - Jianlin Su, Murtadha Ahmed, Yu Lu, Shengfeng Pan, Wen Bo, and Yunfeng Liu. *Neurocomputing 2024*

 - Functional Interpolation for Relative Positions improves Long Context Transformers.
    [pdf](https://openreview.net/pdf?id=rR03qFesqk)
    - Shanda Li, Chong You, Guru Guruganesh, Joshua Ainslie, Santiago Ontanon, Manzil Zaheer, Sumit Sanghai, Yiming Yang, Sanjiv Kumar, and Srinadh Bhojanapalli. *The Twelfth International Conference on Learning Representations 2024*

 - A Length-Extrapolatable Transformer.
    [pdf](https://arxiv.org/pdf/2212.10554)
    - Yutao Sun, Li Dong, Barun Patra, Shuming Ma, Shaohan Huang, Alon Benhaim, Vishrav Chaudhary, Xia Song, and Furu Wei. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - A Length-Extrapolatable Transformer.
    [pdf](https://arxiv.org/pdf/2212.10554)
    - Yutao Sun, Li Dong, Barun Patra, Shuming Ma, Shaohan Huang, Alon Benhaim, Vishrav Chaudhary, Xia Song, and Furu Wei. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - Longllmlingua: Accelerating and enhancing llms in long context scenarios via prompt compression.
    [pdf](https://aclanthology.org/2024.acl-long.91.pdf)
    - Huiqiang Jiang, Qianhui Wu, Xufang Luo, Dongsheng Li, Chin-Yew Lin, Yuqing Yang, and Lili Qiu. *arXiv preprint arXiv:2310.06839 2023*

 - Adapting Language Models to Compress Contexts.
    [pdf](https://arxiv.org/pdf/2305.14788)
    - Alexis Chevalier, Alexander Wettig, Anirudh Ajith, and Danqi Chen. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

<!-- end  comment 195 -->

<!-- begin toxic noise prompt -->

 - TrojLLM: A Black-box Trojan Prompt Attack on Large Language Models.
    [pdf](https://arxiv.org/pdf/2306.06815)
    - Jiaqi Xue, Mengxin Zheng, Ting Hua, Yilin Shen, Yepeng Liu, Ladislau Boloni, and Qian Lou. *Thirty-seventh Conference on Neural Information Processing Systems 2023*

 - Gama: Generative adversarial multi-object scene attacks.
    [pdf](https://arxiv.org/pdf/2209.09502)
    - Abhishek Aich, Calvin-Khang Ta, Akash Gupta, Chengyu Song, Srikanth Krishnamurthy, Salman Asif, and Amit Roy-Chowdhury. *Advances in Neural Information Processing Systems 2022*

 - Boosting Adversarial Transferability using Dynamic Cues.
    [pdf](https://arxiv.org/pdf/2302.12252)
    - Muzammal Naseer, Ahmad Mahmood, Salman Khan, and Fahad Khan. *The Eleventh International Conference on Learning Representations 2023*

 - Set-level guidance attack: Boosting adversarial transferability of vision-language pre-training models.
    [pdf](https://arxiv.org/pdf/2307.14061)
    - Dong Lu, Zhiqiang Wang, Teng Wang, Weili Guan, Hongchang Gao, and Feng Zheng. *Proceedings of the IEEE/CVF International Conference on Computer Vision 2023*

 - Jailbroken: How Does LLM Safety Training Fail?.
    [pdf](https://arxiv.org/pdf/2307.02483)
    - Alexander Wei, Nika Haghtalab, and Jacob Steinhardt. *Thirty-seventh Conference on Neural Information Processing Systems 2023*

 - Jailbreak in pieces: Compositional Adversarial Attacks on Multi-Modal Language Models.
    [pdf](https://arxiv.org/pdf/2307.14539)
    - Erfan Shayegani, Yue Dong, and Nael Abu-Ghazaleh. *The Twelfth International Conference on Learning Representations 2024*

 - ProPILE: Probing Privacy Leakage in Large Language Models.
    [pdf](https://arxiv.org/pdf/2307.01881)
    - Siwon Kim, Sangdoo Yun, Hwaran Lee, Martin Gubri, Sungroh Yoon, and Seong Joon Oh. *Thirty-seventh Conference on Neural Information Processing Systems 2023*

 - On Evaluating Adversarial Robustness of Large Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2305.16934)
    - Yunqing Zhao, Tianyu Pang, Chao Du, Xiao Yang, Chongxuan Li, Ngai-man Cheung, and Min Lin. *Thirty-seventh Conference on Neural Information Processing Systems 2023*

 - BadChain: Backdoor Chain-of-Thought Prompting for Large Language Models.
    [pdf](https://arxiv.org/pdf/2401.12242)
    - Zhen Xiang, Fengqing Jiang, Zidi Xiong, Bhaskar Ramasubramanian, Radha Poovendran, and Bo Li. *The Twelfth International Conference on Learning Representations 2024*

 - Data poisoning attacks against multimodal encoders.
    [pdf](https://arxiv.org/pdf/2209.15266)
    - Ziqing Yang, Xinlei He, Zheng Li, Michael Backes, Mathias Humbert, Pascal Berrang, and Yang Zhang. *International Conference on Machine Learning 2023*

 - Poisoning language models during instruction tuning.
    [pdf](https://arxiv.org/pdf/2305.00944)
    - Alexander Wan, Eric Wallace, Sheng Shen, and Dan Klein. *International Conference on Machine Learning 2023*

 - ProPILE: Probing Privacy Leakage in Large Language Models.
    [pdf](https://arxiv.org/pdf/2307.01881)
    - Siwon Kim, Sangdoo Yun, Hwaran Lee, Martin Gubri, Sungroh Yoon, and Seong Joon Oh. *Thirty-seventh Conference on Neural Information Processing Systems 2023*

 - TrojLLM: A Black-box Trojan Prompt Attack on Large Language Models.
    [pdf](https://arxiv.org/pdf/2306.06815)
    - Jiaqi Xue, Mengxin Zheng, Ting Hua, Yilin Shen, Yepeng Liu, Ladislau Boloni, and Qian Lou. *Thirty-seventh Conference on Neural Information Processing Systems 2023*

 - On Evaluating Adversarial Robustness of Large Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2305.16934)
    - Yunqing Zhao, Tianyu Pang, Chao Du, Xiao Yang, Chongxuan Li, Ngai-man Cheung, and Min Lin. *Thirty-seventh Conference on Neural Information Processing Systems 2023*

 - Gama: Generative adversarial multi-object scene attacks.
    [pdf](https://arxiv.org/pdf/2209.09502)
    - Abhishek Aich, Calvin-Khang Ta, Akash Gupta, Chengyu Song, Srikanth Krishnamurthy, Salman Asif, and Amit Roy-Chowdhury. *Advances in Neural Information Processing Systems 2022*

 - Boosting Adversarial Transferability using Dynamic Cues.
    [pdf](https://arxiv.org/pdf/2302.12252)
    - Muzammal Naseer, Ahmad Mahmood, Salman Khan, and Fahad Khan. *The Eleventh International Conference on Learning Representations 2023*

 - Set-level guidance attack: Boosting adversarial transferability of vision-language pre-training models.
    [pdf](https://arxiv.org/pdf/2307.14061)
    - Dong Lu, Zhiqiang Wang, Teng Wang, Weili Guan, Hongchang Gao, and Feng Zheng. *Proceedings of the IEEE/CVF International Conference on Computer Vision 2023*

 - Jailbroken: How Does LLM Safety Training Fail?.
    [pdf](https://arxiv.org/pdf/2307.02483)
    - Alexander Wei, Nika Haghtalab, and Jacob Steinhardt. *Thirty-seventh Conference on Neural Information Processing Systems 2023*

 - Jailbreak in pieces: Compositional Adversarial Attacks on Multi-Modal Language Models.
    [pdf](https://arxiv.org/pdf/2307.14539)
    - Erfan Shayegani, Yue Dong, and Nael Abu-Ghazaleh. *The Twelfth International Conference on Learning Representations 2024*

 - Poisoning language models during instruction tuning.
    [pdf](https://arxiv.org/pdf/2305.00944)
    - Alexander Wan, Eric Wallace, Sheng Shen, and Dan Klein. *International Conference on Machine Learning 2023*

 - BadChain: Backdoor Chain-of-Thought Prompting for Large Language Models.
    [pdf](https://arxiv.org/pdf/2401.12242)
    - Zhen Xiang, Fengqing Jiang, Zidi Xiong, Bhaskar Ramasubramanian, Radha Poovendran, and Bo Li. *The Twelfth International Conference on Learning Representations 2024*

 - Data poisoning attacks against multimodal encoders.
    [pdf](https://arxiv.org/pdf/2209.15266)
    - Ziqing Yang, Xinlei He, Zheng Li, Michael Backes, Mathias Humbert, Pascal Berrang, and Yang Zhang. *International Conference on Machine Learning 2023*

 - Mathattack: Attacking large language models towards math solving ability.
    [pdf](https://arxiv.org/pdf/2309.01686)
    - Zihao Zhou, Qiufeng Wang, Mingyu Jin, Jie Yao, Jianan Ye, Wei Liu, Wei Wang, Xiaowei Huang, and Kaizhu Huang. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - VQAttack: Transferable Adversarial Attacks on Visual Question Answering via Pre-trained Models.
    [pdf](https://arxiv.org/pdf/2402.11083)
    - Ziyi Yin, Muchao Ye, Tianrong Zhang, Jiaqi Wang, Han Liu, Jinghui Chen, Ting Wang, and Fenglong Ma. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Visual adversarial examples jailbreak aligned large language models.
    [pdf](https://arxiv.org/pdf/2306.13213)
    - Xiangyu Qi, Kaixuan Huang, Ashwinee Panda, Peter Henderson, Mengdi Wang, and Prateek Mittal. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Codeattack: Code-based adversarial attacks for pre-trained programming language models.
    [pdf](https://arxiv.org/pdf/2206.00052)
    - Akshita Jha and Chandan K Reddy. *Proceedings of the AAAI Conference on Artificial Intelligence 2023*

 - Learn2weight: Parameter adaptation against similar-domain adversarial attacks.
    [pdf](https://arxiv.org/pdf/2205.07315)
    - Siddhartha Datta. *arXiv preprint arXiv:2205.07315 2022*

 - Enhance Robustness of Language Models Against Variation Attack through Graph Integration.
    [pdf](https://arxiv.org/pdf/2404.12014)
    - Zi Xiong, Lizhi Qing, Yangyang Kang, Jiawei Liu, Hongsong Li, Changlong Sun, Xiaozhong Liu, and Wei Lu. *arXiv preprint arXiv:2404.12014 2024*

 - Mathattack: Attacking large language models towards math solving ability.
    [pdf](https://arxiv.org/pdf/2309.01686)
    - Zihao Zhou, Qiufeng Wang, Mingyu Jin, Jie Yao, Jianan Ye, Wei Liu, Wei Wang, Xiaowei Huang, and Kaizhu Huang. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Codeattack: Code-based adversarial attacks for pre-trained programming language models.
    [pdf](https://arxiv.org/pdf/2206.00052)
    - Akshita Jha and Chandan K Reddy. *Proceedings of the AAAI Conference on Artificial Intelligence 2023*

 - Towards transferable adversarial attacks on vision transformers.
    [pdf](https://arxiv.org/pdf/2109.04176)
    - Zhipeng Wei, Jingjing Chen, Micah Goldblum, Zuxuan Wu, Tom Goldstein, and Yu-Gang Jiang. *Proceedings of the AAAI Conference on Artificial Intelligence 2022*

 - A context aware approach for generating natural language attacks.
    [pdf](https://arxiv.org/pdf/2012.13339v1)
    - Rishabh Maheshwary, Saket Maheshwary, and Vikram Pudi. *Proceedings of the AAAI conference on artificial intelligence 2021*

 - Learn2weight: Parameter adaptation against similar-domain adversarial attacks.
    [pdf](https://arxiv.org/pdf/2205.07315)
    - Siddhartha Datta. *arXiv preprint arXiv:2205.07315 2022*

 - Enhance Robustness of Language Models Against Variation Attack through Graph Integration.
    [pdf](https://arxiv.org/pdf/2404.12014)
    - Zi Xiong, Lizhi Qing, Yangyang Kang, Jiawei Liu, Hongsong Li, Changlong Sun, Xiaozhong Liu, and Wei Lu. *arXiv preprint arXiv:2404.12014 2024*

 - VQAttack: Transferable Adversarial Attacks on Visual Question Answering via Pre-trained Models.
    [pdf](https://arxiv.org/pdf/2402.11083)
    - Ziyi Yin, Muchao Ye, Tianrong Zhang, Jiaqi Wang, Han Liu, Jinghui Chen, Ting Wang, and Fenglong Ma. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Visual adversarial examples jailbreak aligned large language models.
    [pdf](https://arxiv.org/pdf/2306.13213)
    - Xiangyu Qi, Kaixuan Huang, Ashwinee Panda, Peter Henderson, Mengdi Wang, and Prateek Mittal. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Self-attention attribution: Interpreting information interactions inside transformer.
    [pdf](https://arxiv.org/pdf/2004.11207)
    - Yaru Hao, Li Dong, Furu Wei, and Ke Xu. *Proceedings of the AAAI Conference on Artificial Intelligence 2021*

 - Generating natural language attacks in a hard label black box setting.
    [pdf](https://arxiv.org/pdf/2012.14956)
    - Rishabh Maheshwary, Saket Maheshwary, and Vikram Pudi. *Proceedings of the AAAI Conference on Artificial Intelligence 2021*

 - One prompt word is enough to boost adversarial robustness for pre-trained vision-language models.
    [pdf](https://arxiv.org/pdf/2403.01849)
    - Lin Li, Haoyan Guan, Jianing Qiu, and Michael Spratling. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2024*

 - Flocks of Stochastic Parrots: Differentially Private Prompt Learning for Large Language Models.
    [pdf](https://arxiv.org/pdf/2305.15594)
    - Haonan Duan, Adam Dziedzic, Nicolas Papernot, and Franziska Boenisch. *Thirty-seventh Conference on Neural Information Processing Systems 2023*

 - TaiChi: Improving the Robustness of NLP Models by Seeking Common Ground While Reserving Differences.
    [pdf](https://aclanthology.org/2024.lrec-main.1351.pdf)
    - Huimin Chen, Chengyu Wang, Yanhao Wang, Cen Chen, and Yinggui Wang. *Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024) 2024*

 - ORTicket: Let One Robust BERT Ticket Transfer across Different Tasks.
    [pdf](https://aclanthology.org/2024.lrec-main.1096.pdf)
    - Yuhao Zhou, Wenxiang Chen, Rui Zheng, Zhiheng Xi, Tao Gui, Qi Zhang, and Xuan-Jing Huang. *Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024) 2024*

 - Causality Based Front-door Defense Against Backdoor Attack on Language Models.
    [pdf](https://openreview.net/pdf?id=dmHHVcHFdM)
    - Yiran Liu, Xiaoang Xu, Zhiyi Hou, and Yang Yu. *Forty-first International Conference on Machine Learning 2024*

 - PAD: A Robustness Enhancement Ensemble Method via Promoting Attention Diversity.
    [pdf](https://aclanthology.org/2024.lrec-main.1100.pdf)
    - Yuting Yang, Pei Huang, Feifei Ma, Juan Cao, and Jintao Li. *Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024) 2024*

 - Learn2weight: Parameter adaptation against similar-domain adversarial attacks.
    [pdf](https://arxiv.org/pdf/2205.07315)
    - Siddhartha Datta. *arXiv preprint arXiv:2205.07315 2022*

 - Plugat: A plug and play module to defend against textual adversarial attack.
    [pdf](https://aclanthology.org/2022.coling-1.253.pdf)
    - Rui Zheng, Rong Bao, Qin Liu, Tao Gui, Qi Zhang, Xuan-Jing Huang, Rui Xie, and Wei Wu. *Proceedings of the 29th International Conference on Computational Linguistics 2022*

 - Unveiling the Implicit Toxicity in Large Language Models.
    [pdf](https://aclanthology.org/2023.emnlp-main.84.pdf)
    - Jiaxin Wen, Pei Ke, Hao Sun, Zhexin Zhang, Chengfei Li, Jinfeng Bai, and Minlie Huang. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Preserving privacy through dememorization: An unlearning technique for mitigating memorization risks in language models.
    [pdf](https://aclanthology.org/2023.emnlp-main.265.pdf)
    - Aly Kassem, Omar Mahmoud, and Sherif Saad. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

<!-- end toxic noise prompt -->

### Long Context
 - SLOG: A Structural Generalization Benchmark for Semantic Parsing.
    [pdf](https://aclanthology.org/2023.emnlp-main.194.pdf)
    - Bingzhi Li, Lucia Donatelli, Alexander Koller, Tal Linzen, Yuekun Yao, and Najoung Kim. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Lost in the Middle: How Language Models Use Long Contexts.
    [pdf](https://arxiv.org/pdf/2307.03172)
    - Nelson F Liu, Kevin Lin, John Hewitt, Ashwin Paranjape, Michele Bevilacqua, Fabio Petroni, and Percy Liang. *Transactions of the Association for Computational Linguistics Transactions of the Association for Computational Linguistics*

 - Lost in the Middle: How Language Models Use Long Contexts.
    [pdf](https://arxiv.org/pdf/2307.03172)
    - Nelson F Liu, Kevin Lin, John Hewitt, Ashwin Paranjape, Michele Bevilacqua, Fabio Petroni, and Percy Liang. *Transactions of the Association for Computational Linguistics Transactions of the Association for Computational Linguistics*

 - Found in the Middle: Calibrating Positional Attention Bias Improves Long Context Utilization.
    [pdf](https://arxiv.org/pdf/2406.16008)
    - Cheng-Yu Hsieh, Yung-Sung Chuang, Chun-Liang Li, Zifeng Wang, Long T Le, Abhishek Kumar, James Glass, Alexander Ratner, Chen-Yu Lee, Ranjay Krishna, and others. *arXiv preprint arXiv:2406.16008 2024*

 - Found in the Middle: Calibrating Positional Attention Bias Improves Long Context Utilization.
    [pdf](https://arxiv.org/pdf/2406.16008)
    - Cheng-Yu Hsieh, Yung-Sung Chuang, Chun-Liang Li, Zifeng Wang, Long T Le, Abhishek Kumar, James Glass, Alexander Ratner, Chen-Yu Lee, Ranjay Krishna, and others. *arXiv preprint arXiv:2406.16008 2024*

 - Make Your LLM Fully Utilize the Context.
    [pdf](https://arxiv.org/pdf/2404.16811)
    - Shengnan An, Zexiong Ma, Zeqi Lin, Nanning Zheng, and Jian-Guang Lou. *arXiv preprint arXiv:2404.16811 2024*

- Gpt-4 technical report.
  [pdf](https://arxiv.org/abs/2303.08774)
    - Josh Achiam, Steven Adler, Sandhini Agarwal, Lama Ahmad, Ilge Akkaya, Florencia Leoni Aleman, Diogo Almeida, Janko Altenschmidt, Sam Altman, Shyamal Anadkat, and others. *arXiv preprint arXiv:2303.08774 2023*

 - LongAgent: Scaling Language Models to 128k Context through Multi-Agent Collaboration.
    [pdf](https://arxiv.org/pdf/2402.11550)
    - Jun Zhao, Can Zu, Hao Xu, Yi Lu, Wei He, Yiwen Ding, Tao Gui, Qi Zhang, and Xuanjing Huang. *arXiv preprint arXiv:2402.11550 2024*

 - LongLoRA: Efficient Fine-tuning of Long-Context Large Language Models.
    [pdf](https://arxiv.org/pdf/2309.12307)
    - Yukang Chen, Shengju Qian, Haotian Tang, Xin Lai, Zhijian Liu, Song Han, and Jiaya Jia. *The Twelfth International Conference on Learning Representations 2024*

 - Train Short, Test Long: Attention with Linear Biases Enables Input Length Extrapolation.
    [pdf](https://arxiv.org/pdf/2108.12409)
    - Ofir Press, Noah Smith, and Mike Lewis. *International Conference on Learning Representations 2022*

 - A Length-Extrapolatable Transformer.
    [pdf](https://arxiv.org/pdf/2212.10554)
    - Yutao Sun, Li Dong, Barun Patra, Shuming Ma, Shaohan Huang, Alon Benhaim, Vishrav Chaudhary, Xia Song, and Furu Wei. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - Roformer: Enhanced transformer with rotary position embedding.
    [pdf](https://arxiv.org/pdf/2104.09864)
    - Jianlin Su, Murtadha Ahmed, Yu Lu, Shengfeng Pan, Wen Bo, and Yunfeng Liu. *Neurocomputing 2024*

 - Functional Interpolation for Relative Positions improves Long Context Transformers.
    [pdf](https://openreview.net/pdf?id=rR03qFesqk)
    - Shanda Li, Chong You, Guru Guruganesh, Joshua Ainslie, Santiago Ontanon, Manzil Zaheer, Sumit Sanghai, Yiming Yang, Sanjiv Kumar, and Srinadh Bhojanapalli. *The Twelfth International Conference on Learning Representations 2024*

 - Train Short, Test Long: Attention with Linear Biases Enables Input Length Extrapolation.
    [pdf](https://arxiv.org/pdf/2108.12409)
    - Ofir Press, Noah Smith, and Mike Lewis. *International Conference on Learning Representations 2022*

 - A Length-Extrapolatable Transformer.
    [pdf](https://arxiv.org/pdf/2212.10554)
    - Yutao Sun, Li Dong, Barun Patra, Shuming Ma, Shaohan Huang, Alon Benhaim, Vishrav Chaudhary, Xia Song, and Furu Wei. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - A Length-Extrapolatable Transformer.
    [pdf](https://arxiv.org/pdf/2212.10554)
    - Yutao Sun, Li Dong, Barun Patra, Shuming Ma, Shaohan Huang, Alon Benhaim, Vishrav Chaudhary, Xia Song, and Furu Wei. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - Longllmlingua: Accelerating and enhancing llms in long context scenarios via prompt compression.
    [pdf](https://aclanthology.org/2024.acl-long.91.pdf)
    - Huiqiang Jiang, Qianhui Wu, Xufang Luo, Dongsheng Li, Chin-Yew Lin, Yuqing Yang, and Lili Qiu. *arXiv preprint arXiv:2310.06839 2023*

 - Adapting Language Models to Compress Contexts.
    [pdf](https://arxiv.org/pdf/2305.14788)
    - Alexis Chevalier, Alexander Wettig, Anirudh Ajith, and Danqi Chen. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - SLOG: A Structural Generalization Benchmark for Semantic Parsing.
    [pdf](https://aclanthology.org/2023.emnlp-main.194.pdf)
    - Bingzhi Li, Lucia Donatelli, Alexander Koller, Tal Linzen, Yuekun Yao, and Najoung Kim. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Lost in the Middle: How Language Models Use Long Contexts.
    [pdf](https://arxiv.org/pdf/2307.03172)
    - Nelson F Liu, Kevin Lin, John Hewitt, Ashwin Paranjape, Michele Bevilacqua, Fabio Petroni, and Percy Liang. *Transactions of the Association for Computational Linguistics Transactions of the Association for Computational Linguistics*

 - Train Short, Test Long: Attention with Linear Biases Enables Input Length Extrapolation.
    [pdf](https://arxiv.org/pdf/2108.12409)
    - Ofir Press, Noah Smith, and Mike Lewis. *International Conference on Learning Representations 2022*

 - A Length-Extrapolatable Transformer.
    [pdf](https://arxiv.org/pdf/2212.10554)
    - Yutao Sun, Li Dong, Barun Patra, Shuming Ma, Shaohan Huang, Alon Benhaim, Vishrav Chaudhary, Xia Song, and Furu Wei. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - Roformer: Enhanced transformer with rotary position embedding.
    [pdf](https://arxiv.org/pdf/2104.09864)
    - Jianlin Su, Murtadha Ahmed, Yu Lu, Shengfeng Pan, Wen Bo, and Yunfeng Liu. *Neurocomputing 2024*

 - Functional Interpolation for Relative Positions improves Long Context Transformers.
    [pdf](https://openreview.net/pdf?id=rR03qFesqk)
    - Shanda Li, Chong You, Guru Guruganesh, Joshua Ainslie, Santiago Ontanon, Manzil Zaheer, Sumit Sanghai, Yiming Yang, Sanjiv Kumar, and Srinadh Bhojanapalli. *The Twelfth International Conference on Learning Representations 2024*

 - Lost in the Middle: How Language Models Use Long Contexts.
    [pdf](https://arxiv.org/pdf/2307.03172)
    - Nelson F Liu, Kevin Lin, John Hewitt, Ashwin Paranjape, Michele Bevilacqua, Fabio Petroni, and Percy Liang. *Transactions of the Association for Computational Linguistics Transactions of the Association for Computational Linguistics*

 - Found in the Middle: Calibrating Positional Attention Bias Improves Long Context Utilization.
    [pdf](https://arxiv.org/pdf/2406.16008)
    - Cheng-Yu Hsieh, Yung-Sung Chuang, Chun-Liang Li, Zifeng Wang, Long T Le, Abhishek Kumar, James Glass, Alexander Ratner, Chen-Yu Lee, Ranjay Krishna, and others. *arXiv preprint arXiv:2406.16008 2024*

 - Found in the Middle: Calibrating Positional Attention Bias Improves Long Context Utilization.
    [pdf](https://arxiv.org/pdf/2406.16008)
    - Cheng-Yu Hsieh, Yung-Sung Chuang, Chun-Liang Li, Zifeng Wang, Long T Le, Abhishek Kumar, James Glass, Alexander Ratner, Chen-Yu Lee, Ranjay Krishna, and others. *arXiv preprint arXiv:2406.16008 2024*

 - Make Your LLM Fully Utilize the Context.
    [pdf](https://arxiv.org/pdf/2404.16811)
    - Shengnan An, Zexiong Ma, Zeqi Lin, Nanning Zheng, and Jian-Guang Lou. *arXiv preprint arXiv:2404.16811 2024*

- Gpt-4 technical report.
  [pdf](https://arxiv.org/abs/2303.08774)
    - Josh Achiam, Steven Adler, Sandhini Agarwal, Lama Ahmad, Ilge Akkaya, Florencia Leoni Aleman, Diogo Almeida, Janko Altenschmidt, Sam Altman, Shyamal Anadkat, and others. *arXiv preprint arXiv:2303.08774 2023*

 - LongAgent: Scaling Language Models to 128k Context through Multi-Agent Collaboration.
    [pdf](https://arxiv.org/pdf/2402.11550)
    - Jun Zhao, Can Zu, Hao Xu, Yi Lu, Wei He, Yiwen Ding, Tao Gui, Qi Zhang, and Xuanjing Huang. *arXiv preprint arXiv:2402.11550 2024*

 - LongLoRA: Efficient Fine-tuning of Long-Context Large Language Models.
    [pdf](https://arxiv.org/pdf/2309.12307)
    - Yukang Chen, Shengju Qian, Haotian Tang, Xin Lai, Zhijian Liu, Song Han, and Jiaya Jia. *The Twelfth International Conference on Learning Representations 2024*

 - Longllmlingua: Accelerating and enhancing llms in long context scenarios via prompt compression.
    [pdf](https://aclanthology.org/2024.acl-long.91.pdf)
    - Huiqiang Jiang, Qianhui Wu, Xufang Luo, Dongsheng Li, Chin-Yew Lin, Yuqing Yang, and Lili Qiu. *arXiv preprint arXiv:2310.06839 2023*

 - Adapting Language Models to Compress Contexts.
    [pdf](https://arxiv.org/pdf/2305.14788)
    - Alexis Chevalier, Alexander Wettig, Anirudh Ajith, and Danqi Chen. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

### Attack and Defense
 - TrojLLM: A Black-box Trojan Prompt Attack on Large Language Models.
    [pdf](https://arxiv.org/pdf/2306.06815)
    - Jiaqi Xue, Mengxin Zheng, Ting Hua, Yilin Shen, Yepeng Liu, Ladislau Boloni, and Qian Lou. *Thirty-seventh Conference on Neural Information Processing Systems 2023*

 - Gama: Generative adversarial multi-object scene attacks.
    [pdf](https://arxiv.org/pdf/2209.09502)
    - Abhishek Aich, Calvin-Khang Ta, Akash Gupta, Chengyu Song, Srikanth Krishnamurthy, Salman Asif, and Amit Roy-Chowdhury. *Advances in Neural Information Processing Systems 2022*

 - Boosting Adversarial Transferability using Dynamic Cues.
    [pdf](https://arxiv.org/pdf/2302.12252)
    - Muzammal Naseer, Ahmad Mahmood, Salman Khan, and Fahad Khan. *The Eleventh International Conference on Learning Representations 2023*

 - Set-level guidance attack: Boosting adversarial transferability of vision-language pre-training models.
    [pdf](https://arxiv.org/pdf/2307.14061)
    - Dong Lu, Zhiqiang Wang, Teng Wang, Weili Guan, Hongchang Gao, and Feng Zheng. *Proceedings of the IEEE/CVF International Conference on Computer Vision 2023*

 - Jailbroken: How Does LLM Safety Training Fail?.
    [pdf](https://arxiv.org/pdf/2307.02483)
    - Alexander Wei, Nika Haghtalab, and Jacob Steinhardt. *Thirty-seventh Conference on Neural Information Processing Systems 2023*

 - Jailbreak in pieces: Compositional Adversarial Attacks on Multi-Modal Language Models.
    [pdf](https://arxiv.org/pdf/2307.14539)
    - Erfan Shayegani, Yue Dong, and Nael Abu-Ghazaleh. *The Twelfth International Conference on Learning Representations 2024*

 - ProPILE: Probing Privacy Leakage in Large Language Models.
    [pdf](https://arxiv.org/pdf/2307.01881)
    - Siwon Kim, Sangdoo Yun, Hwaran Lee, Martin Gubri, Sungroh Yoon, and Seong Joon Oh. *Thirty-seventh Conference on Neural Information Processing Systems 2023*

 - On Evaluating Adversarial Robustness of Large Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2305.16934)
    - Yunqing Zhao, Tianyu Pang, Chao Du, Xiao Yang, Chongxuan Li, Ngai-man Cheung, and Min Lin. *Thirty-seventh Conference on Neural Information Processing Systems 2023*

 - BadChain: Backdoor Chain-of-Thought Prompting for Large Language Models.
    [pdf](https://arxiv.org/pdf/2401.12242)
    - Zhen Xiang, Fengqing Jiang, Zidi Xiong, Bhaskar Ramasubramanian, Radha Poovendran, and Bo Li. *The Twelfth International Conference on Learning Representations 2024*

 - Data poisoning attacks against multimodal encoders.
    [pdf](https://arxiv.org/pdf/2209.15266)
    - Ziqing Yang, Xinlei He, Zheng Li, Michael Backes, Mathias Humbert, Pascal Berrang, and Yang Zhang. *International Conference on Machine Learning 2023*

 - Poisoning language models during instruction tuning.
    [pdf](https://arxiv.org/pdf/2305.00944)
    - Alexander Wan, Eric Wallace, Sheng Shen, and Dan Klein. *International Conference on Machine Learning 2023*

 - ProPILE: Probing Privacy Leakage in Large Language Models.
    [pdf](https://arxiv.org/pdf/2307.01881)
    - Siwon Kim, Sangdoo Yun, Hwaran Lee, Martin Gubri, Sungroh Yoon, and Seong Joon Oh. *Thirty-seventh Conference on Neural Information Processing Systems 2023*

 - TrojLLM: A Black-box Trojan Prompt Attack on Large Language Models.
    [pdf](https://arxiv.org/pdf/2306.06815)
    - Jiaqi Xue, Mengxin Zheng, Ting Hua, Yilin Shen, Yepeng Liu, Ladislau Boloni, and Qian Lou. *Thirty-seventh Conference on Neural Information Processing Systems 2023*

 - On Evaluating Adversarial Robustness of Large Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2305.16934)
    - Yunqing Zhao, Tianyu Pang, Chao Du, Xiao Yang, Chongxuan Li, Ngai-man Cheung, and Min Lin. *Thirty-seventh Conference on Neural Information Processing Systems 2023*

 - Gama: Generative adversarial multi-object scene attacks.
    [pdf](https://arxiv.org/pdf/2209.09502)
    - Abhishek Aich, Calvin-Khang Ta, Akash Gupta, Chengyu Song, Srikanth Krishnamurthy, Salman Asif, and Amit Roy-Chowdhury. *Advances in Neural Information Processing Systems 2022*

 - Boosting Adversarial Transferability using Dynamic Cues.
    [pdf](https://arxiv.org/pdf/2302.12252)
    - Muzammal Naseer, Ahmad Mahmood, Salman Khan, and Fahad Khan. *The Eleventh International Conference on Learning Representations 2023*

 - Jailbroken: How Does LLM Safety Training Fail?.
    [pdf](https://arxiv.org/pdf/2307.02483)
    - Alexander Wei, Nika Haghtalab, and Jacob Steinhardt. *Thirty-seventh Conference on Neural Information Processing Systems 2023*

 - Jailbreak in pieces: Compositional Adversarial Attacks on Multi-Modal Language Models.
    [pdf](https://arxiv.org/pdf/2307.14539)
    - Erfan Shayegani, Yue Dong, and Nael Abu-Ghazaleh. *The Twelfth International Conference on Learning Representations 2024*

 - Poisoning language models during instruction tuning.
    [pdf](https://arxiv.org/pdf/2305.00944)
    - Alexander Wan, Eric Wallace, Sheng Shen, and Dan Klein. *International Conference on Machine Learning 2023*

 - BadChain: Backdoor Chain-of-Thought Prompting for Large Language Models.
    [pdf](https://arxiv.org/pdf/2401.12242)
    - Zhen Xiang, Fengqing Jiang, Zidi Xiong, Bhaskar Ramasubramanian, Radha Poovendran, and Bo Li. *The Twelfth International Conference on Learning Representations 2024*

 - Data poisoning attacks against multimodal encoders.
    [pdf](https://arxiv.org/pdf/2209.15266)
    - Ziqing Yang, Xinlei He, Zheng Li, Michael Backes, Mathias Humbert, Pascal Berrang, and Yang Zhang. *International Conference on Machine Learning 2023*

 - Mathattack: Attacking large language models towards math solving ability.
    [pdf](https://arxiv.org/pdf/2309.01686)
    - Zihao Zhou, Qiufeng Wang, Mingyu Jin, Jie Yao, Jianan Ye, Wei Liu, Wei Wang, Xiaowei Huang, and Kaizhu Huang. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - VQAttack: Transferable Adversarial Attacks on Visual Question Answering via Pre-trained Models.
    [pdf](https://arxiv.org/pdf/2402.11083)
    - Ziyi Yin, Muchao Ye, Tianrong Zhang, Jiaqi Wang, Han Liu, Jinghui Chen, Ting Wang, and Fenglong Ma. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Visual adversarial examples jailbreak aligned large language models.
    [pdf](https://arxiv.org/pdf/2306.13213)
    - Xiangyu Qi, Kaixuan Huang, Ashwinee Panda, Peter Henderson, Mengdi Wang, and Prateek Mittal. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Codeattack: Code-based adversarial attacks for pre-trained programming language models.
    [pdf](https://arxiv.org/pdf/2206.00052)
    - Akshita Jha and Chandan K Reddy. *Proceedings of the AAAI Conference on Artificial Intelligence 2023*

 - Learn2weight: Parameter adaptation against similar-domain adversarial attacks.
    [pdf](https://arxiv.org/pdf/2205.07315)
    - Siddhartha Datta. *arXiv preprint arXiv:2205.07315 2022*

 - Enhance Robustness of Language Models Against Variation Attack through Graph Integration.
    [pdf](https://arxiv.org/pdf/2404.12014)
    - Zi Xiong, Lizhi Qing, Yangyang Kang, Jiawei Liu, Hongsong Li, Changlong Sun, Xiaozhong Liu, and Wei Lu. *arXiv preprint arXiv:2404.12014 2024*

 - Mathattack: Attacking large language models towards math solving ability.
    [pdf](https://arxiv.org/pdf/2309.01686)
    - Zihao Zhou, Qiufeng Wang, Mingyu Jin, Jie Yao, Jianan Ye, Wei Liu, Wei Wang, Xiaowei Huang, and Kaizhu Huang. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Codeattack: Code-based adversarial attacks for pre-trained programming language models.
    [pdf](https://arxiv.org/pdf/2206.00052)
    - Akshita Jha and Chandan K Reddy. *Proceedings of the AAAI Conference on Artificial Intelligence 2023*

 - Towards transferable adversarial attacks on vision transformers.
    [pdf](https://arxiv.org/pdf/2109.04176)
    - Zhipeng Wei, Jingjing Chen, Micah Goldblum, Zuxuan Wu, Tom Goldstein, and Yu-Gang Jiang. *Proceedings of the AAAI Conference on Artificial Intelligence 2022*

 - A context aware approach for generating natural language attacks.
    [pdf](https://arxiv.org/pdf/2012.13339v1)
    - Rishabh Maheshwary, Saket Maheshwary, and Vikram Pudi. *Proceedings of the AAAI conference on artificial intelligence 2021*

 - Learn2weight: Parameter adaptation against similar-domain adversarial attacks.
    [pdf](https://arxiv.org/pdf/2205.07315)
    - Siddhartha Datta. *arXiv preprint arXiv:2205.07315 2022*

 - Enhance Robustness of Language Models Against Variation Attack through Graph Integration.
    [pdf](https://arxiv.org/pdf/2404.12014)
    - Zi Xiong, Lizhi Qing, Yangyang Kang, Jiawei Liu, Hongsong Li, Changlong Sun, Xiaozhong Liu, and Wei Lu. *arXiv preprint arXiv:2404.12014 2024*

 - VQAttack: Transferable Adversarial Attacks on Visual Question Answering via Pre-trained Models.
    [pdf](https://arxiv.org/pdf/2402.11083)
    - Ziyi Yin, Muchao Ye, Tianrong Zhang, Jiaqi Wang, Han Liu, Jinghui Chen, Ting Wang, and Fenglong Ma. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Visual adversarial examples jailbreak aligned large language models.
    [pdf](https://arxiv.org/pdf/2306.13213)
    - Xiangyu Qi, Kaixuan Huang, Ashwinee Panda, Peter Henderson, Mengdi Wang, and Prateek Mittal. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Self-attention attribution: Interpreting information interactions inside transformer.
    [pdf](https://arxiv.org/pdf/2004.11207)
    - Yaru Hao, Li Dong, Furu Wei, and Ke Xu. *Proceedings of the AAAI Conference on Artificial Intelligence 2021*

 - Generating natural language attacks in a hard label black box setting.
    [pdf](https://arxiv.org/pdf/2012.14956)
    - Rishabh Maheshwary, Saket Maheshwary, and Vikram Pudi. *Proceedings of the AAAI Conference on Artificial Intelligence 2021*

 - One prompt word is enough to boost adversarial robustness for pre-trained vision-language models.
    [pdf](https://arxiv.org/pdf/2403.01849)
    - Lin Li, Haoyan Guan, Jianing Qiu, and Michael Spratling. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2024*

 - Flocks of Stochastic Parrots: Differentially Private Prompt Learning for Large Language Models.
    [pdf](https://arxiv.org/pdf/2305.15594)
    - Haonan Duan, Adam Dziedzic, Nicolas Papernot, and Franziska Boenisch. *Thirty-seventh Conference on Neural Information Processing Systems 2023*

 - TaiChi: Improving the Robustness of NLP Models by Seeking Common Ground While Reserving Differences.
    [pdf](https://aclanthology.org/2024.lrec-main.1351.pdf)
    - Huimin Chen, Chengyu Wang, Yanhao Wang, Cen Chen, and Yinggui Wang. *Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024) 2024*

 - ORTicket: Let One Robust BERT Ticket Transfer across Different Tasks.
    [pdf](https://aclanthology.org/2024.lrec-main.1096.pdf)
    - Yuhao Zhou, Wenxiang Chen, Rui Zheng, Zhiheng Xi, Tao Gui, Qi Zhang, and Xuan-Jing Huang. *Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024) 2024*

 - Causality Based Front-door Defense Against Backdoor Attack on Language Models.
    [pdf](https://openreview.net/pdf?id=dmHHVcHFdM)
    - Yiran Liu, Xiaoang Xu, Zhiyi Hou, and Yang Yu. *Forty-first International Conference on Machine Learning 2024*

 - PAD: A Robustness Enhancement Ensemble Method via Promoting Attention Diversity.
    [pdf](https://aclanthology.org/2024.lrec-main.1100.pdf)
    - Yuting Yang, Pei Huang, Feifei Ma, Juan Cao, and Jintao Li. *Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024) 2024*

 - Learn2weight: Parameter adaptation against similar-domain adversarial attacks.
    [pdf](https://arxiv.org/pdf/2205.07315)
    - Siddhartha Datta. *arXiv preprint arXiv:2205.07315 2022*

 - Plugat: A plug and play module to defend against textual adversarial attack.
    [pdf](https://aclanthology.org/2022.coling-1.253.pdf)
    - Rui Zheng, Rong Bao, Qin Liu, Tao Gui, Qi Zhang, Xuan-Jing Huang, Rui Xie, and Wei Wu. *Proceedings of the 29th International Conference on Computational Linguistics 2022*

 - Unveiling the Implicit Toxicity in Large Language Models.
    [pdf](https://aclanthology.org/2023.emnlp-main.84.pdf)
    - Jiaxin Wen, Pei Ke, Hao Sun, Zhexin Zhang, Chengfei Li, Jinfeng Bai, and Minlie Huang. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Preserving privacy through dememorization: An unlearning technique for mitigating memorization risks in language models.
    [pdf](https://aclanthology.org/2023.emnlp-main.265.pdf)
    - Aly Kassem, Omar Mahmoud, and Sherif Saad. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

### Noise Decoding
 - Contrastive Decoding: Open-ended Text Generation as Optimization.
    [pdf](https://arxiv.org/pdf/2210.15097)
    - Xiang Lisa Li, Ari Holtzman, Daniel Fried, Percy Liang, Jason Eisner, Tatsunori Hashimoto, Luke Zettlemoyer, and Mike Lewis. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - RLCD: Reinforcement learning from contrastive distillation for LM alignment.
    [pdf](https://arxiv.org/pdf/2307.12950)
    - Kevin Yang, Dan Klein, Asli Celikyilmaz, Nanyun Peng, and Yuandong Tian. *The Twelfth International Conference on Learning Representations 2024*

 - Self-Destructing Models: Increasing the Costs of Harmful Dual Uses of Foundation Models.
    [pdf](https://arxiv.org/pdf/2211.14946)
    - Peter Henderson, Eric Mitchell, Christopher Manning, Dan Jurafsky, and Chelsea Finn. *Proceedings of the 2023 AAAI/ACM Conference on AI, Ethics, and Society 2023*

 - Speculative Decoding: Exploiting Speculative Execution for Accelerating Seq2seq Generation.
    [pdf](https://arxiv.org/pdf/2203.16487)
    - Heming Xia, Tao Ge, Peiyi Wang, Si-Qing Chen, Furu Wei, and Zhifang Sui. *Findings of the Association for Computational Linguistics: EMNLP 2023*

 - Lost in the Middle: How Language Models Use Long Contexts.
    [pdf](https://aclanthology.org/2024.tacl-1.9.pdf)
    - Nelson F. Liu, Kevin Lin, John Hewitt, Ashwin Paranjape, Michele Bevilacqua, Fabio Petroni, and Percy Liang. *Transactions of the Association for Computational Linguistics 2024*

 - Constitutional ai: Harmlessness from ai feedback.
    [pdf](https://scalingintelligence.stanford.edu/pubs/constitutionalai.pdf)
    - Yuntao Bai, Saurav Kadavath, Sandipan Kundu, Amanda Askell, Jackson Kernion, Andy Jones, Anna Chen, Anna Goldie, Azalia Mirhoseini, Cameron McKinnon, and others. *arXiv preprint arXiv:2212.08073 2022*

 - Self-consistency improves chain of thought reasoning in language models.
    [pdf](https://arxiv.org/pdf/2203.11171)
    - Xuezhi Wang, Jason Wei, Dale Schuurmans, Quoc Le, Ed Chi, Sharan Narang, Aakanksha Chowdhery, and Denny Zhou. *Unknown Venue 2023*

 - Reasoning with Language Model is Planning with World Model.
    [pdf](https://arxiv.org/pdf/2305.14992)
    - Shibo Hao, Yi Gu, Haodi Ma, Joshua Hong, Zhen Wang, Daisy Wang, and Zhiting Hu. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Rewoo: Decoupling reasoning from observations for efficient augmented language models.
    [pdf](https://arxiv.org/pdf/2305.18323)
    - Binfeng Xu, Zhiyuan Peng, Bowen Lei, Subhabrata Mukherjee, Yuchen Liu, and Dongkuan Xu. *arXiv preprint arXiv:2305.18323 2023*

 - Tree of thoughts: Deliberate problem solving with large language models.
    [pdf](https://arxiv.org/pdf/2305.10601)
    - Shunyu Yao, Dian Yu, Jeffrey Zhao, Izhak Shafran, Tom Griffiths, Yuan Cao, and Karthik Narasimhan. *Advances in neural information processing systems 2023*

 - Self-rag: Learning to retrieve, generate, and critique through self-reflection.
    [pdf](https://arxiv.org/pdf/2310.11511)
    - Akari Asai, Zeqiu Wu, Yizhong Wang, Avirup Sil, and Hannaneh Hajishirzi. *The Twelfth International Conference on Learning Representations 2023*

 - ToRA: A Tool-Integrated Reasoning Agent for Mathematical Problem Solving.
    [pdf](https://openreview.net/pdf?id=Ep0TtjVoap)
    - Zhibin Gou, Zhihong Shao, Yeyun Gong, yelong shen, Yujiu Yang, Minlie Huang, Nan Duan, and Weizhu Chen. *The Twelfth International Conference on Learning Representations 2024*

 - Causality Based Front-door Defense Against Backdoor Attack on Language Models.
    [pdf](https://openreview.net/pdf?id=dmHHVcHFdM)
    - Yiran Liu, Xiaoang Xu, Zhiyi Hou, and Yang Yu. *Forty-first International Conference on Machine Learning 2024*

 - Causality for Large Language Models.
    [pdf](https://arxiv.org/pdf/2410.15319)
    - Anpeng Wu, Kun Kuang, Minqin Zhu, Yingrong Wang, Yujia Zheng, Kairong Han, Baohong Li, Guangyi Chen, Fei Wu, and Kun Zhang. *CoRR 2024*

 - Bridging causal discovery and large language models: A comprehensive survey of integrative approaches and future directions.
    [pdf](https://arxiv.org/pdf/2402.11068v1)
    - Guangya Wan, Yuqi Wu, Mengxuan Hu, Zhixuan Chu, and Sheng Li. *arXiv preprint arXiv:2402.11068 2024*

 - Causality Based Front-door Defense Against Backdoor Attack on Language Models.
    [pdf](https://openreview.net/pdf?id=dmHHVcHFdM)
    - Yiran Liu, Xiaoang Xu, Zhiyi Hou, and Yang Yu. *Forty-first International Conference on Machine Learning 2024*

 - Causality for Large Language Models.
    [pdf](https://arxiv.org/pdf/2410.15319)
    - Anpeng Wu, Kun Kuang, Minqin Zhu, Yingrong Wang, Yujia Zheng, Kairong Han, Baohong Li, Guangyi Chen, Fei Wu, and Kun Zhang. *CoRR 2024*

 - Bridging causal discovery and large language models: A comprehensive survey of integrative approaches and future directions.
    [pdf](https://arxiv.org/pdf/2402.11068v1)
    - Guangya Wan, Yuqi Wu, Mengxuan Hu, Zhixuan Chu, and Sheng Li. *arXiv preprint arXiv:2402.11068 2024*

<!-- begin comment 307 -->

 - Causality Based Front-door Defense Against Backdoor Attack on Language Models.
    [pdf](https://openreview.net/pdf?id=dmHHVcHFdM)
    - Yiran Liu, Xiaoang Xu, Zhiyi Hou, and Yang Yu. *Forty-first International Conference on Machine Learning 2024*

 - Causality for Large Language Models.
    [pdf](https://arxiv.org/pdf/2410.15319)
    - Anpeng Wu, Kun Kuang, Minqin Zhu, Yingrong Wang, Yujia Zheng, Kairong Han, Baohong Li, Guangyi Chen, Fei Wu, and Kun Zhang. *CoRR 2024*

 - Bridging causal discovery and large language models: A comprehensive survey of integrative approaches and future directions.
    [pdf](https://arxiv.org/pdf/2402.11068v1)
    - Guangya Wan, Yuqi Wu, Mengxuan Hu, Zhixuan Chu, and Sheng Li. *arXiv preprint arXiv:2402.11068 2024*

<!-- end comment 307 -->

<!-- begin comment 316 -->

 - Quantifying Language Models' Sensitivity to Spurious Features in Prompt Design or: How I learned to start worrying about prompt formatting.
    [pdf](https://arxiv.org/pdf/2310.11324)
    - Melanie Sclar, Yejin Choi, Yulia Tsvetkov, and Alane Suhr. *ICLR 2024*

 - Generating Novel Leads for Drug Discovery using LLMs with Logical Feedback.
    [pdf](https://www.biorxiv.org/content/10.1101/2023.09.14.557698v1.full.pdf)
    - Shreyas Bhat Brahmavar, Ashwin Srinivasan, Tirtharaj Dash, Sowmya Ramaswamy Krishnan, Lovekesh Vig, Arijit Roy, and Raviprasad Aduri. *AAAI 2024*

 - Generating Novel Leads for Drug Discovery using LLMs with Logical Feedback.
    [pdf](https://www.biorxiv.org/content/10.1101/2023.09.14.557698v1.full.pdf)
    - Shreyas Bhat Brahmavar, Ashwin Srinivasan, Tirtharaj Dash, Sowmya Ramaswamy Krishnan, Lovekesh Vig, Arijit Roy, and Raviprasad Aduri. *AAAI 2024*

- Towards robust in-context learning for machine translation with large language models.
  [pdf](https://aclanthology.org/2024.lrec-main.1444.pdf)
    - Shaolin Zhu, Menglong Cui, and Deyi Xiong. *LREC-COLING 2024*

- Combining Discourse Coherence with Large Language Models for More Inclusive, Equitable, and Robust Task-Oriented Dialogue.
  [pdf](https://aclanthology.org/2024.lrec-main.314.pdf)
    - Katherine Atwell, Mert Inan, Anthony B Sicilia, and Malihe Alikhani. *LREC-COLING 2024*

- Evaluating the Zero-shot Robustness of Instruction-tuned Language Models.
  [pdf](https://arxiv.org/pdf/2306.11270)
    - Jiuding Sun, Chantal Shaib, and Byron C Wallace. *The Twelfth International Conference on Learning Representations 2024*

- Towards robust in-context learning for machine translation with large language models.
  [pdf](https://aclanthology.org/2024.lrec-main.1444.pdf)
    - Shaolin Zhu, Menglong Cui, and Deyi Xiong. *LREC-COLING 2024*

- “was it “stated” or was it “claimed”?: How linguistic bias affects generative language models.
  [pdf](https://aclanthology.org/2021.emnlp-main.790.pdf)
    - Roma Patel and Ellie Pavlick. *EMNLP 2021*

- Detecting Cybercrimes in Accordance with Pakistani Law: Dataset and Evaluation Using PLMs.
  [pdf](https://aclanthology.org/2024.lrec-main.422.pdf)
    - Faizad Ullah, Ali Faheem, Ubaid Azam, Muhammad Sohaib Ayub, Faisal Kamiran, and Asim Karim. *Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024) 2024*

 - Generating Novel Leads for Drug Discovery using LLMs with Logical Feedback.
    [pdf](https://www.biorxiv.org/content/10.1101/2023.09.14.557698v1.full.pdf)
    - Shreyas Bhat Brahmavar, Ashwin Srinivasan, Tirtharaj Dash, Sowmya Ramaswamy Krishnan, Lovekesh Vig, Arijit Roy, and Raviprasad Aduri. *AAAI 2024*

 - On Second Thought, Let’s Not Think Step by Step! Bias and Toxicity in Zero-Shot Reasoning.
    [pdf](https://aclanthology.org/2023.acl-long.244.pdf)
    - Omar Shaikh, Hongxin Zhang, William Held, Michael Bernstein, and Diyi Yang. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

- InterFair: Debiasing with Natural Language Feedback for Fair Interpretable Predictions.
  [pdf](https://arxiv.org/pdf/2210.07440)
    - Bodhisattwa Prasad Majumder, Zexue He, and Julian McAuley. *arXiv e-prints 2022*

- Correcting Language Model Bias for Text Classification in True Zero-Shot Learning.
  [pdf](https://aclanthology.org/2024.lrec-main.359.pdf)
    - Feng Zhao, Wan Xianlin, Cheng Yan, and Chu Kiong Loo. *LREC-COLING 2024*

- Projective Methods for Mitigating Gender Bias in Pre-trained Language Models.
  [pdf](https://arxiv.org/pdf/2403.18803)
    - Hillary Dawkins, Isar Nejadgholi, Daniel Gillis, and Judi McCuaig. *arXiv:2403.18803 2024*

- Identifying and mitigating spurious correlations for improving robustness in nlp models.
  [pdf](https://aclanthology.org/2022.findings-naacl.130.pdf)
    - Tianlu Wang, Rohit Sridhar, Diyi Yang, and Xuezhi Wang. *arXiv preprint arXiv:2110.07736 2021*

- Measuring Inductive Biases of In-Context Learning with Underspecified Demonstrations.
  [pdf](https://aclanthology.org/2023.acl-long.632.pdf)
    - Chenglei Si, Dan Friedman, Nitish Joshi, Shi Feng, Danqi Chen, and He He. *Unknown Venue 2023*

- Mitigating Label Biases for In-context Learning.
  [pdf](https://arxiv.org/pdf/2305.19148)
    - Yu Fei, Yifan Hou, Zeming Chen, and Antoine Bosselut. *ACL 2023*

<!-- end comment 354 -->

<!-- begin comment 368 -->

 - Generating Novel Leads for Drug Discovery using LLMs with Logical Feedback.
    [pdf](https://www.biorxiv.org/content/10.1101/2023.09.14.557698v1.full.pdf)
    - Shreyas Bhat Brahmavar, Ashwin Srinivasan, Tirtharaj Dash, Sowmya Ramaswamy Krishnan, Lovekesh Vig, Arijit Roy, and Raviprasad Aduri. *AAAI 2024*

- Combining Discourse Coherence with Large Language Models for More Inclusive, Equitable, and Robust Task-Oriented Dialogue.
  [pdf](https://aclanthology.org/2024.lrec-main.314.pdf)
    - Katherine Atwell, Mert Inan, Anthony B Sicilia, and Malihe Alikhani. *LREC-COLING 2024*

- Towards robust in-context learning for machine translation with large language models.
  [pdf](https://aclanthology.org/2024.lrec-main.1444.pdf)
    - Shaolin Zhu, Menglong Cui, and Deyi Xiong. *LREC-COLING 2024*

- Correcting Language Model Bias for Text Classification in True Zero-Shot Learning.
  [pdf](https://aclanthology.org/2024.lrec-main.359.pdf)
    - Feng Zhao, Wan Xianlin, Cheng Yan, and Chu Kiong Loo. *LREC-COLING 2024*

- Projective Methods for Mitigating Gender Bias in Pre-trained Language Models.
  [pdf](https://arxiv.org/pdf/2403.18803)
    - Hillary Dawkins, Isar Nejadgholi, Daniel Gillis, and Judi McCuaig. *arXiv:2403.18803 2024*

- Detecting Cybercrimes in Accordance with Pakistani Law: Dataset and Evaluation Using PLMs.
  [pdf](https://aclanthology.org/2024.lrec-main.422.pdf)
    - Faizad Ullah, Ali Faheem, Ubaid Azam, Muhammad Sohaib Ayub, Faisal Kamiran, and Asim Karim. *Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024) 2024*

 - Evaluating Prompting Strategies for Grammatical Error Correction Based on Language Proficiency.
    [pdf](https://arxiv.org/pdf/2402.15930)
    - Min Zeng, Jiexin Kuang, Mengyang Qiu, Jayoung Song, and Jungyeul Park. *arXiv preprint arXiv:2402.15930 2024*

- Identifying and mitigating spurious correlations for improving robustness in nlp models.
  [pdf](https://aclanthology.org/2022.findings-naacl.130.pdf)
    - Tianlu Wang, Rohit Sridhar, Diyi Yang, and Xuezhi Wang. *arXiv preprint arXiv:2110.07736 2021*

- “was it “stated” or was it “claimed”?: How linguistic bias affects generative language models.
  [pdf](https://aclanthology.org/2021.emnlp-main.790.pdf)
    - Roma Patel and Ellie Pavlick. *EMNLP 2021*

- Measuring Inductive Biases of In-Context Learning with Underspecified Demonstrations.
  [pdf](https://aclanthology.org/2023.acl-long.632.pdf)
    - Chenglei Si, Dan Friedman, Nitish Joshi, Shi Feng, Danqi Chen, and He He. *Unknown Venue 2023*

- Mitigating Label Biases for In-context Learning.
  [pdf](https://arxiv.org/pdf/2305.19148)
    - Yu Fei, Yifan Hou, Zeming Chen, and Antoine Bosselut. *ACL 2023*

 - Language models are few-shot learners.
    [pdf](https://arxiv.org/pdf/2005.14165)
    - Tom Brown, Benjamin Mann, Nick Ryder, Melanie Subbiah, Jared D Kaplan, Prafulla Dhariwal, Arvind Neelakantan, Pranav Shyam, Girish Sastry, Amanda Askell, and others. *Advances in neural information processing systems 2020*

 - On Second Thought, Let’s Not Think Step by Step! Bias and Toxicity in Zero-Shot Reasoning.
    [pdf](https://aclanthology.org/2023.acl-long.244.pdf)
    - Omar Shaikh, Hongxin Zhang, William Held, Michael Bernstein, and Diyi Yang. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

- InterFair: Debiasing with Natural Language Feedback for Fair Interpretable Predictions.
  [pdf](https://arxiv.org/pdf/2210.07440)
    - Bodhisattwa Prasad Majumder, Zexue He, and Julian McAuley. *arXiv e-prints 2022*

<!-- end comment 374 -->

<!-- begin comment 377 -->

 - Crosslingual Generalization through Multitask Finetuning.
    [pdf](https://aclanthology.org/2023.acl-long.891.pdf)
    - Niklas Muennighoff, Thomas Wang, Lintang Sutawika, Adam Roberts, Stella Biderman, Teven Le Scao, M Saiful Bari, Sheng Shen, Zheng Xin Yong, Hailey Schoelkopf, and others. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - Revisiting non-English Text Simplification: A Unified Multilingual Benchmark.
    [pdf](https://arxiv.org/pdf/2305.15678)
    - Michael Ryan, Tarek Naous, and Wei Xu. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - Language Model Tokenizers Introduce Unfairness Between Languages.
    [pdf](https://arxiv.org/pdf/2305.15425)
    - Aleksandar Petrov, Emanuele La Malfa, Philip Torr, and Adel Bibi. *Thirty-seventh Conference on Neural Information Processing Systems 2023*

 - Gendered Grammar or Ingrained Bias? Exploring Gender Bias in Icelandic Language Models.
    [pdf](https://aclanthology.org/2024.lrec-main.671.pdf)
    - Steinunn Rut Fri and Hafsteinn Einarsson. *Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024) 2024*

<!-- end comment 390 -->

<!-- begin comment 392 -->

 - Language Model Tokenizers Introduce Unfairness Between Languages.
    [pdf](https://arxiv.org/pdf/2305.15425)
    - Aleksandar Petrov, Emanuele La Malfa, Philip Torr, and Adel Bibi. *Thirty-seventh Conference on Neural Information Processing Systems 2023*

 - Gendered Grammar or Ingrained Bias? Exploring Gender Bias in Icelandic Language Models.
    [pdf](https://aclanthology.org/2024.lrec-main.671.pdf)
    - Steinunn Rut Fri and Hafsteinn Einarsson. *Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024) 2024*

 - Crosslingual Generalization through Multitask Finetuning.
    [pdf](https://aclanthology.org/2023.acl-long.891.pdf)
    - Niklas Muennighoff, Thomas Wang, Lintang Sutawika, Adam Roberts, Stella Biderman, Teven Le Scao, M Saiful Bari, Sheng Shen, Zheng Xin Yong, Hailey Schoelkopf, and others. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - Revisiting non-English Text Simplification: A Unified Multilingual Benchmark.
    [pdf](https://arxiv.org/pdf/2305.15678)
    - Michael Ryan, Tarek Naous, and Wei Xu. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - Benchmarking Large Language Model Capabilities for Conditional Generation.
    [pdf](https://arxiv.org/pdf/2306.16793)
    - Joshua Maynez, Priyanka Agrawal, and Sebastian Gehrmann. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - Stitching Segments and Sentences towards Generalization in Video-Text Pre-training.
    [pdf](https://ojs.aaai.org/index.php/AAAI/article/view/28202)
    - Fan Ma, Xiaojie Jin, Heng Wang, Jingjia Huang, Linchao Zhu, and Yi Yang. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Do Androids Laugh at Electric Sheep? Humor “Understanding” Benchmarks from The New Yorker Caption Contest.
    [pdf](https://arxiv.org/pdf/2209.06293)
    - Jack Hessel and Ana Marasović. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

<!-- end comment 411 -->

### Causal Inspired Methods
<!-- begin comment 477 -->

 - TrojLLM: A Black-box Trojan Prompt Attack on Large Language Models.
    [pdf](https://arxiv.org/pdf/2306.06815)
    - Jiaqi Xue, Mengxin Zheng, Ting Hua, Yilin Shen, Yepeng Liu, Ladislau Boloni, and Qian Lou. *Thirty-seventh Conference on Neural Information Processing Systems 2023*

 - Gama: Generative adversarial multi-object scene attacks.
    [pdf](https://arxiv.org/pdf/2209.09502)
    - Abhishek Aich, Calvin-Khang Ta, Akash Gupta, Chengyu Song, Srikanth Krishnamurthy, Salman Asif, and Amit Roy-Chowdhury. *Advances in Neural Information Processing Systems 2022*

 - Boosting Adversarial Transferability using Dynamic Cues.
    [pdf](https://arxiv.org/pdf/2302.12252)
    - Muzammal Naseer, Ahmad Mahmood, Salman Khan, and Fahad Khan. *The Eleventh International Conference on Learning Representations 2023*

 - Set-level guidance attack: Boosting adversarial transferability of vision-language pre-training models.
    [pdf](https://arxiv.org/pdf/2307.14061)
    - Dong Lu, Zhiqiang Wang, Teng Wang, Weili Guan, Hongchang Gao, and Feng Zheng. *Proceedings of the IEEE/CVF International Conference on Computer Vision 2023*

 - Jailbroken: How Does LLM Safety Training Fail?.
    [pdf](https://arxiv.org/pdf/2307.02483)
    - Alexander Wei, Nika Haghtalab, and Jacob Steinhardt. *Thirty-seventh Conference on Neural Information Processing Systems 2023*

 - Jailbreak in pieces: Compositional Adversarial Attacks on Multi-Modal Language Models.
    [pdf](https://arxiv.org/pdf/2307.14539)
    - Erfan Shayegani, Yue Dong, and Nael Abu-Ghazaleh. *The Twelfth International Conference on Learning Representations 2024*

 - ProPILE: Probing Privacy Leakage in Large Language Models.
    [pdf](https://arxiv.org/pdf/2307.01881)
    - Siwon Kim, Sangdoo Yun, Hwaran Lee, Martin Gubri, Sungroh Yoon, and Seong Joon Oh. *Thirty-seventh Conference on Neural Information Processing Systems 2023*

 - On Evaluating Adversarial Robustness of Large Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2305.16934)
    - Yunqing Zhao, Tianyu Pang, Chao Du, Xiao Yang, Chongxuan Li, Ngai-man Cheung, and Min Lin. *Thirty-seventh Conference on Neural Information Processing Systems 2023*

 - BadChain: Backdoor Chain-of-Thought Prompting for Large Language Models.
    [pdf](https://arxiv.org/pdf/2401.12242)
    - Zhen Xiang, Fengqing Jiang, Zidi Xiong, Bhaskar Ramasubramanian, Radha Poovendran, and Bo Li. *The Twelfth International Conference on Learning Representations 2024*

 - Data poisoning attacks against multimodal encoders.
    [pdf](https://arxiv.org/pdf/2209.15266)
    - Ziqing Yang, Xinlei He, Zheng Li, Michael Backes, Mathias Humbert, Pascal Berrang, and Yang Zhang. *International Conference on Machine Learning 2023*

 - Poisoning language models during instruction tuning.
    [pdf](https://arxiv.org/pdf/2305.00944)
    - Alexander Wan, Eric Wallace, Sheng Shen, and Dan Klein. *International Conference on Machine Learning 2023*

 - ProPILE: Probing Privacy Leakage in Large Language Models.
    [pdf](https://arxiv.org/pdf/2307.01881)
    - Siwon Kim, Sangdoo Yun, Hwaran Lee, Martin Gubri, Sungroh Yoon, and Seong Joon Oh. *Thirty-seventh Conference on Neural Information Processing Systems 2023*

 - TrojLLM: A Black-box Trojan Prompt Attack on Large Language Models.
    [pdf](https://arxiv.org/pdf/2306.06815)
    - Jiaqi Xue, Mengxin Zheng, Ting Hua, Yilin Shen, Yepeng Liu, Ladislau Boloni, and Qian Lou. *Thirty-seventh Conference on Neural Information Processing Systems 2023*

 - On Evaluating Adversarial Robustness of Large Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2305.16934)
    - Yunqing Zhao, Tianyu Pang, Chao Du, Xiao Yang, Chongxuan Li, Ngai-man Cheung, and Min Lin. *Thirty-seventh Conference on Neural Information Processing Systems 2023*

 - Gama: Generative adversarial multi-object scene attacks.
    [pdf](https://arxiv.org/pdf/2209.09502)
    - Abhishek Aich, Calvin-Khang Ta, Akash Gupta, Chengyu Song, Srikanth Krishnamurthy, Salman Asif, and Amit Roy-Chowdhury. *Advances in Neural Information Processing Systems 2022*

 - Boosting Adversarial Transferability using Dynamic Cues.
    [pdf](https://arxiv.org/pdf/2302.12252)
    - Muzammal Naseer, Ahmad Mahmood, Salman Khan, and Fahad Khan. *The Eleventh International Conference on Learning Representations 2023*

 - Set-level guidance attack: Boosting adversarial transferability of vision-language pre-training models.
    [pdf](https://arxiv.org/pdf/2307.14061)
    - Dong Lu, Zhiqiang Wang, Teng Wang, Weili Guan, Hongchang Gao, and Feng Zheng. *Proceedings of the IEEE/CVF International Conference on Computer Vision 2023*

 - Jailbroken: How Does LLM Safety Training Fail?.
    [pdf](https://arxiv.org/pdf/2307.02483)
    - Alexander Wei, Nika Haghtalab, and Jacob Steinhardt. *Thirty-seventh Conference on Neural Information Processing Systems 2023*

 - Jailbreak in pieces: Compositional Adversarial Attacks on Multi-Modal Language Models.
    [pdf](https://arxiv.org/pdf/2307.14539)
    - Erfan Shayegani, Yue Dong, and Nael Abu-Ghazaleh. *The Twelfth International Conference on Learning Representations 2024*

 - Poisoning language models during instruction tuning.
    [pdf](https://arxiv.org/pdf/2305.00944)
    - Alexander Wan, Eric Wallace, Sheng Shen, and Dan Klein. *International Conference on Machine Learning 2023*

 - BadChain: Backdoor Chain-of-Thought Prompting for Large Language Models.
    [pdf](https://arxiv.org/pdf/2401.12242)
    - Zhen Xiang, Fengqing Jiang, Zidi Xiong, Bhaskar Ramasubramanian, Radha Poovendran, and Bo Li. *The Twelfth International Conference on Learning Representations 2024*

 - Data poisoning attacks against multimodal encoders.
    [pdf](https://arxiv.org/pdf/2209.15266)
    - Ziqing Yang, Xinlei He, Zheng Li, Michael Backes, Mathias Humbert, Pascal Berrang, and Yang Zhang. *International Conference on Machine Learning 2023*

 - One prompt word is enough to boost adversarial robustness for pre-trained vision-language models.
    [pdf](https://arxiv.org/pdf/2403.01849)
    - Lin Li, Haoyan Guan, Jianing Qiu, and Michael Spratling. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2024*

 - Flocks of Stochastic Parrots: Differentially Private Prompt Learning for Large Language Models.
    [pdf](https://arxiv.org/pdf/2305.15594)
    - Haonan Duan, Adam Dziedzic, Nicolas Papernot, and Franziska Boenisch. *Thirty-seventh Conference on Neural Information Processing Systems 2023*

 - VQAttack: Transferable Adversarial Attacks on Visual Question Answering via Pre-trained Models.
    [pdf](https://arxiv.org/pdf/2402.11083)
    - Ziyi Yin, Muchao Ye, Tianrong Zhang, Jiaqi Wang, Han Liu, Jinghui Chen, Ting Wang, and Fenglong Ma. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Visual adversarial examples jailbreak aligned large language models.
    [pdf](https://arxiv.org/pdf/2306.13213)
    - Xiangyu Qi, Kaixuan Huang, Ashwinee Panda, Peter Henderson, Mengdi Wang, and Prateek Mittal. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Mathattack: Attacking large language models towards math solving ability.
    [pdf](https://arxiv.org/pdf/2309.01686)
    - Zihao Zhou, Qiufeng Wang, Mingyu Jin, Jie Yao, Jianan Ye, Wei Liu, Wei Wang, Xiaowei Huang, and Kaizhu Huang. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Codeattack: Code-based adversarial attacks for pre-trained programming language models.
    [pdf](https://arxiv.org/pdf/2206.00052)
    - Akshita Jha and Chandan K Reddy. *Proceedings of the AAAI Conference on Artificial Intelligence 2023*

 - Towards transferable adversarial attacks on vision transformers.
    [pdf](https://arxiv.org/pdf/2109.04176)
    - Zhipeng Wei, Jingjing Chen, Micah Goldblum, Zuxuan Wu, Tom Goldstein, and Yu-Gang Jiang. *Proceedings of the AAAI Conference on Artificial Intelligence 2022*

 - Self-attention attribution: Interpreting information interactions inside transformer.
    [pdf](https://arxiv.org/pdf/2004.11207)
    - Yaru Hao, Li Dong, Furu Wei, and Ke Xu. *Proceedings of the AAAI Conference on Artificial Intelligence 2021*

 - Generating natural language attacks in a hard label black box setting.
    [pdf](https://arxiv.org/pdf/2012.14956)
    - Rishabh Maheshwary, Saket Maheshwary, and Vikram Pudi. *Proceedings of the AAAI Conference on Artificial Intelligence 2021*

 - A context aware approach for generating natural language attacks.
    [pdf](https://arxiv.org/pdf/2012.13339v1)
    - Rishabh Maheshwary, Saket Maheshwary, and Vikram Pudi. *Proceedings of the AAAI conference on artificial intelligence 2021*

 - Enhance Robustness of Language Models Against Variation Attack through Graph Integration.
    [pdf](https://arxiv.org/pdf/2404.12014)
    - Zi Xiong, Lizhi Qing, Yangyang Kang, Jiawei Liu, Hongsong Li, Changlong Sun, Xiaozhong Liu, and Wei Lu. *arXiv preprint arXiv:2404.12014 2024*

 - Learn2weight: Parameter adaptation against similar-domain adversarial attacks.
    [pdf](https://arxiv.org/pdf/2205.07315)
    - Siddhartha Datta. *arXiv preprint arXiv:2205.07315 2022*

 - ORTicket: Let One Robust BERT Ticket Transfer across Different Tasks.
    [pdf](https://aclanthology.org/2024.lrec-main.1096.pdf)
    - Yuhao Zhou, Wenxiang Chen, Rui Zheng, Zhiheng Xi, Tao Gui, Qi Zhang, and Xuan-Jing Huang. *Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024) 2024*

 - PAD: A Robustness Enhancement Ensemble Method via Promoting Attention Diversity.
    [pdf](https://aclanthology.org/2024.lrec-main.1100.pdf)
    - Yuting Yang, Pei Huang, Feifei Ma, Juan Cao, and Jintao Li. *Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024) 2024*

 - TaiChi: Improving the Robustness of NLP Models by Seeking Common Ground While Reserving Differences.
    [pdf](https://aclanthology.org/2024.lrec-main.1351.pdf)
    - Huimin Chen, Chengyu Wang, Yanhao Wang, Cen Chen, and Yinggui Wang. *Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024) 2024*

 - Plugat: A plug and play module to defend against textual adversarial attack.
    [pdf](https://aclanthology.org/2022.coling-1.253.pdf)
    - Rui Zheng, Rong Bao, Qin Liu, Tao Gui, Qi Zhang, Xuan-Jing Huang, Rui Xie, and Wei Wu. *Proceedings of the 29th International Conference on Computational Linguistics 2022*

 - Learn2weight: Parameter adaptation against similar-domain adversarial attacks.
    [pdf](https://arxiv.org/pdf/2205.07315)
    - Siddhartha Datta. *arXiv preprint arXiv:2205.07315 2022*

 - Is LLM-as-a-Judge Robust? Investigating Universal Adversarial Attacks on Zero-shot LLM Assessment.
    [pdf](https://aclanthology.org/2024.emnlp-main.427.pdf)
    - Vyas Raina, Adian Liusie, and Mark Gales. *arXiv preprint arXiv:2402.14016 2024*

 - Unveiling the Implicit Toxicity in Large Language Models.
    [pdf](https://aclanthology.org/2023.emnlp-main.84.pdf)
    - Jiaxin Wen, Pei Ke, Hao Sun, Zhexin Zhang, Chengfei Li, Jinfeng Bai, and Minlie Huang. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Preserving privacy through dememorization: An unlearning technique for mitigating memorization risks in language models.
    [pdf](https://aclanthology.org/2023.emnlp-main.265.pdf)
    - Aly Kassem, Omar Mahmoud, and Sherif Saad. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Privacy Implications of Retrieval-Based Language Models.
    [pdf](https://arxiv.org/pdf/2305.14888)
    - Yangsibo Huang, Samyak Gupta, Zexuan Zhong, Kai Li, and Danqi Chen. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

<!-- end comment 502 -->

## OOD Robustness
### Domain Transfer and Generalization
 - Cross-Task Generalization via Natural Language Crowdsourcing Instructions.
    [pdf](https://arxiv.org/pdf/2104.08773)
    - Swaroop Mishra, Daniel Khashabi, Chitta Baral, and Hannaneh Hajishirzi. *Proceedings of the 60th Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2022*

 - Active Instruction Tuning: Improving Cross-Task Generalization by Training on Prompt Sensitive Tasks.
    [pdf](https://arxiv.org/pdf/2311.00288)
    - Po-Nien Kung, Fan Yin, Di Wu, Kai-Wei Chang, and Nanyun Peng. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Towards Reliable Misinformation Mitigation: Generalization, Uncertainty, and GPT-4.
    [pdf](https://aclanthology.org/2023.emnlp-main.395.pdf)
    - Kellin Pelrine, Anne Imouza, Camille Thibault, Meilina Reksoprodjo, Caleb Gupta, Joel Christoph, Jean-Fran{}ois Godbout, and Reihaneh Rabbany. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - DiNeR: A Large Realistic Dataset for Evaluating Compositional Generalization.
    [pdf](https://aclanthology.org/2023.emnlp-main.924.pdf)
    - Chengang Hu, Xiao Liu, and Yansong Feng. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - SCITAB: A Challenging Benchmark for Compositional Reasoning and Claim Verification on Scientific Tables.
    [pdf](https://aclanthology.org/2023.emnlp-main.483.pdf)
    - Xinyuan Lu, Liangming Pan, Qian Liu, Preslav Nakov, and Min-Yen Kan. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - MedEval: A Multi-Level, Multi-Task, and Multi-Domain Medical Benchmark for Language Model Evaluation.
    [pdf](https://aclanthology.org/2023.emnlp-main.540.pdf)
    - Zexue He, Yu Wang, An Yan, Yao Liu, Eric Chang, Amilcare Gentili, Julian McAuley, and Chun-nan Hsu. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Cross-Task Generalization via Natural Language Crowdsourcing Instructions.
    [pdf](https://arxiv.org/pdf/2104.08773)
    - Swaroop Mishra, Daniel Khashabi, Chitta Baral, and Hannaneh Hajishirzi. *Proceedings of the 60th Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2022*

 - DiNeR: A Large Realistic Dataset for Evaluating Compositional Generalization.
    [pdf](https://aclanthology.org/2023.emnlp-main.924.pdf)
    - Chengang Hu, Xiao Liu, and Yansong Feng. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Geodesic multi-modal mixup for robust fine-tuning.
    [pdf](https://arxiv.org/pdf/2203.03897)
    - Changdae Oh, Junhyuk So, Hoyoon Byun, YongTaek Lim, Minchul Shin, Jong-June Jeon, and Kyungwoo Song. *Advances in Neural Information Processing Systems 2024*

 - Masked images are counterfactual samples for robust fine-tuning.
    [pdf](https://arxiv.org/pdf/2303.03052)
    - Yao Xiao, Ziyi Tang, Pengxu Wei, Cong Liu, and Liang Lin. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2023*

 - SCITAB: A Challenging Benchmark for Compositional Reasoning and Claim Verification on Scientific Tables.
    [pdf](https://aclanthology.org/2023.emnlp-main.483.pdf)
    - Xinyuan Lu, Liangming Pan, Qian Liu, Preslav Nakov, and Min-Yen Kan. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - MedEval: A Multi-Level, Multi-Task, and Multi-Domain Medical Benchmark for Language Model Evaluation.
    [pdf](https://aclanthology.org/2023.emnlp-main.540.pdf)
    - Zexue He, Yu Wang, An Yan, Yao Liu, Eric Chang, Amilcare Gentili, Julian McAuley, and Chun-nan Hsu. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Active Instruction Tuning: Improving Cross-Task Generalization by Training on Prompt Sensitive Tasks.
    [pdf](https://arxiv.org/pdf/2311.00288)
    - Po-Nien Kung, Fan Yin, Di Wu, Kai-Wei Chang, and Nanyun Peng. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Anchor-based Robust Finetuning of Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2404.06244)
    - Jinwei Han, Zhiwen Lin, Zhongyisun Sun, Yingguo Gao, Ke Yan, Shouhong Ding, Yuan Gao, and Gui-Song Xia. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2024*

 - Two-stage LLM Fine-tuning with Less Specialization and More Generalization.
    [pdf](https://openreview.net/pdf?id=pCEgna6Qco)
    - Yihan Wang, Si Si, Daliang Li, Michal Lukasik, Felix Yu, Cho-Jui Hsieh, Inderjit S Dhillon, and Sanjiv Kumar. *The Twelfth International Conference on Learning Representations 2024*

 - Surgical Fine-Tuning Improves Adaptation to Distribution Shifts.
    [pdf](https://arxiv.org/pdf/2210.11466)
    - Yoonho Lee, Annie S Chen, Fahim Tajwar, Ananya Kumar, Huaxiu Yao, Percy Liang, and Chelsea Finn. *The Eleventh International Conference on Learning Representations 2023*

 - Finetune like you pretrain: Improved finetuning of zero-shot vision models.
    [pdf](https://arxiv.org/pdf/2212.00638)
    - Sachin Goyal, Ananya Kumar, Sankalp Garg, Zico Kolter, and Aditi Raghunathan. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2023*

 - Mitigating spurious correlations in multi-modal models during fine-tuning.
    [pdf](https://arxiv.org/pdf/2304.03916)
    - Yu Yang, Besmira Nushi, Hamid Palangi, and Baharan Mirzasoleiman. *International Conference on Machine Learning 2023*

 - Masked images are counterfactual samples for robust fine-tuning.
    [pdf](https://arxiv.org/pdf/2303.03052)
    - Yao Xiao, Ziyi Tang, Pengxu Wei, Cong Liu, and Liang Lin. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2023*

 - Gradient-Regulated Meta-Prompt Learning for Generalizable Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2303.06571v2)
    - Juncheng Li, Minghe Gao, Longhui Wei, Siliang Tang, Wenqiao Zhang, Mengze Li, Wei Ji, Qi Tian, Tat-Seng Chua, and Yueting Zhuang. *Proceedings of the IEEE/CVF International Conference on Computer Vision (ICCV) 2023*

 - Active Instruction Tuning: Improving Cross-Task Generalization by Training on Prompt Sensitive Tasks.
    [pdf](https://arxiv.org/pdf/2311.00288)
    - Po-Nien Kung, Fan Yin, Di Wu, Kai-Wei Chang, and Nanyun Peng. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Towards Reliable Misinformation Mitigation: Generalization, Uncertainty, and GPT-4.
    [pdf](https://aclanthology.org/2023.emnlp-main.395.pdf)
    - Kellin Pelrine, Anne Imouza, Camille Thibault, Meilina Reksoprodjo, Caleb Gupta, Joel Christoph, Jean-Fran{}ois Godbout, and Reihaneh Rabbany. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Efficient equivariant transfer learning from pretrained models.
    [pdf](https://arxiv.org/pdf/2305.09900)
    - Sourya Basu, Pulkit Katdare, Prasanna Sattigeri, Vijil Chenthamarakshan, Katherine Driggs-Campbell, Payel Das, and Lav R Varshney. *Advances in Neural Information Processing Systems 2024*

 - Trainable projected gradient method for robust fine-tuning.
    [pdf](https://arxiv.org/pdf/2303.10720)
    - Junjiao Tian, Zecheng He, Xiaoliang Dai, Chih-Yao Ma, Yen-Cheng Liu, and Zsolt Kira. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2023*

<!-- begin table -->

 - Cross-Task Generalization via Natural Language Crowdsourcing Instructions.
    [pdf](https://arxiv.org/pdf/2104.08773)
    - Swaroop Mishra, Daniel Khashabi, Chitta Baral, and Hannaneh Hajishirzi. *Proceedings of the 60th Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2022*

 - DiNeR: A Large Realistic Dataset for Evaluating Compositional Generalization.
    [pdf](https://aclanthology.org/2023.emnlp-main.924.pdf)
    - Chengang Hu, Xiao Liu, and Yansong Feng. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Geodesic multi-modal mixup for robust fine-tuning.
    [pdf](https://arxiv.org/pdf/2203.03897)
    - Changdae Oh, Junhyuk So, Hoyoon Byun, YongTaek Lim, Minchul Shin, Jong-June Jeon, and Kyungwoo Song. *Advances in Neural Information Processing Systems 2024*

 - SCITAB: A Challenging Benchmark for Compositional Reasoning and Claim Verification on Scientific Tables.
    [pdf](https://aclanthology.org/2023.emnlp-main.483.pdf)
    - Xinyuan Lu, Liangming Pan, Qian Liu, Preslav Nakov, and Min-Yen Kan. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Masked images are counterfactual samples for robust fine-tuning.
    [pdf](https://arxiv.org/pdf/2303.03052)
    - Yao Xiao, Ziyi Tang, Pengxu Wei, Cong Liu, and Liang Lin. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2023*

 - Anchor-based Robust Finetuning of Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2404.06244)
    - Jinwei Han, Zhiwen Lin, Zhongyisun Sun, Yingguo Gao, Ke Yan, Shouhong Ding, Yuan Gao, and Gui-Song Xia. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2024*

 - Two-stage LLM Fine-tuning with Less Specialization and More Generalization.
    [pdf](https://openreview.net/pdf?id=pCEgna6Qco)
    - Yihan Wang, Si Si, Daliang Li, Michal Lukasik, Felix Yu, Cho-Jui Hsieh, Inderjit S Dhillon, and Sanjiv Kumar. *The Twelfth International Conference on Learning Representations 2024*

 - Surgical Fine-Tuning Improves Adaptation to Distribution Shifts.
    [pdf](https://arxiv.org/pdf/2210.11466)
    - Yoonho Lee, Annie S Chen, Fahim Tajwar, Ananya Kumar, Huaxiu Yao, Percy Liang, and Chelsea Finn. *The Eleventh International Conference on Learning Representations 2023*

 - Finetune like you pretrain: Improved finetuning of zero-shot vision models.
    [pdf](https://arxiv.org/pdf/2212.00638)
    - Sachin Goyal, Ananya Kumar, Sankalp Garg, Zico Kolter, and Aditi Raghunathan. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2023*

 - Trainable projected gradient method for robust fine-tuning.
    [pdf](https://arxiv.org/pdf/2303.10720)
    - Junjiao Tian, Zecheng He, Xiaoliang Dai, Chih-Yao Ma, Yen-Cheng Liu, and Zsolt Kira. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2023*

 - Efficient equivariant transfer learning from pretrained models.
    [pdf](https://arxiv.org/pdf/2305.09900)
    - Sourya Basu, Pulkit Katdare, Prasanna Sattigeri, Vijil Chenthamarakshan, Katherine Driggs-Campbell, Payel Das, and Lav R Varshney. *Advances in Neural Information Processing Systems 2024*

 - A Sentence Speaks a Thousand Images: Domain Generalization through Distilling CLIP with Language Guidance.
    [pdf](https://arxiv.org/pdf/2309.12530)
    - Zeyi Huang, Andy Zhou, Zijian Ling, Mu Cai, Haohan Wang, and Yong Jae Lee. *Proceedings of the IEEE/CVF International Conference on Computer Vision (ICCV) 2023*

 - PracticalDG: Perturbation Distillation on Vision-Language Models for Hybrid Domain Generalization.
    [pdf](https://arxiv.org/pdf/2404.09011)
    - Zining Chen, Weiqiu Wang, Zhicheng Zhao, Fei Su, Aidong Men, and Hongying Meng. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - Source-Free Domain Adaptation with Frozen Multimodal Foundation Model.
    [pdf](https://arxiv.org/pdf/2311.16510)
    - Song Tang, Wenxin Su, Mao Ye, and Xiatian Zhu. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - Dual Memory Networks: A Versatile Adaptation Approach for Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2403.17589)
    - Yabin Zhang, Wenjie Zhu, Hui Tang, Zhiyuan Ma, Kaiyang Zhou, and Lei Zhang. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - Overcoming the Pitfalls of Vision-Language Model Finetuning for OOD Generalization.
    [pdf](https://arxiv.org/pdf/2401.15914)
    - Yuhang Zang, Hanlin Goh, Joshua M. Susskind, and Chen Huang. *The Twelfth International Conference on Learning Representations 2024*

 - Leveraging Vision-Language Models for Improving Domain Generalization in Image Classification.
    [pdf](https://arxiv.org/pdf/2310.08255)
    - Sravanti Addepalli, Ashish Ramayee Asokan, Lakshay Sharma, and R Venkatesh Babu. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2024*

 - Negative Label Guided OOD Detection with Pretrained Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2403.20078)
    - Xue Jiang, Feng Liu, Zhen Fang, Hong Chen, Tongliang Liu, Feng Zheng, and Bo Han. *The Twelfth International Conference on Learning Representations 2024*

 - Unified out-of-distribution detection: A model-specific perspective.
    [pdf](https://arxiv.org/pdf/2304.06813)
    - Reza Averly and Wei-Lun Chao. *Proceedings of the IEEE/CVF International Conference on Computer Vision 2023*

 - SelfCheckGPT: Zero-Resource Black-Box Hallucination Detection for Generative Large Language Models.
    [pdf](https://arxiv.org/pdf/2303.08896)
    - Potsawee Manakul, Adian Liusie, and Mark Gales. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - How Good Are LLMs at Out-of-Distribution Detection?.
    [pdf](https://arxiv.org/pdf/2308.10261)
    - Bo Liu, Li-Ming Zhan, Zexin Lu, Yujie Feng, Lei Xue, and Xiao-Ming Wu. *Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024) 2024*

 - Enhancing Uncertainty-Based Hallucination Detection with Stronger Focus.
    [pdf](https://arxiv.org/pdf/2311.13230)
    - Tianhang Zhang, Lin Qiu, Qipeng Guo, Cheng Deng, Yue Zhang, Zheng Zhang, Chenghu Zhou, Xinbing Wang, and Luoyi Fu. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Why LLMs Hallucinate, and How to Get (Evidential) Closure: Perceptual, Intensional, and Extensional Learning for Faithful Natural Language Generation.
    [pdf](https://aclanthology.org/2023.emnlp-main.192.pdf)
    - Adam Bouyamourn. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Enhancing job recommendation through llm-based generative adversarial networks.
    [pdf](https://arxiv.org/pdf/2307.10747)
    - Yingpeng Du, Di Luo, Rui Yan, Xiaopei Wang, Hongzhi Liu, Hengshu Zhu, Yang Song, and Jie Zhang. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - How Do In-Context Examples Affect Compositional Generalization?.
    [pdf](https://aclanthology.org/2023.acl-long.618.pdf)
    - Shengnan An, Zeqi Lin, Qiang Fu, Bei Chen, Nanning Zheng, Jian-Guang Lou, and Dongmei Zhang. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - RoCoIns: Enhancing Robustness of Large Language Models through Code-Style Instructions.
    [pdf](https://arxiv.org/pdf/2402.16431)
    - Yuansen Zhang, Xiao Wang, Zhiheng Xi, Han Xia, Tao Gui, Qi Zhang, and Xuanjing Huang. *arXiv preprint arXiv:2402.16431 2024*

 - HINT: Hypernetwork Instruction Tuning for Efficient Zero-and Few-Shot Generalisation.
    [pdf](https://arxiv.org/pdf/2212.10315)
    - Hamish Ivison, Akshita Bhagia, Yizhong Wang, Hannaneh Hajishirzi, and Matthew E Peters. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - Augmentation-Adapted Retriever Improves Generalization of Language Models as Generic Plug-In.
    [pdf](https://arxiv.org/pdf/2305.17331)
    - Zichun Yu, Chenyan Xiong, Shi Yu, and Zhiyuan Liu. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - Multitask Prompted Training Enables Zero-Shot Task Generalization.
    [pdf](https://arxiv.org/pdf/2110.08207)
    - Victor Sanh, Albert Webson, Colin Raffel, Stephen Bach, Lintang Sutawika, Zaid Alyafeai, Antoine Chaffin, Arnaud Stiegler, Arun Raja, Manan Dey, M Saiful Bari, Canwen Xu, Urmish Thakker, Shanya Sharma Sharma, Eliza Szczechla, Taewoon Kim, Gunjan Chhablani, Nihal Nayak, Debajyoti Datta, Jonathan Chang, Mike Tian-Jian Jiang, Han Wang, Matteo Manica, Sheng Shen, Zheng Xin Yong, Harshit Pandey, Rachel Bawden, Thomas Wang, Trishala Neeraj, Jos Rozen, Abheesht Sharma, Andrea Santilli, Thibault Fevry, Jason Alan Fries, Ryan Teehan, Teven Le Scao, Stella Biderman, Leo Gao, Thomas Wolf, and Alexander M Rush. *International Conference on Learning Representations 2022*

 - Zero-Shot Robustification of Zero-Shot Models.
    [pdf](https://arxiv.org/pdf/2309.04344)
    - Dyah Adila, Changho Shin, Linrong Cai, and Frederic Sala. *The Twelfth International Conference on Learning Representations 2024*

 - Compositional Task Representations for Large Language Models.
    [pdf](https://openreview.net/pdf?id=6axIMJA7ME3)
    - NAN SHAO, Zefan Cai, Hanwei xu, Chonghua Liao, Yanan Zheng, and Zhilin Yang. *The Eleventh International Conference on Learning Representations 2023*

 - Language-Driven Anchors for Zero-Shot Adversarial Robustness.
    [pdf](https://arxiv.org/pdf/2301.13096)
    - Xiao Li, Wei Zhang, Yining Liu, Zhanhao Hu, Bo Zhang, and Xiaolin Hu. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - Pre-trained Model Guided Fine-Tuning for Zero-Shot Adversarial Robustness.
    [pdf](https://arxiv.org/pdf/2401.04350)
    - Sibo Wang, Jie Zhang, Zheng Yuan, and Shiguang Shan. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - Test-time prompt tuning for zero-shot generalization in vision-language models.
    [pdf](https://arxiv.org/pdf/2209.07511)
    - Manli Shu, Weili Nie, De-An Huang, Zhiding Yu, Tom Goldstein, Anima Anandkumar, and Chaowei Xiao. *Advances in Neural Information Processing Systems 2022*

 - Efficient Test-Time Adaptation of Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2403.18293)
    - Adilbek Karmanov, Dayan Guan, Shijian Lu, Abdulmotaleb El Saddik, and Eric Xing. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2024*

 - Align your prompts: Test-time prompting with distribution alignment for zero-shot generalization.
    [pdf](https://arxiv.org/pdf/2311.01459)
    - Jameel Abdul Samadh, Mohammad Hanan Gani, Noor Hussein, Muhammad Uzair Khattak, Muhammad Muzammal Naseer, Fahad Shahbaz Khan, and Salman H Khan. *Advances in Neural Information Processing Systems 2024*

 - Test-Time Adaptation with CLIP Reward for Zero-Shot Generalization in Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2305.18010)
    - Shuai Zhao, Xiaohan Wang, Linchao Zhu, and Yi Yang. *The Twelfth International Conference on Learning Representations 2024*

 - On the Test-Time Zero-Shot Generalization of Vision-Language Models: Do We Really Need Prompt Learning?.
    [pdf](https://arxiv.org/pdf/2405.02266)
    - Maxime Zanella and Ismail Ben Ayed. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - Direct preference optimization: your language model is secretly a reward model.
    [pdf](https://arxiv.org/pdf/2305.18290)
    - Rafael Rafailov, Archit Sharma, Eric Mitchell, Stefano Ermon, Christopher D Manning, and Chelsea Finn. *Proceedings of the 37th International Conference on Neural Information Processing Systems 2023*

 - DRESS: Instructing Large Vision-Language Models to Align and Interact with Humans via Natural Language Feedback.
    [pdf](https://arxiv.org/pdf/2311.10081)
    - Yangyi Chen, Karan Sikka, Michael Cogswell, Heng Ji, and Ajay Divakaran. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - Pretraining language models with human preferences.
    [pdf](https://arxiv.org/pdf/2302.08582)
    - Tomasz Korbak, Kejian Shi, Angelica Chen, Rasika Vinayak Bhalerao, Christopher Buckley, Jason Phang, Samuel R Bowman, and Ethan Perez. *International Conference on Machine Learning 2023*

 - Inverse-RLignment: Inverse Reinforcement Learning from Demonstrations for LLM Alignment.
    [pdf](https://openreview.net/pdf?id=BrUxhfVepA)
    - Hao Sun and Mihaela van der Schaar. *arXiv preprint arXiv:2405.15624 2024*

 - Aligning as Debiasing: Causality-Aware Alignment via Reinforcement Learning with Interventional Feedback.
    [pdf](https://aclanthology.org/2024.naacl-long.262.pdf)
    - Yu Xia, Tong Yu, Zhankui He, Handong Zhao, Julian McAuley, and Shuai Li. *Proceedings of the 2024 Conference of the North American Chapter of the Association for Computational Linguistics: Human Language Technologies (Volume 1: Long Papers) 2024*

 - Moca: Measuring human-language model alignment on causal and moral judgment tasks.
    [pdf](https://arxiv.org/pdf/2310.19677)
    - Allen Nie, Yuhui Zhang, Atharva Shailesh Amdekar, Chris Piech, Tatsunori B Hashimoto, and Tobias Gerstenberg. *Advances in Neural Information Processing Systems 2024*

 - Optimizing Language Models for Human Preferences is a Causal Inference Problem.
    [pdf](https://arxiv.org/pdf/2402.14979)
    - Victoria Lin, Eli Ben-Michael, and Louis-Philippe Morency. *The 40th Conference on Uncertainty in Artificial Intelligence 2024*

 - On Robust Prefix-Tuning for Text Classification.
    [pdf](https://arxiv.org/pdf/2203.10378)
    - Zonghan Yang and Yang Liu. *International Conference on Learning Representations 2022*

 - Why Is Prompt Tuning for Vision-Language Models Robust to Noisy Labels?.
    [pdf](https://arxiv.org/pdf/2307.11978)
    - Cheng-En Wu, Yu Tian, Haichao Yu, Heng Wang, Pedro Morgado, Yu Hen Hu, and Linjie Yang. *Proceedings of the IEEE/CVF International Conference on Computer Vision (ICCV) 2023*

 - Understanding and Mitigating the Label Noise in Pre-training on Downstream Tasks.
    [pdf](https://arxiv.org/pdf/2309.17002)
    - Hao Chen, Jindong Wang, Ankit Shah, Ran Tao, Hongxin Wei, Xing Xie, Masashi Sugiyama, and Bhiksha Raj. *The Twelfth International Conference on Learning Representations 2024*

 - Large Language Models Can Be Strong Differentially Private Learners.
    [pdf](https://arxiv.org/pdf/2110.05679)
    - Xuechen Li, Florian Tramer, Percy Liang, and Tatsunori Hashimoto. *International Conference on Learning Representations 2022*

 - Fairness-aware structured pruning in transformers.
    [pdf](https://arxiv.org/pdf/2312.15398)
    - Abdelrahman Zayed, Gon{}alo Mordido, Samira Shabanian, Ioana Baldini, and Sarath Chandar. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Differentially Private Fine-tuning of Language Models.
    [pdf](https://arxiv.org/pdf/2110.06500)
    - Da Yu, Saurabh Naik, Arturs Backurs, Sivakanth Gopi, Huseyin A Inan, Gautam Kamath, Janardhan Kulkarni, Yin Tat Lee, Andre Manoel, Lukas Wutschitz, Sergey Yekhanin, and Huishuai Zhang. *International Conference on Learning Representations 2022*

 - Attention Satisfies: A Constraint-Satisfaction Lens on Factual Errors of Language Models.
    [pdf](https://arxiv.org/pdf/2309.15098)
    - Mert Yuksekgonul, Varun Chandrasekaran, Erik Jones, Suriya Gunasekar, Ranjita Naik, Hamid Palangi, Ece Kamar, and Besmira Nushi. *The Twelfth International Conference on Learning Representations 2024*

 - VISTA-LLAMA: Reducing Hallucination in Video Language Models via Equal Distance to Visual Tokens.
    [pdf](https://arxiv.org/pdf/2312.08870)
    - Fan Ma, Xiaojie Jin, Heng Wang, Yuchen Xian, Jiashi Feng, and Yi Yang. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - Mitigating Object Hallucinations in Large Vision-Language Models through Visual Contrastive Decoding.
    [pdf](https://arxiv.org/pdf/2311.16922)
    - Sicong Leng, Hang Zhang, Guanzheng Chen, Xin Li, Shijian Lu, Chunyan Miao, and Lidong Bing. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - DoLa: Decoding by Contrasting Layers Improves Factuality in Large Language Models.
    [pdf](https://arxiv.org/pdf/2309.03883)
    - Yung-Sung Chuang, Yujia Xie, Hongyin Luo, Yoon Kim, James R. Glass, and Pengcheng He. *The Twelfth International Conference on Learning Representations 2024*

 - Ontofact: Unveiling fantastic fact-skeleton of llms via ontology-driven reinforcement learning.
    [pdf](https://openreview.net/pdf?id=Kl2RwSP6bS)
    - Ziyu Shang, Wenjun Ke, Nana Xiu, Peng Wang, Jiajun Liu, Yanhui Li, Zhizhao Luo, and Ke Ji. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Teaching Language Models to Hallucinate Less with Synthetic Tasks.
    [pdf](https://arxiv.org/pdf/2310.06827)
    - Erik Jones, Hamid Palangi, Clarisse Simoes Ribeiro, Varun Chandrasekaran, Subhabrata Mukherjee, Arindam Mitra, Ahmed Hassan Awadallah, and Ece Kamar. *The Twelfth International Conference on Learning Representations 2024*

 - Mitigating large language model hallucinations via autonomous knowledge graph-based retrofitting.
    [pdf](https://arxiv.org/pdf/2311.13314)
    - Xinyan Guan, Yanjiang Liu, Hongyu Lin, Yaojie Lu, Ben He, Xianpei Han, and Le Sun. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - A Cause-Effect Look at Alleviating Hallucination of Knowledge-grounded Dialogue Generation.
    [pdf](https://arxiv.org/pdf/2404.03491)
    - Jifan Yu, Xiaohan Zhang, Yifan Xu, Xuanyu Lei, Zijun Yao, Jing Zhang, Lei Hou, and Juanzi Li. *arXiv preprint arXiv:2404.03491 2024*

 - Causal-debias: Unifying debiasing in pretrained language models and fine-tuning via causal invariant learning.
    [pdf](https://aclanthology.org/2023.acl-long.232.pdf)
    - Fan Zhou, Yuzhou Mao, Liu Yu, Yi Yang, and Ting Zhong. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

<!-- end table -->

 - A Sentence Speaks a Thousand Images: Domain Generalization through Distilling CLIP with Language Guidance.
    [pdf](https://arxiv.org/pdf/2309.12530)
    - Zeyi Huang, Andy Zhou, Zijian Ling, Mu Cai, Haohan Wang, and Yong Jae Lee. *Proceedings of the IEEE/CVF International Conference on Computer Vision (ICCV) 2023*

 - PracticalDG: Perturbation Distillation on Vision-Language Models for Hybrid Domain Generalization.
    [pdf](https://arxiv.org/pdf/2404.09011)
    - Zining Chen, Weiqiu Wang, Zhicheng Zhao, Fei Su, Aidong Men, and Hongying Meng. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - Source-Free Domain Adaptation with Frozen Multimodal Foundation Model.
    [pdf](https://arxiv.org/pdf/2311.16510)
    - Song Tang, Wenxin Su, Mao Ye, and Xiatian Zhu. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - Fine-Tuning can Distort Pretrained Features and Underperform Out-of-Distribution.
    [pdf](https://arxiv.org/pdf/2202.10054)
    - Ananya Kumar, Aditi Raghunathan, Robbie Matthew Jones, Tengyu Ma, and Percy Liang. *International Conference on Learning Representations 2022*

 - Clipood: Generalizing clip to out-of-distributions.
    [pdf](https://openreview.net/pdf?id=DTM83ccsMA)
    - Yang Shu, Xingzhuo Guo, Jialong Wu, Ximei Wang, Jianmin Wang, and Mingsheng Long. *International Conference on Machine Learning 2023*

 - A Closer Look at Model Adaptation using Feature Distortion and Simplicity Bias.
    [pdf](https://arxiv.org/pdf/2303.13500)
    - Puja Trivedi, Danai Koutra, and Jayaraman J. Thiagarajan. *The Eleventh International Conference on Learning Representations 2023*

 - Dual Memory Networks: A Versatile Adaptation Approach for Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2403.17589)
    - Yabin Zhang, Wenjie Zhu, Hui Tang, Zhiyuan Ma, Kaiyang Zhou, and Lei Zhang. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - Overcoming the Pitfalls of Vision-Language Model Finetuning for OOD Generalization.
    [pdf](https://arxiv.org/pdf/2401.15914)
    - Yuhang Zang, Hanlin Goh, Joshua M. Susskind, and Chen Huang. *The Twelfth International Conference on Learning Representations 2024*

 - Leveraging Vision-Language Models for Improving Domain Generalization in Image Classification.
    [pdf](https://arxiv.org/pdf/2310.08255)
    - Sravanti Addepalli, Ashish Ramayee Asokan, Lakshay Sharma, and R Venkatesh Babu. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2024*

 - Cross-Task Generalization via Natural Language Crowdsourcing Instructions.
    [pdf](https://arxiv.org/pdf/2104.08773)
    - Swaroop Mishra, Daniel Khashabi, Chitta Baral, and Hannaneh Hajishirzi. *Proceedings of the 60th Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2022*

 - DiNeR: A Large Realistic Dataset for Evaluating Compositional Generalization.
    [pdf](https://aclanthology.org/2023.emnlp-main.924.pdf)
    - Chengang Hu, Xiao Liu, and Yansong Feng. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Geodesic multi-modal mixup for robust fine-tuning.
    [pdf](https://arxiv.org/pdf/2203.03897)
    - Changdae Oh, Junhyuk So, Hoyoon Byun, YongTaek Lim, Minchul Shin, Jong-June Jeon, and Kyungwoo Song. *Advances in Neural Information Processing Systems 2024*

 - Masked images are counterfactual samples for robust fine-tuning.
    [pdf](https://arxiv.org/pdf/2303.03052)
    - Yao Xiao, Ziyi Tang, Pengxu Wei, Cong Liu, and Liang Lin. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2023*

 - SCITAB: A Challenging Benchmark for Compositional Reasoning and Claim Verification on Scientific Tables.
    [pdf](https://aclanthology.org/2023.emnlp-main.483.pdf)
    - Xinyuan Lu, Liangming Pan, Qian Liu, Preslav Nakov, and Min-Yen Kan. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - MedEval: A Multi-Level, Multi-Task, and Multi-Domain Medical Benchmark for Language Model Evaluation.
    [pdf](https://aclanthology.org/2023.emnlp-main.540.pdf)
    - Zexue He, Yu Wang, An Yan, Yao Liu, Eric Chang, Amilcare Gentili, Julian McAuley, and Chun-nan Hsu. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Active Instruction Tuning: Improving Cross-Task Generalization by Training on Prompt Sensitive Tasks.
    [pdf](https://arxiv.org/pdf/2311.00288)
    - Po-Nien Kung, Fan Yin, Di Wu, Kai-Wei Chang, and Nanyun Peng. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Evaluating the Impact of Model Scale for Compositional Generalization in Semantic Parsing.
    [pdf](https://aclanthology.org/2022.emnlp-main.624.pdf)
    - Linlu Qiu, Peter Shaw, Panupong Pasupat, Tianze Shi, Jonathan Herzig, Emily Pitler, Fei Sha, and Kristina Toutanova. *Proceedings of the 2022 Conference on Empirical Methods in Natural Language Processing 2022*

 - Active Instruction Tuning: Improving Cross-Task Generalization by Training on Prompt Sensitive Tasks.
    [pdf](https://arxiv.org/pdf/2311.00288)
    - Po-Nien Kung, Fan Yin, Di Wu, Kai-Wei Chang, and Nanyun Peng. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Towards Reliable Misinformation Mitigation: Generalization, Uncertainty, and GPT-4.
    [pdf](https://aclanthology.org/2023.emnlp-main.395.pdf)
    - Kellin Pelrine, Anne Imouza, Camille Thibault, Meilina Reksoprodjo, Caleb Gupta, Joel Christoph, Jean-Fran{}ois Godbout, and Reihaneh Rabbany. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Surgical Fine-Tuning Improves Adaptation to Distribution Shifts.
    [pdf](https://arxiv.org/pdf/2210.11466)
    - Yoonho Lee, Annie S Chen, Fahim Tajwar, Ananya Kumar, Huaxiu Yao, Percy Liang, and Chelsea Finn. *The Eleventh International Conference on Learning Representations 2023*

 - Two-stage LLM Fine-tuning with Less Specialization and More Generalization.
    [pdf](https://openreview.net/pdf?id=pCEgna6Qco)
    - Yihan Wang, Si Si, Daliang Li, Michal Lukasik, Felix Yu, Cho-Jui Hsieh, Inderjit S Dhillon, and Sanjiv Kumar. *The Twelfth International Conference on Learning Representations 2024*

 - Finetune like you pretrain: Improved finetuning of zero-shot vision models.
    [pdf](https://arxiv.org/pdf/2212.00638)
    - Sachin Goyal, Ananya Kumar, Sankalp Garg, Zico Kolter, and Aditi Raghunathan. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2023*

 - Trainable projected gradient method for robust fine-tuning.
    [pdf](https://arxiv.org/pdf/2303.10720)
    - Junjiao Tian, Zecheng He, Xiaoliang Dai, Chih-Yao Ma, Yen-Cheng Liu, and Zsolt Kira. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2023*

 - Mitigating spurious correlations in multi-modal models during fine-tuning.
    [pdf](https://arxiv.org/pdf/2304.03916)
    - Yu Yang, Besmira Nushi, Hamid Palangi, and Baharan Mirzasoleiman. *International Conference on Machine Learning 2023*

 - Geodesic multi-modal mixup for robust fine-tuning.
    [pdf](https://arxiv.org/pdf/2203.03897)
    - Changdae Oh, Junhyuk So, Hoyoon Byun, YongTaek Lim, Minchul Shin, Jong-June Jeon, and Kyungwoo Song. *Advances in Neural Information Processing Systems 2024*

 - Robust fine-tuning of zero-shot models.
    [pdf](https://arxiv.org/pdf/2109.01903)
    - Mitchell Wortsman, Gabriel Ilharco, Jong Wook Kim, Mike Li, Simon Kornblith, Rebecca Roelofs, Raphael Gontijo Lopes, Hannaneh Hajishirzi, Ali Farhadi, Hongseok Namkoong, and others. *Proceedings of the IEEE/CVF conference on computer vision and pattern recognition 2022*

 - Efficient equivariant transfer learning from pretrained models.
    [pdf](https://arxiv.org/pdf/2305.09900)
    - Sourya Basu, Pulkit Katdare, Prasanna Sattigeri, Vijil Chenthamarakshan, Katherine Driggs-Campbell, Payel Das, and Lav R Varshney. *Advances in Neural Information Processing Systems 2024*

 - Gradient-Regulated Meta-Prompt Learning for Generalizable Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2303.06571v2)
    - Juncheng Li, Minghe Gao, Longhui Wei, Siliang Tang, Wenqiao Zhang, Mengze Li, Wei Ji, Qi Tian, Tat-Seng Chua, and Yueting Zhuang. *Proceedings of the IEEE/CVF International Conference on Computer Vision (ICCV) 2023*

 - Mitigating spurious correlations in multi-modal models during fine-tuning.
    [pdf](https://arxiv.org/pdf/2304.03916)
    - Yu Yang, Besmira Nushi, Hamid Palangi, and Baharan Mirzasoleiman. *International Conference on Machine Learning 2023*

 - Masked images are counterfactual samples for robust fine-tuning.
    [pdf](https://arxiv.org/pdf/2303.03052)
    - Yao Xiao, Ziyi Tang, Pengxu Wei, Cong Liu, and Liang Lin. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2023*

 - Anchor-based Robust Finetuning of Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2404.06244)
    - Jinwei Han, Zhiwen Lin, Zhongyisun Sun, Yingguo Gao, Ke Yan, Shouhong Ding, Yuan Gao, and Gui-Song Xia. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2024*

 - PracticalDG: Perturbation Distillation on Vision-Language Models for Hybrid Domain Generalization.
    [pdf](https://arxiv.org/pdf/2404.09011)
    - Zining Chen, Weiqiu Wang, Zhicheng Zhao, Fei Su, Aidong Men, and Hongying Meng. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - Source-Free Domain Adaptation with Frozen Multimodal Foundation Model.
    [pdf](https://arxiv.org/pdf/2311.16510)
    - Song Tang, Wenxin Su, Mao Ye, and Xiatian Zhu. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - A Sentence Speaks a Thousand Images: Domain Generalization through Distilling CLIP with Language Guidance.
    [pdf](https://arxiv.org/pdf/2309.12530)
    - Zeyi Huang, Andy Zhou, Zijian Ling, Mu Cai, Haohan Wang, and Yong Jae Lee. *Proceedings of the IEEE/CVF International Conference on Computer Vision (ICCV) 2023*

 - Fine-Tuning can Distort Pretrained Features and Underperform Out-of-Distribution.
    [pdf](https://arxiv.org/pdf/2202.10054)
    - Ananya Kumar, Aditi Raghunathan, Robbie Matthew Jones, Tengyu Ma, and Percy Liang. *International Conference on Learning Representations 2022*

 - Clipood: Generalizing clip to out-of-distributions.
    [pdf](https://openreview.net/pdf?id=DTM83ccsMA)
    - Yang Shu, Xingzhuo Guo, Jialong Wu, Ximei Wang, Jianmin Wang, and Mingsheng Long. *International Conference on Machine Learning 2023*

 - A Closer Look at Model Adaptation using Feature Distortion and Simplicity Bias.
    [pdf](https://arxiv.org/pdf/2303.13500)
    - Puja Trivedi, Danai Koutra, and Jayaraman J. Thiagarajan. *The Eleventh International Conference on Learning Representations 2023*

 - Dual Memory Networks: A Versatile Adaptation Approach for Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2403.17589)
    - Yabin Zhang, Wenjie Zhu, Hui Tang, Zhiyuan Ma, Kaiyang Zhou, and Lei Zhang. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - Overcoming the Pitfalls of Vision-Language Model Finetuning for OOD Generalization.
    [pdf](https://arxiv.org/pdf/2401.15914)
    - Yuhang Zang, Hanlin Goh, Joshua M. Susskind, and Chen Huang. *The Twelfth International Conference on Learning Representations 2024*

 - Leveraging Vision-Language Models for Improving Domain Generalization in Image Classification.
    [pdf](https://arxiv.org/pdf/2310.08255)
    - Sravanti Addepalli, Ashish Ramayee Asokan, Lakshay Sharma, and R Venkatesh Babu. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2024*

### OOD Detection
 - Why LLMs Hallucinate, and How to Get (Evidential) Closure: Perceptual, Intensional, and Extensional Learning for Faithful Natural Language Generation.
    [pdf](https://aclanthology.org/2023.emnlp-main.192.pdf)
    - Adam Bouyamourn. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Fine-tuned LLMs Know More, Hallucinate Less with Few-Shot Sequence-to-Sequence Semantic Parsing over Wikidata.
    [pdf](https://aclanthology.org/2023.emnlp-main.353.pdf)
    - Silei Xu, Shicheng Liu, Theo Culhane, Elizaveta Pertseva, Meng-Hsi Wu, Sina Semnani, and Monica Lam. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - CRUSH4SQL: Collective Retrieval Using Schema Hallucination For Text2SQL.
    [pdf](https://arxiv.org/pdf/2311.01173)
    - Mayank Kothyari, Dhruva Dhingra, Sunita Sarawagi, and Soumen Chakrabarti. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Detecting and Mitigating Hallucinations in Multilingual Summarisation.
    [pdf](https://arxiv.org/pdf/2305.13632)
    - Yifu Qiu, Yftah Ziser, Anna Korhonen, Edoardo Ponti, and Shay B Cohen. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - SelfCheckGPT: Zero-Resource Black-Box Hallucination Detection for Generative Large Language Models.
    [pdf](https://arxiv.org/pdf/2303.08896)
    - Potsawee Manakul, Adian Liusie, and Mark Gales. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - How Good Are LLMs at Out-of-Distribution Detection?.
    [pdf](https://arxiv.org/pdf/2308.10261)
    - Bo Liu, Li-Ming Zhan, Zexin Lu, Yujie Feng, Lei Xue, and Xiao-Ming Wu. *Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024) 2024*

 - Negative Label Guided OOD Detection with Pretrained Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2403.20078)
    - Xue Jiang, Feng Liu, Zhen Fang, Hong Chen, Tongliang Liu, Feng Zheng, and Bo Han. *The Twelfth International Conference on Learning Representations 2024*

 - Unified out-of-distribution detection: A model-specific perspective.
    [pdf](https://arxiv.org/pdf/2304.06813)
    - Reza Averly and Wei-Lun Chao. *Proceedings of the IEEE/CVF International Conference on Computer Vision 2023*

 - Enhancing Uncertainty-Based Hallucination Detection with Stronger Focus.
    [pdf](https://arxiv.org/pdf/2311.13230)
    - Tianhang Zhang, Lin Qiu, Qipeng Guo, Cheng Deng, Yue Zhang, Zheng Zhang, Chenghu Zhou, Xinbing Wang, and Luoyi Fu. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - SelfCheckGPT: Zero-Resource Black-Box Hallucination Detection for Generative Large Language Models.
    [pdf](https://arxiv.org/pdf/2303.08896)
    - Potsawee Manakul, Adian Liusie, and Mark Gales. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Why LLMs Hallucinate, and How to Get (Evidential) Closure: Perceptual, Intensional, and Extensional Learning for Faithful Natural Language Generation.
    [pdf](https://aclanthology.org/2023.emnlp-main.192.pdf)
    - Adam Bouyamourn. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Fine-tuned LLMs Know More, Hallucinate Less with Few-Shot Sequence-to-Sequence Semantic Parsing over Wikidata.
    [pdf](https://aclanthology.org/2023.emnlp-main.353.pdf)
    - Silei Xu, Shicheng Liu, Theo Culhane, Elizaveta Pertseva, Meng-Hsi Wu, Sina Semnani, and Monica Lam. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - CRUSH4SQL: Collective Retrieval Using Schema Hallucination For Text2SQL.
    [pdf](https://arxiv.org/pdf/2311.01173)
    - Mayank Kothyari, Dhruva Dhingra, Sunita Sarawagi, and Soumen Chakrabarti. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Why LLMs Hallucinate, and How to Get (Evidential) Closure: Perceptual, Intensional, and Extensional Learning for Faithful Natural Language Generation.
    [pdf](https://aclanthology.org/2023.emnlp-main.192.pdf)
    - Adam Bouyamourn. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Fine-tuned LLMs Know More, Hallucinate Less with Few-Shot Sequence-to-Sequence Semantic Parsing over Wikidata.
    [pdf](https://aclanthology.org/2023.emnlp-main.353.pdf)
    - Silei Xu, Shicheng Liu, Theo Culhane, Elizaveta Pertseva, Meng-Hsi Wu, Sina Semnani, and Monica Lam. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - CRUSH4SQL: Collective Retrieval Using Schema Hallucination For Text2SQL.
    [pdf](https://arxiv.org/pdf/2311.01173)
    - Mayank Kothyari, Dhruva Dhingra, Sunita Sarawagi, and Soumen Chakrabarti. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Detecting and Mitigating Hallucinations in Multilingual Summarisation.
    [pdf](https://arxiv.org/pdf/2305.13632)
    - Yifu Qiu, Yftah Ziser, Anna Korhonen, Edoardo Ponti, and Shay B Cohen. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - SelfCheckGPT: Zero-Resource Black-Box Hallucination Detection for Generative Large Language Models.
    [pdf](https://arxiv.org/pdf/2303.08896)
    - Potsawee Manakul, Adian Liusie, and Mark Gales. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - How Good Are LLMs at Out-of-Distribution Detection?.
    [pdf](https://arxiv.org/pdf/2308.10261)
    - Bo Liu, Li-Ming Zhan, Zexin Lu, Yujie Feng, Lei Xue, and Xiao-Ming Wu. *Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024) 2024*

 - Negative Label Guided OOD Detection with Pretrained Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2403.20078)
    - Xue Jiang, Feng Liu, Zhen Fang, Hong Chen, Tongliang Liu, Feng Zheng, and Bo Han. *The Twelfth International Conference on Learning Representations 2024*

 - Unified out-of-distribution detection: A model-specific perspective.
    [pdf](https://arxiv.org/pdf/2304.06813)
    - Reza Averly and Wei-Lun Chao. *Proceedings of the IEEE/CVF International Conference on Computer Vision 2023*

 - Enhancing Uncertainty-Based Hallucination Detection with Stronger Focus.
    [pdf](https://arxiv.org/pdf/2311.13230)
    - Tianhang Zhang, Lin Qiu, Qipeng Guo, Cheng Deng, Yue Zhang, Zheng Zhang, Chenghu Zhou, Xinbing Wang, and Luoyi Fu. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - SelfCheckGPT: Zero-Resource Black-Box Hallucination Detection for Generative Large Language Models.
    [pdf](https://arxiv.org/pdf/2303.08896)
    - Potsawee Manakul, Adian Liusie, and Mark Gales. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Why LLMs Hallucinate, and How to Get (Evidential) Closure: Perceptual, Intensional, and Extensional Learning for Faithful Natural Language Generation.
    [pdf](https://aclanthology.org/2023.emnlp-main.192.pdf)
    - Adam Bouyamourn. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Fine-tuned LLMs Know More, Hallucinate Less with Few-Shot Sequence-to-Sequence Semantic Parsing over Wikidata.
    [pdf](https://aclanthology.org/2023.emnlp-main.353.pdf)
    - Silei Xu, Shicheng Liu, Theo Culhane, Elizaveta Pertseva, Meng-Hsi Wu, Sina Semnani, and Monica Lam. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - CRUSH4SQL: Collective Retrieval Using Schema Hallucination For Text2SQL.
    [pdf](https://arxiv.org/pdf/2311.01173)
    - Mayank Kothyari, Dhruva Dhingra, Sunita Sarawagi, and Soumen Chakrabarti. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Category-Extensible Out-of-Distribution Detection via Hierarchical Context Descriptions.
    [pdf](https://arxiv.org/pdf/2407.16725)
    - Kai Liu, Zhihang Fu, Chao Chen, Sheng Jin, Ze Chen, Mingyuan Tao, Rongxin Jiang, and Jieping Ye. *Thirty-seventh Conference on Neural Information Processing Systems 2023*

 - Negative Label Guided OOD Detection with Pretrained Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2403.20078)
    - Xue Jiang, Feng Liu, Zhen Fang, Hong Chen, Tongliang Liu, Feng Zheng, and Bo Han. *The Twelfth International Conference on Learning Representations 2024*

 - Unified out-of-distribution detection: A model-specific perspective.
    [pdf](https://arxiv.org/pdf/2304.06813)
    - Reza Averly and Wei-Lun Chao. *Proceedings of the IEEE/CVF International Conference on Computer Vision 2023*

 - How Good Are LLMs at Out-of-Distribution Detection?.
    [pdf](https://arxiv.org/pdf/2308.10261)
    - Bo Liu, Li-Ming Zhan, Zexin Lu, Yujie Feng, Lei Xue, and Xiao-Ming Wu. *Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024) 2024*

 - Enhancing Uncertainty-Based Hallucination Detection with Stronger Focus.
    [pdf](https://arxiv.org/pdf/2311.13230)
    - Tianhang Zhang, Lin Qiu, Qipeng Guo, Cheng Deng, Yue Zhang, Zheng Zhang, Chenghu Zhou, Xinbing Wang, and Luoyi Fu. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - The Troubling Emergence of Hallucination in Large Language Models-An Extensive Definition, Quantification, and Prescriptive Remediations.
    [pdf](https://aclanthology.org/2023.emnlp-main.155.pdf)
    - Vipula Rawte, Swagata Chakraborty, Agnibh Pathak, Anubhav Sarkar, SM Towhidul Islam Tonmoy, Aman Chadha, Amit Sheth, and Amitava Das. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Why LLMs Hallucinate, and How to Get (Evidential) Closure: Perceptual, Intensional, and Extensional Learning for Faithful Natural Language Generation.
    [pdf](https://aclanthology.org/2023.emnlp-main.192.pdf)
    - Adam Bouyamourn. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Fine-tuned LLMs Know More, Hallucinate Less with Few-Shot Sequence-to-Sequence Semantic Parsing over Wikidata.
    [pdf](https://aclanthology.org/2023.emnlp-main.353.pdf)
    - Silei Xu, Shicheng Liu, Theo Culhane, Elizaveta Pertseva, Meng-Hsi Wu, Sina Semnani, and Monica Lam. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - CRUSH4SQL: Collective Retrieval Using Schema Hallucination For Text2SQL.
    [pdf](https://arxiv.org/pdf/2311.01173)
    - Mayank Kothyari, Dhruva Dhingra, Sunita Sarawagi, and Soumen Chakrabarti. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Detecting and Mitigating Hallucinations in Multilingual Summarisation.
    [pdf](https://arxiv.org/pdf/2305.13632)
    - Yifu Qiu, Yftah Ziser, Anna Korhonen, Edoardo Ponti, and Shay B Cohen. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - SelfCheckGPT: Zero-Resource Black-Box Hallucination Detection for Generative Large Language Models.
    [pdf](https://arxiv.org/pdf/2303.08896)
    - Potsawee Manakul, Adian Liusie, and Mark Gales. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Enhancing Uncertainty-Based Hallucination Detection with Stronger Focus.
    [pdf](https://arxiv.org/pdf/2311.13230)
    - Tianhang Zhang, Lin Qiu, Qipeng Guo, Cheng Deng, Yue Zhang, Zheng Zhang, Chenghu Zhou, Xinbing Wang, and Luoyi Fu. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - SelfCheckGPT: Zero-Resource Black-Box Hallucination Detection for Generative Large Language Models.
    [pdf](https://arxiv.org/pdf/2303.08896)
    - Potsawee Manakul, Adian Liusie, and Mark Gales. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Enhancing Uncertainty-Based Hallucination Detection with Stronger Focus.
    [pdf](https://arxiv.org/pdf/2311.13230)
    - Tianhang Zhang, Lin Qiu, Qipeng Guo, Cheng Deng, Yue Zhang, Zheng Zhang, Chenghu Zhou, Xinbing Wang, and Luoyi Fu. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - SelfCheckGPT: Zero-Resource Black-Box Hallucination Detection for Generative Large Language Models.
    [pdf](https://arxiv.org/pdf/2303.08896)
    - Potsawee Manakul, Adian Liusie, and Mark Gales. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - The Troubling Emergence of Hallucination in Large Language Models-An Extensive Definition, Quantification, and Prescriptive Remediations.
    [pdf](https://aclanthology.org/2023.emnlp-main.155.pdf)
    - Vipula Rawte, Swagata Chakraborty, Agnibh Pathak, Anubhav Sarkar, SM Towhidul Islam Tonmoy, Aman Chadha, Amit Sheth, and Amitava Das. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Why LLMs Hallucinate, and How to Get (Evidential) Closure: Perceptual, Intensional, and Extensional Learning for Faithful Natural Language Generation.
    [pdf](https://aclanthology.org/2023.emnlp-main.192.pdf)
    - Adam Bouyamourn. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Fine-tuned LLMs Know More, Hallucinate Less with Few-Shot Sequence-to-Sequence Semantic Parsing over Wikidata.
    [pdf](https://aclanthology.org/2023.emnlp-main.353.pdf)
    - Silei Xu, Shicheng Liu, Theo Culhane, Elizaveta Pertseva, Meng-Hsi Wu, Sina Semnani, and Monica Lam. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - CRUSH4SQL: Collective Retrieval Using Schema Hallucination For Text2SQL.
    [pdf](https://arxiv.org/pdf/2311.01173)
    - Mayank Kothyari, Dhruva Dhingra, Sunita Sarawagi, and Soumen Chakrabarti. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Detecting and Mitigating Hallucinations in Multilingual Summarisation.
    [pdf](https://arxiv.org/pdf/2305.13632)
    - Yifu Qiu, Yftah Ziser, Anna Korhonen, Edoardo Ponti, and Shay B Cohen. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Cross-Task Generalization via Natural Language Crowdsourcing Instructions.
    [pdf](https://arxiv.org/pdf/2104.08773)
    - Swaroop Mishra, Daniel Khashabi, Chitta Baral, and Hannaneh Hajishirzi. *Proceedings of the 60th Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2022*

 - Active Instruction Tuning: Improving Cross-Task Generalization by Training on Prompt Sensitive Tasks.
    [pdf](https://arxiv.org/pdf/2311.00288)
    - Po-Nien Kung, Fan Yin, Di Wu, Kai-Wei Chang, and Nanyun Peng. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Towards Reliable Misinformation Mitigation: Generalization, Uncertainty, and GPT-4.
    [pdf](https://aclanthology.org/2023.emnlp-main.395.pdf)
    - Kellin Pelrine, Anne Imouza, Camille Thibault, Meilina Reksoprodjo, Caleb Gupta, Joel Christoph, Jean-Fran{}ois Godbout, and Reihaneh Rabbany. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - DiNeR: A Large Realistic Dataset for Evaluating Compositional Generalization.
    [pdf](https://aclanthology.org/2023.emnlp-main.924.pdf)
    - Chengang Hu, Xiao Liu, and Yansong Feng. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - SCITAB: A Challenging Benchmark for Compositional Reasoning and Claim Verification on Scientific Tables.
    [pdf](https://aclanthology.org/2023.emnlp-main.483.pdf)
    - Xinyuan Lu, Liangming Pan, Qian Liu, Preslav Nakov, and Min-Yen Kan. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - MedEval: A Multi-Level, Multi-Task, and Multi-Domain Medical Benchmark for Language Model Evaluation.
    [pdf](https://aclanthology.org/2023.emnlp-main.540.pdf)
    - Zexue He, Yu Wang, An Yan, Yao Liu, Eric Chang, Amilcare Gentili, Julian McAuley, and Chun-nan Hsu. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - On the Connection between Pre-training Data Diversity and Fine-tuning Robustness.
    [pdf](https://arxiv.org/pdf/2307.12532)
    - Vivek Ramanujan, Thao Nguyen, Sewoong Oh, Ali Farhadi, and Ludwig Schmidt. *Thirty-seventh Conference on Neural Information Processing Systems 2023*

 - Quality not quantity: On the interaction between dataset design and robustness of clip.
    [pdf](https://arxiv.org/pdf/2208.05516)
    - Thao Nguyen, Gabriel Ilharco, Mitchell Wortsman, Sewoong Oh, and Ludwig Schmidt. *Advances in Neural Information Processing Systems 2022*

 - Leveraging the inductive bias of large language models for abstract textual reasoning.
    [pdf](https://openreview.net/pdf?id=urueR03mkng)
    - Christopher Rytting and David Wingate. *Advances in Neural Information Processing Systems 2021*

 - Cross-Task Generalization via Natural Language Crowdsourcing Instructions.
    [pdf](https://arxiv.org/pdf/2104.08773)
    - Swaroop Mishra, Daniel Khashabi, Chitta Baral, and Hannaneh Hajishirzi. *Proceedings of the 60th Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2022*

 - DiNeR: A Large Realistic Dataset for Evaluating Compositional Generalization.
    [pdf](https://aclanthology.org/2023.emnlp-main.924.pdf)
    - Chengang Hu, Xiao Liu, and Yansong Feng. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Geodesic multi-modal mixup for robust fine-tuning.
    [pdf](https://arxiv.org/pdf/2203.03897)
    - Changdae Oh, Junhyuk So, Hoyoon Byun, YongTaek Lim, Minchul Shin, Jong-June Jeon, and Kyungwoo Song. *Advances in Neural Information Processing Systems 2024*

 - Masked images are counterfactual samples for robust fine-tuning.
    [pdf](https://arxiv.org/pdf/2303.03052)
    - Yao Xiao, Ziyi Tang, Pengxu Wei, Cong Liu, and Liang Lin. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2023*

 - SCITAB: A Challenging Benchmark for Compositional Reasoning and Claim Verification on Scientific Tables.
    [pdf](https://aclanthology.org/2023.emnlp-main.483.pdf)
    - Xinyuan Lu, Liangming Pan, Qian Liu, Preslav Nakov, and Min-Yen Kan. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - MedEval: A Multi-Level, Multi-Task, and Multi-Domain Medical Benchmark for Language Model Evaluation.
    [pdf](https://aclanthology.org/2023.emnlp-main.540.pdf)
    - Zexue He, Yu Wang, An Yan, Yao Liu, Eric Chang, Amilcare Gentili, Julian McAuley, and Chun-nan Hsu. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Active Instruction Tuning: Improving Cross-Task Generalization by Training on Prompt Sensitive Tasks.
    [pdf](https://arxiv.org/pdf/2311.00288)
    - Po-Nien Kung, Fan Yin, Di Wu, Kai-Wei Chang, and Nanyun Peng. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Evaluating the Impact of Model Scale for Compositional Generalization in Semantic Parsing.
    [pdf](https://aclanthology.org/2022.emnlp-main.624.pdf)
    - Linlu Qiu, Peter Shaw, Panupong Pasupat, Tianze Shi, Jonathan Herzig, Emily Pitler, Fei Sha, and Kristina Toutanova. *Proceedings of the 2022 Conference on Empirical Methods in Natural Language Processing 2022*

 - Active Instruction Tuning: Improving Cross-Task Generalization by Training on Prompt Sensitive Tasks.
    [pdf](https://arxiv.org/pdf/2311.00288)
    - Po-Nien Kung, Fan Yin, Di Wu, Kai-Wei Chang, and Nanyun Peng. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Towards Reliable Misinformation Mitigation: Generalization, Uncertainty, and GPT-4.
    [pdf](https://aclanthology.org/2023.emnlp-main.395.pdf)
    - Kellin Pelrine, Anne Imouza, Camille Thibault, Meilina Reksoprodjo, Caleb Gupta, Joel Christoph, Jean-Fran{}ois Godbout, and Reihaneh Rabbany. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Surgical Fine-Tuning Improves Adaptation to Distribution Shifts.
    [pdf](https://arxiv.org/pdf/2210.11466)
    - Yoonho Lee, Annie S Chen, Fahim Tajwar, Ananya Kumar, Huaxiu Yao, Percy Liang, and Chelsea Finn. *The Eleventh International Conference on Learning Representations 2023*

 - Two-stage LLM Fine-tuning with Less Specialization and More Generalization.
    [pdf](https://openreview.net/pdf?id=pCEgna6Qco)
    - Yihan Wang, Si Si, Daliang Li, Michal Lukasik, Felix Yu, Cho-Jui Hsieh, Inderjit S Dhillon, and Sanjiv Kumar. *The Twelfth International Conference on Learning Representations 2024*

 - Finetune like you pretrain: Improved finetuning of zero-shot vision models.
    [pdf](https://arxiv.org/pdf/2212.00638)
    - Sachin Goyal, Ananya Kumar, Sankalp Garg, Zico Kolter, and Aditi Raghunathan. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2023*

 - Trainable projected gradient method for robust fine-tuning.
    [pdf](https://arxiv.org/pdf/2303.10720)
    - Junjiao Tian, Zecheng He, Xiaoliang Dai, Chih-Yao Ma, Yen-Cheng Liu, and Zsolt Kira. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2023*

 - Mitigating spurious correlations in multi-modal models during fine-tuning.
    [pdf](https://arxiv.org/pdf/2304.03916)
    - Yu Yang, Besmira Nushi, Hamid Palangi, and Baharan Mirzasoleiman. *International Conference on Machine Learning 2023*

 - Geodesic multi-modal mixup for robust fine-tuning.
    [pdf](https://arxiv.org/pdf/2203.03897)
    - Changdae Oh, Junhyuk So, Hoyoon Byun, YongTaek Lim, Minchul Shin, Jong-June Jeon, and Kyungwoo Song. *Advances in Neural Information Processing Systems 2024*

 - Robust fine-tuning of zero-shot models.
    [pdf](https://arxiv.org/pdf/2109.01903)
    - Mitchell Wortsman, Gabriel Ilharco, Jong Wook Kim, Mike Li, Simon Kornblith, Rebecca Roelofs, Raphael Gontijo Lopes, Hannaneh Hajishirzi, Ali Farhadi, Hongseok Namkoong, and others. *Proceedings of the IEEE/CVF conference on computer vision and pattern recognition 2022*

 - Efficient equivariant transfer learning from pretrained models.
    [pdf](https://arxiv.org/pdf/2305.09900)
    - Sourya Basu, Pulkit Katdare, Prasanna Sattigeri, Vijil Chenthamarakshan, Katherine Driggs-Campbell, Payel Das, and Lav R Varshney. *Advances in Neural Information Processing Systems 2024*

 - Gradient-Regulated Meta-Prompt Learning for Generalizable Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2303.06571v2)
    - Juncheng Li, Minghe Gao, Longhui Wei, Siliang Tang, Wenqiao Zhang, Mengze Li, Wei Ji, Qi Tian, Tat-Seng Chua, and Yueting Zhuang. *Proceedings of the IEEE/CVF International Conference on Computer Vision (ICCV) 2023*

 - Mitigating spurious correlations in multi-modal models during fine-tuning.
    [pdf](https://arxiv.org/pdf/2304.03916)
    - Yu Yang, Besmira Nushi, Hamid Palangi, and Baharan Mirzasoleiman. *International Conference on Machine Learning 2023*

 - Masked images are counterfactual samples for robust fine-tuning.
    [pdf](https://arxiv.org/pdf/2303.03052)
    - Yao Xiao, Ziyi Tang, Pengxu Wei, Cong Liu, and Liang Lin. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2023*

 - Anchor-based Robust Finetuning of Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2404.06244)
    - Jinwei Han, Zhiwen Lin, Zhongyisun Sun, Yingguo Gao, Ke Yan, Shouhong Ding, Yuan Gao, and Gui-Song Xia. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2024*

 - PracticalDG: Perturbation Distillation on Vision-Language Models for Hybrid Domain Generalization.
    [pdf](https://arxiv.org/pdf/2404.09011)
    - Zining Chen, Weiqiu Wang, Zhicheng Zhao, Fei Su, Aidong Men, and Hongying Meng. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - Source-Free Domain Adaptation with Frozen Multimodal Foundation Model.
    [pdf](https://arxiv.org/pdf/2311.16510)
    - Song Tang, Wenxin Su, Mao Ye, and Xiatian Zhu. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - A Sentence Speaks a Thousand Images: Domain Generalization through Distilling CLIP with Language Guidance.
    [pdf](https://arxiv.org/pdf/2309.12530)
    - Zeyi Huang, Andy Zhou, Zijian Ling, Mu Cai, Haohan Wang, and Yong Jae Lee. *Proceedings of the IEEE/CVF International Conference on Computer Vision (ICCV) 2023*

 - Fine-Tuning can Distort Pretrained Features and Underperform Out-of-Distribution.
    [pdf](https://arxiv.org/pdf/2202.10054)
    - Ananya Kumar, Aditi Raghunathan, Robbie Matthew Jones, Tengyu Ma, and Percy Liang. *International Conference on Learning Representations 2022*

 - Clipood: Generalizing clip to out-of-distributions.
    [pdf](https://openreview.net/pdf?id=DTM83ccsMA)
    - Yang Shu, Xingzhuo Guo, Jialong Wu, Ximei Wang, Jianmin Wang, and Mingsheng Long. *International Conference on Machine Learning 2023*

 - A Closer Look at Model Adaptation using Feature Distortion and Simplicity Bias.
    [pdf](https://arxiv.org/pdf/2303.13500)
    - Puja Trivedi, Danai Koutra, and Jayaraman J. Thiagarajan. *The Eleventh International Conference on Learning Representations 2023*

 - Dual Memory Networks: A Versatile Adaptation Approach for Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2403.17589)
    - Yabin Zhang, Wenjie Zhu, Hui Tang, Zhiyuan Ma, Kaiyang Zhou, and Lei Zhang. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - Overcoming the Pitfalls of Vision-Language Model Finetuning for OOD Generalization.
    [pdf](https://arxiv.org/pdf/2401.15914)
    - Yuhang Zang, Hanlin Goh, Joshua M. Susskind, and Chen Huang. *The Twelfth International Conference on Learning Representations 2024*

 - Leveraging Vision-Language Models for Improving Domain Generalization in Image Classification.
    [pdf](https://arxiv.org/pdf/2310.08255)
    - Sravanti Addepalli, Ashish Ramayee Asokan, Lakshay Sharma, and R Venkatesh Babu. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2024*

 - Efficient equivariant transfer learning from pretrained models.
    [pdf](https://arxiv.org/pdf/2305.09900)
    - Sourya Basu, Pulkit Katdare, Prasanna Sattigeri, Vijil Chenthamarakshan, Katherine Driggs-Campbell, Payel Das, and Lav R Varshney. *Advances in Neural Information Processing Systems 2024*

 - PracticalDG: Perturbation Distillation on Vision-Language Models for Hybrid Domain Generalization.
    [pdf](https://arxiv.org/pdf/2404.09011)
    - Zining Chen, Weiqiu Wang, Zhicheng Zhao, Fei Su, Aidong Men, and Hongying Meng. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - Dual Memory Networks: A Versatile Adaptation Approach for Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2403.17589)
    - Yabin Zhang, Wenjie Zhu, Hui Tang, Zhiyuan Ma, Kaiyang Zhou, and Lei Zhang. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - Source-Free Domain Adaptation with Frozen Multimodal Foundation Model.
    [pdf](https://arxiv.org/pdf/2311.16510)
    - Song Tang, Wenxin Su, Mao Ye, and Xiatian Zhu. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - Gradient-Regulated Meta-Prompt Learning for Generalizable Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2303.06571v2)
    - Juncheng Li, Minghe Gao, Longhui Wei, Siliang Tang, Wenqiao Zhang, Mengze Li, Wei Ji, Qi Tian, Tat-Seng Chua, and Yueting Zhuang. *Proceedings of the IEEE/CVF International Conference on Computer Vision (ICCV) 2023*

 - A Sentence Speaks a Thousand Images: Domain Generalization through Distilling CLIP with Language Guidance.
    [pdf](https://arxiv.org/pdf/2309.12530)
    - Zeyi Huang, Andy Zhou, Zijian Ling, Mu Cai, Haohan Wang, and Yong Jae Lee. *Proceedings of the IEEE/CVF International Conference on Computer Vision (ICCV) 2023*

 - Cross-Task Generalization via Natural Language Crowdsourcing Instructions.
    [pdf](https://arxiv.org/pdf/2104.08773)
    - Swaroop Mishra, Daniel Khashabi, Chitta Baral, and Hannaneh Hajishirzi. *Proceedings of the 60th Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2022*

 - Active Instruction Tuning: Improving Cross-Task Generalization by Training on Prompt Sensitive Tasks.
    [pdf](https://arxiv.org/pdf/2311.00288)
    - Po-Nien Kung, Fan Yin, Di Wu, Kai-Wei Chang, and Nanyun Peng. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Towards Reliable Misinformation Mitigation: Generalization, Uncertainty, and GPT-4.
    [pdf](https://aclanthology.org/2023.emnlp-main.395.pdf)
    - Kellin Pelrine, Anne Imouza, Camille Thibault, Meilina Reksoprodjo, Caleb Gupta, Joel Christoph, Jean-Fran{}ois Godbout, and Reihaneh Rabbany. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - DiNeR: A Large Realistic Dataset for Evaluating Compositional Generalization.
    [pdf](https://aclanthology.org/2023.emnlp-main.924.pdf)
    - Chengang Hu, Xiao Liu, and Yansong Feng. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - SCITAB: A Challenging Benchmark for Compositional Reasoning and Claim Verification on Scientific Tables.
    [pdf](https://aclanthology.org/2023.emnlp-main.483.pdf)
    - Xinyuan Lu, Liangming Pan, Qian Liu, Preslav Nakov, and Min-Yen Kan. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - MedEval: A Multi-Level, Multi-Task, and Multi-Domain Medical Benchmark for Language Model Evaluation.
    [pdf](https://aclanthology.org/2023.emnlp-main.540.pdf)
    - Zexue He, Yu Wang, An Yan, Yao Liu, Eric Chang, Amilcare Gentili, Julian McAuley, and Chun-nan Hsu. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Cross-Task Generalization via Natural Language Crowdsourcing Instructions.
    [pdf](https://arxiv.org/pdf/2104.08773)
    - Swaroop Mishra, Daniel Khashabi, Chitta Baral, and Hannaneh Hajishirzi. *Proceedings of the 60th Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2022*

 - DiNeR: A Large Realistic Dataset for Evaluating Compositional Generalization.
    [pdf](https://aclanthology.org/2023.emnlp-main.924.pdf)
    - Chengang Hu, Xiao Liu, and Yansong Feng. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - SCITAB: A Challenging Benchmark for Compositional Reasoning and Claim Verification on Scientific Tables.
    [pdf](https://aclanthology.org/2023.emnlp-main.483.pdf)
    - Xinyuan Lu, Liangming Pan, Qian Liu, Preslav Nakov, and Min-Yen Kan. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - MedEval: A Multi-Level, Multi-Task, and Multi-Domain Medical Benchmark for Language Model Evaluation.
    [pdf](https://aclanthology.org/2023.emnlp-main.540.pdf)
    - Zexue He, Yu Wang, An Yan, Yao Liu, Eric Chang, Amilcare Gentili, Julian McAuley, and Chun-nan Hsu. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Active Instruction Tuning: Improving Cross-Task Generalization by Training on Prompt Sensitive Tasks.
    [pdf](https://arxiv.org/pdf/2311.00288)
    - Po-Nien Kung, Fan Yin, Di Wu, Kai-Wei Chang, and Nanyun Peng. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Towards Reliable Misinformation Mitigation: Generalization, Uncertainty, and GPT-4.
    [pdf](https://aclanthology.org/2023.emnlp-main.395.pdf)
    - Kellin Pelrine, Anne Imouza, Camille Thibault, Meilina Reksoprodjo, Caleb Gupta, Joel Christoph, Jean-Fran{}ois Godbout, and Reihaneh Rabbany. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

- Gpt-4 technical report.
  [pdf](https://arxiv.org/abs/2303.08774)
    - Josh Achiam, Steven Adler, Sandhini Agarwal, Lama Ahmad, Ilge Akkaya, Florencia Leoni Aleman, Diogo Almeida, Janko Altenschmidt, Sam Altman, Shyamal Anadkat, and others. *arXiv preprint arXiv:2303.08774 2023*

 - On the Connection between Pre-training Data Diversity and Fine-tuning Robustness.
    [pdf](https://arxiv.org/pdf/2307.12532)
    - Vivek Ramanujan, Thao Nguyen, Sewoong Oh, Ali Farhadi, and Ludwig Schmidt. *Thirty-seventh Conference on Neural Information Processing Systems 2023*

 - Quality not quantity: On the interaction between dataset design and robustness of clip.
    [pdf](https://arxiv.org/pdf/2208.05516)
    - Thao Nguyen, Gabriel Ilharco, Mitchell Wortsman, Sewoong Oh, and Ludwig Schmidt. *Advances in Neural Information Processing Systems 2022*

 - Leveraging the inductive bias of large language models for abstract textual reasoning.
    [pdf](https://openreview.net/pdf?id=urueR03mkng)
    - Christopher Rytting and David Wingate. *Advances in Neural Information Processing Systems 2021*

 - On the Connection between Pre-training Data Diversity and Fine-tuning Robustness.
    [pdf](https://arxiv.org/pdf/2307.12532)
    - Vivek Ramanujan, Thao Nguyen, Sewoong Oh, Ali Farhadi, and Ludwig Schmidt. *Thirty-seventh Conference on Neural Information Processing Systems 2023*

 - Quality not quantity: On the interaction between dataset design and robustness of clip.
    [pdf](https://arxiv.org/pdf/2208.05516)
    - Thao Nguyen, Gabriel Ilharco, Mitchell Wortsman, Sewoong Oh, and Ludwig Schmidt. *Advances in Neural Information Processing Systems 2022*

 - Leveraging the inductive bias of large language models for abstract textual reasoning.
    [pdf](https://openreview.net/pdf?id=urueR03mkng)
    - Christopher Rytting and David Wingate. *Advances in Neural Information Processing Systems 2021*

 - Overcoming the Pitfalls of Vision-Language Model Finetuning for OOD Generalization.
    [pdf](https://arxiv.org/pdf/2401.15914)
    - Yuhang Zang, Hanlin Goh, Joshua M. Susskind, and Chen Huang. *The Twelfth International Conference on Learning Representations 2024*

 - A Closer Look at Model Adaptation using Feature Distortion and Simplicity Bias.
    [pdf](https://arxiv.org/pdf/2303.13500)
    - Puja Trivedi, Danai Koutra, and Jayaraman J. Thiagarajan. *The Eleventh International Conference on Learning Representations 2023*

 - Surgical Fine-Tuning Improves Adaptation to Distribution Shifts.
    [pdf](https://arxiv.org/pdf/2210.11466)
    - Yoonho Lee, Annie S Chen, Fahim Tajwar, Ananya Kumar, Huaxiu Yao, Percy Liang, and Chelsea Finn. *The Eleventh International Conference on Learning Representations 2023*

 - Fine-Tuning can Distort Pretrained Features and Underperform Out-of-Distribution.
    [pdf](https://arxiv.org/pdf/2202.10054)
    - Ananya Kumar, Aditi Raghunathan, Robbie Matthew Jones, Tengyu Ma, and Percy Liang. *International Conference on Learning Representations 2022*

 - Anchor-based Robust Finetuning of Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2404.06244)
    - Jinwei Han, Zhiwen Lin, Zhongyisun Sun, Yingguo Gao, Ke Yan, Shouhong Ding, Yuan Gao, and Gui-Song Xia. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2024*

 - Finetune like you pretrain: Improved finetuning of zero-shot vision models.
    [pdf](https://arxiv.org/pdf/2212.00638)
    - Sachin Goyal, Ananya Kumar, Sankalp Garg, Zico Kolter, and Aditi Raghunathan. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2023*

 - Masked images are counterfactual samples for robust fine-tuning.
    [pdf](https://arxiv.org/pdf/2303.03052)
    - Yao Xiao, Ziyi Tang, Pengxu Wei, Cong Liu, and Liang Lin. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2023*

 - Trainable projected gradient method for robust fine-tuning.
    [pdf](https://arxiv.org/pdf/2303.10720)
    - Junjiao Tian, Zecheng He, Xiaoliang Dai, Chih-Yao Ma, Yen-Cheng Liu, and Zsolt Kira. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2023*

 - Robust fine-tuning of zero-shot models.
    [pdf](https://arxiv.org/pdf/2109.01903)
    - Mitchell Wortsman, Gabriel Ilharco, Jong Wook Kim, Mike Li, Simon Kornblith, Rebecca Roelofs, Raphael Gontijo Lopes, Hannaneh Hajishirzi, Ali Farhadi, Hongseok Namkoong, and others. *Proceedings of the IEEE/CVF conference on computer vision and pattern recognition 2022*

 - Geodesic multi-modal mixup for robust fine-tuning.
    [pdf](https://arxiv.org/pdf/2203.03897)
    - Changdae Oh, Junhyuk So, Hoyoon Byun, YongTaek Lim, Minchul Shin, Jong-June Jeon, and Kyungwoo Song. *Advances in Neural Information Processing Systems 2024*

 - Clipood: Generalizing clip to out-of-distributions.
    [pdf](https://openreview.net/pdf?id=DTM83ccsMA)
    - Yang Shu, Xingzhuo Guo, Jialong Wu, Ximei Wang, Jianmin Wang, and Mingsheng Long. *International Conference on Machine Learning 2023*

 - Mitigating spurious correlations in multi-modal models during fine-tuning.
    [pdf](https://arxiv.org/pdf/2304.03916)
    - Yu Yang, Besmira Nushi, Hamid Palangi, and Baharan Mirzasoleiman. *International Conference on Machine Learning 2023*

 - Two-stage LLM Fine-tuning with Less Specialization and More Generalization.
    [pdf](https://openreview.net/pdf?id=pCEgna6Qco)
    - Yihan Wang, Si Si, Daliang Li, Michal Lukasik, Felix Yu, Cho-Jui Hsieh, Inderjit S Dhillon, and Sanjiv Kumar. *The Twelfth International Conference on Learning Representations 2024*

 - Overcoming the Pitfalls of Vision-Language Model Finetuning for OOD Generalization.
    [pdf](https://arxiv.org/pdf/2401.15914)
    - Yuhang Zang, Hanlin Goh, Joshua M. Susskind, and Chen Huang. *The Twelfth International Conference on Learning Representations 2024*

 - A Closer Look at Model Adaptation using Feature Distortion and Simplicity Bias.
    [pdf](https://arxiv.org/pdf/2303.13500)
    - Puja Trivedi, Danai Koutra, and Jayaraman J. Thiagarajan. *The Eleventh International Conference on Learning Representations 2023*

 - Surgical Fine-Tuning Improves Adaptation to Distribution Shifts.
    [pdf](https://arxiv.org/pdf/2210.11466)
    - Yoonho Lee, Annie S Chen, Fahim Tajwar, Ananya Kumar, Huaxiu Yao, Percy Liang, and Chelsea Finn. *The Eleventh International Conference on Learning Representations 2023*

 - Fine-Tuning can Distort Pretrained Features and Underperform Out-of-Distribution.
    [pdf](https://arxiv.org/pdf/2202.10054)
    - Ananya Kumar, Aditi Raghunathan, Robbie Matthew Jones, Tengyu Ma, and Percy Liang. *International Conference on Learning Representations 2022*

 - Anchor-based Robust Finetuning of Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2404.06244)
    - Jinwei Han, Zhiwen Lin, Zhongyisun Sun, Yingguo Gao, Ke Yan, Shouhong Ding, Yuan Gao, and Gui-Song Xia. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2024*

 - Finetune like you pretrain: Improved finetuning of zero-shot vision models.
    [pdf](https://arxiv.org/pdf/2212.00638)
    - Sachin Goyal, Ananya Kumar, Sankalp Garg, Zico Kolter, and Aditi Raghunathan. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2023*

 - Masked images are counterfactual samples for robust fine-tuning.
    [pdf](https://arxiv.org/pdf/2303.03052)
    - Yao Xiao, Ziyi Tang, Pengxu Wei, Cong Liu, and Liang Lin. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2023*

 - Trainable projected gradient method for robust fine-tuning.
    [pdf](https://arxiv.org/pdf/2303.10720)
    - Junjiao Tian, Zecheng He, Xiaoliang Dai, Chih-Yao Ma, Yen-Cheng Liu, and Zsolt Kira. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2023*

 - Robust fine-tuning of zero-shot models.
    [pdf](https://arxiv.org/pdf/2109.01903)
    - Mitchell Wortsman, Gabriel Ilharco, Jong Wook Kim, Mike Li, Simon Kornblith, Rebecca Roelofs, Raphael Gontijo Lopes, Hannaneh Hajishirzi, Ali Farhadi, Hongseok Namkoong, and others. *Proceedings of the IEEE/CVF conference on computer vision and pattern recognition 2022*

 - Geodesic multi-modal mixup for robust fine-tuning.
    [pdf](https://arxiv.org/pdf/2203.03897)
    - Changdae Oh, Junhyuk So, Hoyoon Byun, YongTaek Lim, Minchul Shin, Jong-June Jeon, and Kyungwoo Song. *Advances in Neural Information Processing Systems 2024*

 - Clipood: Generalizing clip to out-of-distributions.
    [pdf](https://openreview.net/pdf?id=DTM83ccsMA)
    - Yang Shu, Xingzhuo Guo, Jialong Wu, Ximei Wang, Jianmin Wang, and Mingsheng Long. *International Conference on Machine Learning 2023*

 - Mitigating spurious correlations in multi-modal models during fine-tuning.
    [pdf](https://arxiv.org/pdf/2304.03916)
    - Yu Yang, Besmira Nushi, Hamid Palangi, and Baharan Mirzasoleiman. *International Conference on Machine Learning 2023*

 - Two-stage LLM Fine-tuning with Less Specialization and More Generalization.
    [pdf](https://openreview.net/pdf?id=pCEgna6Qco)
    - Yihan Wang, Si Si, Daliang Li, Michal Lukasik, Felix Yu, Cho-Jui Hsieh, Inderjit S Dhillon, and Sanjiv Kumar. *The Twelfth International Conference on Learning Representations 2024*

 - A comprehensive survey on test-time adaptation under distribution shifts.
    [pdf](https://arxiv.org/pdf/2303.15361)
    - Jian Liang, Ran He, and Tieniu Tan. *International Journal of Computer Vision 2024*

 - Adapting to Distribution Shift by Visual Domain Prompt Generation.
    [pdf](https://arxiv.org/pdf/2405.02797)
    - Zhixiang Chi, Li Gu, Tao Zhong, Huan Liu, YUANHAO YU, Konstantinos N Plataniotis, and Yang Wang. *The Twelfth International Conference on Learning Representations 2024*

 - Efficient Test-Time Adaptation of Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2403.18293)
    - Adilbek Karmanov, Dayan Guan, Shijian Lu, Abdulmotaleb El Saddik, and Eric Xing. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2024*

 - Adapting to Distribution Shift by Visual Domain Prompt Generation.
    [pdf](https://arxiv.org/pdf/2405.02797)
    - Zhixiang Chi, Li Gu, Tao Zhong, Huan Liu, YUANHAO YU, Konstantinos N Plataniotis, and Yang Wang. *The Twelfth International Conference on Learning Representations 2024*

 - Efficient Test-Time Adaptation of Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2403.18293)
    - Adilbek Karmanov, Dayan Guan, Shijian Lu, Abdulmotaleb El Saddik, and Eric Xing. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2024*

 - Adapting to Distribution Shift by Visual Domain Prompt Generation.
    [pdf](https://arxiv.org/pdf/2405.02797)
    - Zhixiang Chi, Li Gu, Tao Zhong, Huan Liu, YUANHAO YU, Konstantinos N Plataniotis, and Yang Wang. *The Twelfth International Conference on Learning Representations 2024*

 - Efficient Test-Time Adaptation of Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2403.18293)
    - Adilbek Karmanov, Dayan Guan, Shijian Lu, Abdulmotaleb El Saddik, and Eric Xing. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2024*

 - Leveraging Vision-Language Models for Improving Domain Generalization in Image Classification.
    [pdf](https://arxiv.org/pdf/2310.08255)
    - Sravanti Addepalli, Ashish Ramayee Asokan, Lakshay Sharma, and R Venkatesh Babu. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2024*

 - Gradient-Regulated Meta-Prompt Learning for Generalizable Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2303.06571v2)
    - Juncheng Li, Minghe Gao, Longhui Wei, Siliang Tang, Wenqiao Zhang, Mengze Li, Wei Ji, Qi Tian, Tat-Seng Chua, and Yueting Zhuang. *Proceedings of the IEEE/CVF International Conference on Computer Vision (ICCV) 2023*

 - Leveraging Vision-Language Models for Improving Domain Generalization in Image Classification.
    [pdf](https://arxiv.org/pdf/2310.08255)
    - Sravanti Addepalli, Ashish Ramayee Asokan, Lakshay Sharma, and R Venkatesh Babu. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2024*

 - Gradient-Regulated Meta-Prompt Learning for Generalizable Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2303.06571v2)
    - Juncheng Li, Minghe Gao, Longhui Wei, Siliang Tang, Wenqiao Zhang, Mengze Li, Wei Ji, Qi Tian, Tat-Seng Chua, and Yueting Zhuang. *Proceedings of the IEEE/CVF International Conference on Computer Vision (ICCV) 2023*

 - RobustLR: A diagnostic benchmark for evaluating logical robustness of deductive reasoners.
    [pdf](https://aclanthology.org/2022.emnlp-main.653.pdf)
    - Soumya Sanyal, Zeyi Liao, and Xiang Ren. *Proceedings of the 2022 Conference on Empirical Methods in Natural Language Processing 2022*

 - This is not a Dataset: A Large Negation Benchmark to Challenge Large Language Models.
    [pdf](https://arxiv.org/pdf/2310.15941)
    - Iker García-Ferrero, Begoña Altuna, Javier Alvez, Itziar Gonzalez-Dios, and German Rigau. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Evaluating the Impact of Model Scale for Compositional Generalization in Semantic Parsing.
    [pdf](https://aclanthology.org/2022.emnlp-main.624.pdf)
    - Linlu Qiu, Peter Shaw, Panupong Pasupat, Tianze Shi, Jonathan Herzig, Emily Pitler, Fei Sha, and Kristina Toutanova. *Proceedings of the 2022 Conference on Empirical Methods in Natural Language Processing 2022*

### Tuning Method
 - How Do In-Context Examples Affect Compositional Generalization?.
    [pdf](https://aclanthology.org/2023.acl-long.618.pdf)
    - Shengnan An, Zeqi Lin, Qiang Fu, Bei Chen, Nanning Zheng, Jian-Guang Lou, and Dongmei Zhang. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - MAGNIFICo: Evaluating the In-Context Learning Ability of Large Language Models to Generalize to Novel Interpretations.
    [pdf](https://arxiv.org/pdf/2310.11634)
    - Arkil Patel, Satwik Bhattamishra, Siva Reddy, and Dzmitry Bahdanau. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Enhancing job recommendation through llm-based generative adversarial networks.
    [pdf](https://arxiv.org/pdf/2307.10747)
    - Yingpeng Du, Di Luo, Rui Yan, Xiaopei Wang, Hongzhi Liu, Hengshu Zhu, Yang Song, and Jie Zhang. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - How Do In-Context Examples Affect Compositional Generalization?.
    [pdf](https://aclanthology.org/2023.acl-long.618.pdf)
    - Shengnan An, Zeqi Lin, Qiang Fu, Bei Chen, Nanning Zheng, Jian-Guang Lou, and Dongmei Zhang. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - RoCoIns: Enhancing Robustness of Large Language Models through Code-Style Instructions.
    [pdf](https://aclanthology.org/2024.lrec-main.1237.pdf)
    - Yuansen Zhang, Xiao Wang, Zhiheng Xi, Han Xia, Tao Gui, Qi Zhang, and Xuanjing Huang. *arXiv preprint arXiv:2402.16431 2024*

 - InstructDial: Improving Zero and Few-shot Generalization in Dialogue through Instruction Tuning.
    [pdf](https://arxiv.org/pdf/2205.12673)
    - Prakhar Gupta, Cathy Jiao, Yi-Ting Yeh, Shikib Mehri, Maxine Eskenazi, and Jeffrey P Bigham. *Proceedings of the 2022 Conference on Empirical Methods in Natural Language Processing 2022*

 - Augmentation-Adapted Retriever Improves Generalization of Language Models as Generic Plug-In.
    [pdf](https://aclanthology.org/2023.acl-long.136.pdf)
    - Zichun Yu, Chenyan Xiong, Shi Yu, and Zhiyuan Liu. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - Supervising model attention with human explanations for robust natural language inference.
    [pdf](https://arxiv.org/pdf/2104.08142)
    - Joe Stacey, Yonatan Belinkov, and Marek Rei. *Proceedings of the AAAI conference on artificial intelligence 2022*

 - Multitask Prompted Training Enables Zero-Shot Task Generalization.
    [pdf](https://arxiv.org/pdf/2110.08207)
    - Victor Sanh, Albert Webson, Colin Raffel, Stephen Bach, Lintang Sutawika, Zaid Alyafeai, Antoine Chaffin, Arnaud Stiegler, Arun Raja, Manan Dey, M Saiful Bari, Canwen Xu, Urmish Thakker, Shanya Sharma Sharma, Eliza Szczechla, Taewoon Kim, Gunjan Chhablani, Nihal Nayak, Debajyoti Datta, Jonathan Chang, Mike Tian-Jian Jiang, Han Wang, Matteo Manica, Sheng Shen, Zheng Xin Yong, Harshit Pandey, Rachel Bawden, Thomas Wang, Trishala Neeraj, Jos Rozen, Abheesht Sharma, Andrea Santilli, Thibault Fevry, Jason Alan Fries, Ryan Teehan, Teven Le Scao, Stella Biderman, Leo Gao, Thomas Wolf, and Alexander M Rush. *International Conference on Learning Representations 2022*

 - Zero-Shot Robustification of Zero-Shot Models.
    [pdf](https://arxiv.org/pdf/2309.04344)
    - Dyah Adila, Changho Shin, Linrong Cai, and Frederic Sala. *The Twelfth International Conference on Learning Representations 2024*

 - Compositional Task Representations for Large Language Models.
    [pdf](https://openreview.net/pdf?id=6axIMJA7ME3)
    - NAN SHAO, Zefan Cai, Hanwei xu, Chonghua Liao, Yanan Zheng, and Zhilin Yang. *The Eleventh International Conference on Learning Representations 2023*

 - Language-Driven Anchors for Zero-Shot Adversarial Robustness.
    [pdf](https://arxiv.org/pdf/2301.13096)
    - Xiao Li, Wei Zhang, Yining Liu, Zhanhao Hu, Bo Zhang, and Xiaolin Hu. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - Pre-trained Model Guided Fine-Tuning for Zero-Shot Adversarial Robustness.
    [pdf](https://arxiv.org/pdf/2401.04350)
    - Sibo Wang, Jie Zhang, Zheng Yuan, and Shiguang Shan. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - How Do In-Context Examples Affect Compositional Generalization?.
    [pdf](https://aclanthology.org/2023.acl-long.618.pdf)
    - Shengnan An, Zeqi Lin, Qiang Fu, Bei Chen, Nanning Zheng, Jian-Guang Lou, and Dongmei Zhang. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - MAGNIFICo: Evaluating the In-Context Learning Ability of Large Language Models to Generalize to Novel Interpretations.
    [pdf](https://aclanthology.org/2023.emnlp-main.134.pdf)
    - Arkil Patel, Satwik Bhattamishra, Siva Reddy, and Dzmitry Bahdanau. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Enhancing job recommendation through llm-based generative adversarial networks.
    [pdf](https://arxiv.org/pdf/2307.10747)
    - Yingpeng Du, Di Luo, Rui Yan, Xiaopei Wang, Hongzhi Liu, Hengshu Zhu, Yang Song, and Jie Zhang. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - How Do In-Context Examples Affect Compositional Generalization?.
    [pdf](https://aclanthology.org/2023.acl-long.618.pdf)
    - Shengnan An, Zeqi Lin, Qiang Fu, Bei Chen, Nanning Zheng, Jian-Guang Lou, and Dongmei Zhang. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - RoCoIns: Enhancing Robustness of Large Language Models through Code-Style Instructions.
    [pdf](https://aclanthology.org/2024.lrec-main.1237.pdf)
    - Yuansen Zhang, Xiao Wang, Zhiheng Xi, Han Xia, Tao Gui, Qi Zhang, and Xuanjing Huang. *arXiv preprint arXiv:2402.16431 2024*

 - Detecting Cybercrimes in Accordance with Pakistani Law: Dataset and Evaluation Using PLMs.
    [pdf](https://aclanthology.org/2024.lrec-main.422.pdf)
    - Faizad Ullah, Ali Faheem, Ubaid Azam, Muhammad Sohaib Ayub, Faisal Kamiran, and Asim Karim. *Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024) 2024*

 - InstructDial: Improving Zero and Few-shot Generalization in Dialogue through Instruction Tuning.
    [pdf](https://arxiv.org/pdf/2205.12673)
    - Prakhar Gupta, Cathy Jiao, Yi-Ting Yeh, Shikib Mehri, Maxine Eskenazi, and Jeffrey P Bigham. *Proceedings of the 2022 Conference on Empirical Methods in Natural Language Processing 2022*

 - Augmentation-Adapted Retriever Improves Generalization of Language Models as Generic Plug-In.
    [pdf](https://aclanthology.org/2023.acl-long.136.pdf)
    - Zichun Yu, Chenyan Xiong, Shi Yu, and Zhiyuan Liu. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - Supervising model attention with human explanations for robust natural language inference.
    [pdf](https://arxiv.org/pdf/2104.08142)
    - Joe Stacey, Yonatan Belinkov, and Marek Rei. *Proceedings of the AAAI conference on artificial intelligence 2022*

 - Multitask Prompted Training Enables Zero-Shot Task Generalization.
    [pdf](https://arxiv.org/pdf/2110.08207)
    - Victor Sanh, Albert Webson, Colin Raffel, Stephen Bach, Lintang Sutawika, Zaid Alyafeai, Antoine Chaffin, Arnaud Stiegler, Arun Raja, Manan Dey, M Saiful Bari, Canwen Xu, Urmish Thakker, Shanya Sharma Sharma, Eliza Szczechla, Taewoon Kim, Gunjan Chhablani, Nihal Nayak, Debajyoti Datta, Jonathan Chang, Mike Tian-Jian Jiang, Han Wang, Matteo Manica, Sheng Shen, Zheng Xin Yong, Harshit Pandey, Rachel Bawden, Thomas Wang, Trishala Neeraj, Jos Rozen, Abheesht Sharma, Andrea Santilli, Thibault Fevry, Jason Alan Fries, Ryan Teehan, Teven Le Scao, Stella Biderman, Leo Gao, Thomas Wolf, and Alexander M Rush. *International Conference on Learning Representations 2022*

 - What language model architecture and pretraining objective works best for zero-shot generalization?.
    [pdf](https://arxiv.org/pdf/2204.05832)
    - Thomas Wang, Adam Roberts, Daniel Hesslow, Teven Le Scao, Hyung Won Chung, Iz Beltagy, Julien Launay, and Colin Raffel. *International Conference on Machine Learning 2022*

 - Language-Driven Anchors for Zero-Shot Adversarial Robustness.
    [pdf](https://arxiv.org/pdf/2301.13096)
    - Xiao Li, Wei Zhang, Yining Liu, Zhanhao Hu, Bo Zhang, and Xiaolin Hu. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - Zero-Shot Robustification of Zero-Shot Models.
    [pdf](https://arxiv.org/pdf/2309.04344)
    - Dyah Adila, Changho Shin, Linrong Cai, and Frederic Sala. *The Twelfth International Conference on Learning Representations 2024*

 - Compositional Task Representations for Large Language Models.
    [pdf](https://openreview.net/pdf?id=6axIMJA7ME3)
    - NAN SHAO, Zefan Cai, Hanwei xu, Chonghua Liao, Yanan Zheng, and Zhilin Yang. *The Eleventh International Conference on Learning Representations 2023*

 - From Images to Textual Prompts: Zero-Shot Visual Question Answering With Frozen Large Language Models.
    [pdf](https://arxiv.org/pdf/2212.10846)
    - Jiaxian Guo, Junnan Li, Dongxu Li, Anthony Meng Huat Tiong, Boyang Li, Dacheng Tao, and Steven Hoi. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2023*

 - Finetuned Language Models are Zero-Shot Learners.
    [pdf](https://arxiv.org/pdf/2109.01652)
    - Jason Wei, Maarten Bosma, Vincent Zhao, Kelvin Guu, Adams Wei Yu, Brian Lester, Nan Du, Andrew M. Dai, and Quoc V Le. *International Conference on Learning Representations 2022*

 - Correcting Language Model Bias for Text Classification in True Zero-Shot Learning.
    [pdf](https://aclanthology.org/2024.lrec-main.359.pdf)
    - Feng Zhao, Wan Xianlin, Cheng Yan, and Chu Kiong Loo. *Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024) 2024*

 - A comprehensive survey on test-time adaptation under distribution shifts.
    [pdf](https://arxiv.org/pdf/2303.15361)
    - Jian Liang, Ran He, and Tieniu Tan. *International Journal of Computer Vision 2024*

 - Adapting to Distribution Shift by Visual Domain Prompt Generation.
    [pdf](https://openreview.net/pdf?id=sSaN4gxuEf)
    - Zhixiang Chi, Li Gu, Tao Zhong, Huan Liu, YUANHAO YU, Konstantinos N Plataniotis, and Yang Wang. *The Twelfth International Conference on Learning Representations 2024*

 - Efficient Test-Time Adaptation of Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2403.18293)
    - Adilbek Karmanov, Dayan Guan, Shijian Lu, Abdulmotaleb El Saddik, and Eric Xing. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2024*

 - Align your prompts: Test-time prompting with distribution alignment for zero-shot generalization.
    [pdf](https://openreview.net/pdf?id=CusNOTRkQw)
    - Jameel Abdul Samadh, Mohammad Hanan Gani, Noor Hussein, Muhammad Uzair Khattak, Muhammad Muzammal Naseer, Fahad Shahbaz Khan, and Salman H Khan. *Advances in Neural Information Processing Systems 2024*

 - Test-time prompt tuning for zero-shot generalization in vision-language models.
    [pdf](https://arxiv.org/abs/2209.07511)
    - Manli Shu, Weili Nie, De-An Huang, Zhiding Yu, Tom Goldstein, Anima Anandkumar, and Chaowei Xiao. *Advances in Neural Information Processing Systems 2022*

 - Test-Time Adaptation with CLIP Reward for Zero-Shot Generalization in Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2305.18010)
    - Shuai Zhao, Xiaohan Wang, Linchao Zhu, and Yi Yang. *The Twelfth International Conference on Learning Representations 2024*

 - On the Test-Time Zero-Shot Generalization of Vision-Language Models: Do We Really Need Prompt Learning?.
    [pdf](https://arxiv.org/pdf/2405.02266)
    - Maxime Zanella and Ismail Ben Ayed. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - Test-time prompt tuning for zero-shot generalization in vision-language models.
    [pdf](https://arxiv.org/pdf/2209.07511)
    - Manli Shu, Weili Nie, De-An Huang, Zhiding Yu, Tom Goldstein, Anima Anandkumar, and Chaowei Xiao. *Advances in Neural Information Processing Systems 2022*

 - Efficient Test-Time Adaptation of Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2403.18293)
    - Adilbek Karmanov, Dayan Guan, Shijian Lu, Abdulmotaleb El Saddik, and Eric Xing. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2024*

 - Align your prompts: Test-time prompting with distribution alignment for zero-shot generalization.
    [pdf](https://arxiv.org/pdf/2311.01459)
    - Jameel Abdul Samadh, Mohammad Hanan Gani, Noor Hussein, Muhammad Uzair Khattak, Muhammad Muzammal Naseer, Fahad Shahbaz Khan, and Salman H Khan. *Advances in Neural Information Processing Systems 2024*

 - Test-Time Adaptation with CLIP Reward for Zero-Shot Generalization in Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2305.18010)
    - Shuai Zhao, Xiaohan Wang, Linchao Zhu, and Yi Yang. *The Twelfth International Conference on Learning Representations 2024*

 - Training language models to follow instructions with human feedback.
    [pdf](https://arxiv.org/pdf/2203.02155)
    - Long Ouyang, Jeffrey Wu, Xu Jiang, Diogo Almeida, Carroll Wainwright, Pamela Mishkin, Chong Zhang, Sandhini Agarwal, Katarina Slama, Alex Ray, and others. *Advances in neural information processing systems 2022*

 - Direct preference optimization: your language model is secretly a reward model.
    [pdf](https://arxiv.org/pdf/2305.18290)
    - Rafael Rafailov, Archit Sharma, Eric Mitchell, Stefano Ermon, Christopher D Manning, and Chelsea Finn. *Proceedings of the 37th International Conference on Neural Information Processing Systems 2023*

 - Direct preference optimization: Your language model is secretly a reward model.
    [pdf](https://arxiv.org/pdf/2305.18290)
    - Rafael Rafailov, Archit Sharma, Eric Mitchell, Christopher D Manning, Stefano Ermon, and Chelsea Finn. *Advances in Neural Information Processing Systems 2024*

 - Improving the robustness of large language models via consistency alignment.
    [pdf](https://arxiv.org/pdf/2403.14221)
    - Zhao Yukun, Yan Lingyong, Sun Weiwei, Xing Guoliang, Wang Shuaiqiang, Meng Chong, Cheng Zhicong, Ren Zhaochun, and Yin Dawei. *arXiv preprint arXiv:2403.14221 2024*

 - DRESS: Instructing Large Vision-Language Models to Align and Interact with Humans via Natural Language Feedback.
    [pdf](https://arxiv.org/abs/2311.10081)
    - Yangyi Chen, Karan Sikka, Michael Cogswell, Heng Ji, and Ajay Divakaran. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - Pretraining language models with human preferences.
    [pdf](https://arxiv.org/pdf/2302.08582)
    - Tomasz Korbak, Kejian Shi, Angelica Chen, Rasika Vinayak Bhalerao, Christopher Buckley, Jason Phang, Samuel R Bowman, and Ethan Perez. *International Conference on Machine Learning 2023*

 - RLHF-V: Towards Trustworthy MLLMs via Behavior Alignment from Fine-grained Correctional Human Feedback.
    [pdf](https://arxiv.org/pdf/2312.00849)
    - Tianyu Yu, Yuan Yao, Haoye Zhang, Taiwen He, Yifeng Han, Ganqu Cui, Jinyi Hu, Zhiyuan Liu, Hai-Tao Zheng, Maosong Sun, and Tat-Seng Chua. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - Improving Generalization of Alignment with Human Preferences through Group Invariant Learning.
    [pdf](https://openreview.net/pdf?id=fwCoLe3TAX)
    - Rui Zheng, Wei Shen, Yuan Hua, Wenbin Lai, Shihan Dou, Yuhao Zhou, Zhiheng Xi, Xiao Wang, Haoran Huang, Tao Gui, Qi Zhang, and Xuanjing Huang. *The Twelfth International Conference on Learning Representations 2024*

 - Inverse-RLignment: Inverse Reinforcement Learning from Demonstrations for LLM Alignment.
    [pdf](https://openreview.net/pdf?id=BrUxhfVepA)
    - Hao Sun and Mihaela van der Schaar. *arXiv preprint arXiv:2405.15624 2024*

 - Large Language Models are biased to overestimate profoundness.
    [pdf](https://arxiv.org/pdf/2310.14422)
    - Eugenio Herrera-Berg, Tomas Browne, and Leon-Villagra. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Aligning as Debiasing: Causality-Aware Alignment via Reinforcement Learning with Interventional Feedback.
    [pdf](https://aclanthology.org/2024.naacl-long.262.pdf)
    - Yu Xia, Tong Yu, Zhankui He, Handong Zhao, Julian McAuley, and Shuai Li. *Proceedings of the 2024 Conference of the North American Chapter of the Association for Computational Linguistics: Human Language Technologies (Volume 1: Long Papers) 2024*

 - Moca: Measuring human-language model alignment on causal and moral judgment tasks.
    [pdf](https://arxiv.org/pdf/2310.19677)
    - Allen Nie, Yuhui Zhang, Atharva Shailesh Amdekar, Chris Piech, Tatsunori B Hashimoto, and Tobias Gerstenberg. *Advances in Neural Information Processing Systems 2024*

 - Optimizing Language Models for Human Preferences is a Causal Inference Problem.
    [pdf](https://arxiv.org/pdf/2402.14979)
    - Victoria Lin, Eli Ben-Michael, and Louis-Philippe Morency. *The 40th Conference on Uncertainty in Artificial Intelligence Unknown Year*

 - Improving the robustness of large language models via consistency alignment.
    [pdf](https://arxiv.org/pdf/2403.14221)
    - Zhao Yukun, Yan Lingyong, Sun Weiwei, Xing Guoliang, Wang Shuaiqiang, Meng Chong, Cheng Zhicong, Ren Zhaochun, and Yin Dawei. *arXiv preprint arXiv:2403.14221 2024*

 - Improving Generalization of Alignment with Human Preferences through Group Invariant Learning.
    [pdf](https://openreview.net/pdf?id=fwCoLe3TAX)
    - Rui Zheng, Wei Shen, Yuan Hua, Wenbin Lai, Shihan Dou, Yuhao Zhou, Zhiheng Xi, Xiao Wang, Haoran Huang, Tao Gui, Qi Zhang, and Xuanjing Huang. *The Twelfth International Conference on Learning Representations 2024*

 - Pretraining language models with human preferences.
    [pdf](https://arxiv.org/pdf/2302.08582)
    - Tomasz Korbak, Kejian Shi, Angelica Chen, Rasika Vinayak Bhalerao, Christopher Buckley, Jason Phang, Samuel R Bowman, and Ethan Perez. *International Conference on Machine Learning 2023*

 - DRESS: Instructing Large Vision-Language Models to Align and Interact with Humans via Natural Language Feedback.
    [pdf](https://arxiv.org/abs/2311.10081)
    - Yangyi Chen, Karan Sikka, Michael Cogswell, Heng Ji, and Ajay Divakaran. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - RLHF-V: Towards Trustworthy MLLMs via Behavior Alignment from Fine-grained Correctional Human Feedback.
    [pdf](https://arxiv.org/pdf/2312.00849)
    - Tianyu Yu, Yuan Yao, Haoye Zhang, Taiwen He, Yifeng Han, Ganqu Cui, Jinyi Hu, Zhiyuan Liu, Hai-Tao Zheng, Maosong Sun, and Tat-Seng Chua. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - Inverse-RLignment: Inverse Reinforcement Learning from Demonstrations for LLM Alignment.
    [pdf](https://openreview.net/pdf?id=BrUxhfVepA)
    - Hao Sun and Mihaela van der Schaar. *arXiv preprint arXiv:2405.15624 2024*

 - Large Language Models are biased to overestimate profoundness.
    [pdf](https://arxiv.org/pdf/2310.14422)
    - Eugenio Herrera-Berg, Tomas Browne, and Leon-Villagra. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Training language models to follow instructions with human feedback.
    [pdf](https://arxiv.org/pdf/2203.02155)
    - Long Ouyang, Jeffrey Wu, Xu Jiang, Diogo Almeida, Carroll Wainwright, Pamela Mishkin, Chong Zhang, Sandhini Agarwal, Katarina Slama, Alex Ray, and others. *Advances in neural information processing systems 2022*

 - On Robust Prefix-Tuning for Text Classification.
    [pdf](https://arxiv.org/pdf/2203.10378)
    - Zonghan Yang and Yang Liu. *International Conference on Learning Representations 2022*

 - Why Is Prompt Tuning for Vision-Language Models Robust to Noisy Labels?.
    [pdf](https://arxiv.org/pdf/2307.11978)
    - Cheng-En Wu, Yu Tian, Haichao Yu, Heng Wang, Pedro Morgado, Yu Hen Hu, and Linjie Yang. *Proceedings of the IEEE/CVF International Conference on Computer Vision (ICCV) 2023*

 - Understanding and Mitigating the Label Noise in Pre-training on Downstream Tasks.
    [pdf](https://arxiv.org/pdf/2309.17002)
    - Hao Chen, Jindong Wang, Ankit Shah, Ran Tao, Hongxin Wei, Xing Xie, Masashi Sugiyama, and Bhiksha Raj. *The Twelfth International Conference on Learning Representations 2024*

 - Exploring the limits of domain-adaptive training for detoxifying large-scale language models.
    [pdf](https://arxiv.org/pdf/2202.04173)
    - Boxin Wang, Wei Ping, Chaowei Xiao, Peng Xu, Mostofa Patwary, Mohammad Shoeybi, Bo Li, Anima Anandkumar, and Bryan Catanzaro. *Advances in Neural Information Processing Systems 2022*

 - Fine-tuning Aligned Language Models Compromises Safety, Even When Users Do Not Intend To!.
    [pdf](https://arxiv.org/pdf/2310.03693)
    - Xiangyu Qi, Yi Zeng, Tinghao Xie, Pin-Yu Chen, Ruoxi Jia, Prateek Mittal, and Peter Henderson. *The Twelfth International Conference on Learning Representations 2024*

 - Large Language Models Can Be Strong Differentially Private Learners.
    [pdf](https://arxiv.org/abs/2110.05679)
    - Xuechen Li, Florian Tramer, Percy Liang, and Tatsunori Hashimoto. *International Conference on Learning Representations 2022*

 - Differentially Private Fine-tuning of Language Models.
    [pdf](https://arxiv.org/abs/2110.06500)
    - Da Yu, Saurabh Naik, Arturs Backurs, Sivakanth Gopi, Huseyin A Inan, Gautam Kamath, Janardhan Kulkarni, Yin Tat Lee, Andre Manoel, Lukas Wutschitz, Sergey Yekhanin, and Huishuai Zhang. *International Conference on Learning Representations 2022*

 - Fairness-aware structured pruning in transformers.
    [pdf](https://arxiv.org/pdf/2312.15398)
    - Abdelrahman Zayed, Gon{}alo Mordido, Samira Shabanian, Ioana Baldini, and Sarath Chandar. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Specialist or Generalist? Instruction Tuning for Specific NLP Tasks.
    [pdf](https://arxiv.org/pdf/2310.15326)
    - Chufan Shi, Yixuan Su, Cheng Yang, Yujiu Yang, and Deng Cai. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - On Robust Prefix-Tuning for Text Classification.
    [pdf](https://arxiv.org/pdf/2203.10378)
    - Zonghan Yang and Yang Liu. *International Conference on Learning Representations 2022*

 - Understanding and Mitigating the Label Noise in Pre-training on Downstream Tasks.
    [pdf](https://arxiv.org/pdf/2309.17002)
    - Hao Chen, Jindong Wang, Ankit Shah, Ran Tao, Hongxin Wei, Xing Xie, Masashi Sugiyama, and Bhiksha Raj. *The Twelfth International Conference on Learning Representations 2024*

 - Why Is Prompt Tuning for Vision-Language Models Robust to Noisy Labels?.
    [pdf](https://arxiv.org/pdf/2307.11978)
    - Cheng-En Wu, Yu Tian, Haichao Yu, Heng Wang, Pedro Morgado, Yu Hen Hu, and Linjie Yang. *Proceedings of the IEEE/CVF International Conference on Computer Vision (ICCV) 2023*

 - Exploring the limits of domain-adaptive training for detoxifying large-scale language models.
    [pdf](https://arxiv.org/pdf/2202.04173)
    - Boxin Wang, Wei Ping, Chaowei Xiao, Peng Xu, Mostofa Patwary, Mohammad Shoeybi, Bo Li, Anima Anandkumar, and Bryan Catanzaro. *Advances in Neural Information Processing Systems 2022*

 - Fine-tuning Aligned Language Models Compromises Safety, Even When Users Do Not Intend To!.
    [pdf](https://arxiv.org/pdf/2310.03693)
    - Xiangyu Qi, Yi Zeng, Tinghao Xie, Pin-Yu Chen, Ruoxi Jia, Prateek Mittal, and Peter Henderson. *The Twelfth International Conference on Learning Representations 2024*

 - Large Language Models Can Be Strong Differentially Private Learners.
    [pdf](https://arxiv.org/abs/2110.05679)
    - Xuechen Li, Florian Tramer, Percy Liang, and Tatsunori Hashimoto. *International Conference on Learning Representations 2022*

 - Differentially Private Fine-tuning of Language Models.
    [pdf](https://arxiv.org/abs/2110.06500)
    - Da Yu, Saurabh Naik, Arturs Backurs, Sivakanth Gopi, Huseyin A Inan, Gautam Kamath, Janardhan Kulkarni, Yin Tat Lee, Andre Manoel, Lukas Wutschitz, Sergey Yekhanin, and Huishuai Zhang. *International Conference on Learning Representations 2022*

 - Fairness-aware structured pruning in transformers.
    [pdf](https://arxiv.org/pdf/2312.15398)
    - Abdelrahman Zayed, Gon{}alo Mordido, Samira Shabanian, Ioana Baldini, and Sarath Chandar. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*




### Hallucination
 - The curious case of hallucinatory (un) answerability: Finding truths in the hidden states of over-confident large language models.
    [pdf](https://arxiv.org/pdf/2310.11877)
    - Aviv Slobodkin, Omer Goldman, Avi Caciularu, Ido Dagan, and Shauli Ravfogel. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Attention Satisfies: A Constraint-Satisfaction Lens on Factual Errors of Language Models.
    [pdf](https://arxiv.org/pdf/2309.15098)
    - Mert Yuksekgonul, Varun Chandrasekaran, Erik Jones, Suriya Gunasekar, Ranjita Naik, Hamid Palangi, Ece Kamar, and Besmira Nushi. *The Twelfth International Conference on Learning Representations 2024*

 - DoLa: Decoding by Contrasting Layers Improves Factuality in Large Language Models.
    [pdf](https://arxiv.org/pdf/2309.03883)
    - Yung-Sung Chuang, Yujia Xie, Hongyin Luo, Yoon Kim, James R. Glass, and Pengcheng He. *The Twelfth International Conference on Learning Representations 2024*

 - Mitigating Object Hallucinations in Large Vision-Language Models through Visual Contrastive Decoding.
    [pdf](https://arxiv.org/pdf/2311.16922)
    - Sicong Leng, Hang Zhang, Guanzheng Chen, Xin Li, Shijian Lu, Chunyan Miao, and Lidong Bing. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - VISTA-LLAMA: Reducing Hallucination in Video Language Models via Equal Distance to Visual Tokens.
    [pdf](https://arxiv.org/pdf/2312.08870)
    - Fan Ma, Xiaojie Jin, Heng Wang, Yuchen Xian, Jiashi Feng, and Yi Yang. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - Teaching Language Models to Hallucinate Less with Synthetic Tasks.
    [pdf](https://arxiv.org/pdf/2310.06827)
    - Erik Jones, Hamid Palangi, Clarisse Simoes Ribeiro, Varun Chandrasekaran, Subhabrata Mukherjee, Arindam Mitra, Ahmed Hassan Awadallah, and Ece Kamar. *The Twelfth International Conference on Learning Representations 2024*

 - Mitigating large language model hallucinations via autonomous knowledge graph-based retrofitting.
    [pdf](https://arxiv.org/pdf/2311.13314)
    - Xinyan Guan, Yanjiang Liu, Hongyu Lin, Yaojie Lu, Ben He, Xianpei Han, and Le Sun. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Identifying and mitigating spurious correlations for improving robustness in nlp models.
    [pdf](https://aclanthology.org/2022.findings-naacl.130.pdf)
    - Tianlu Wang, Rohit Sridhar, Diyi Yang, and Xuezhi Wang. *arXiv preprint arXiv:2110.07736 2021*

 - A Cause-Effect Look at Alleviating Hallucination of Knowledge-grounded Dialogue Generation.
    [pdf](https://arxiv.org/pdf/2404.03491)
    - Jifan Yu, Xiaohan Zhang, Yifan Xu, Xuanyu Lei, Zijun Yao, Jing Zhang, Lei Hou, and Juanzi Li. *arXiv preprint arXiv:2404.03491 2024*

 - Causal-debias: Unifying debiasing in pretrained language models and fine-tuning via causal invariant learning.
    [pdf](https://aclanthology.org/2023.acl-long.232.pdf)
    - Fan Zhou, Yuzhou Mao, Liu Yu, Yi Yang, and Ting Zhong. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - Fine-Tuning Language Models for Factuality.
    [pdf](https://arxiv.org/pdf/2311.08401)
    - Katherine Tian, Eric Mitchell, Huaxiu Yao, Christopher D Manning, and Chelsea Finn. *The Twelfth International Conference on Learning Representations 2024*

 - Ontofact: Unveiling fantastic fact-skeleton of llms via ontology-driven reinforcement learning.
    [pdf](https://ojs.aaai.org/index.php/AAAI/article/download/29859/31497)
    - Ziyu Shang, Wenjun Ke, Nana Xiu, Peng Wang, Jiajun Liu, Yanhui Li, Zhizhao Luo, and Ke Ji. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Enhancing job recommendation through llm-based generative adversarial networks.
    [pdf](https://arxiv.org/pdf/2307.10747)
    - Yingpeng Du, Di Luo, Rui Yan, Xiaopei Wang, Hongzhi Liu, Hengshu Zhu, Yang Song, and Jie Zhang. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Detecting and preventing hallucinations in large vision language models.
    [pdf](https://arxiv.org/pdf/2308.06394)
    - Anisha Gunjal, Jihan Yin, and Erhan Bas. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Evaluating Object Hallucination in Large Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2305.10355)
    - Yifan Li, Yifan Du, Kun Zhou, Jinpeng Wang, Wayne Xin Zhao, and Ji-Rong Wen. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Detecting and preventing hallucinations in large vision language models.
    [pdf](https://arxiv.org/pdf/2308.06394)
    - Anisha Gunjal, Jihan Yin, and Erhan Bas. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Hallucination Augmented Contrastive Learning for Multimodal Large Language Model.
    [pdf](https://arxiv.org/pdf/2312.06968)
    - Chaoya Jiang, Haiyang Xu, Mengfan Dong, Jiaxing Chen, Wei Ye, Ming Yan, Qinghao Ye, Ji Zhang, Fei Huang, and Shikun Zhang. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - The curious case of hallucinatory (un) answerability: Finding truths in the hidden states of over-confident large language models.
    [pdf](https://arxiv.org/pdf/2310.11877)
    - Aviv Slobodkin, Omer Goldman, Avi Caciularu, Ido Dagan, and Shauli Ravfogel. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Ontofact: Unveiling fantastic fact-skeleton of llms via ontology-driven reinforcement learning.
    [pdf](https://ojs.aaai.org/index.php/AAAI/article/download/29859/31497)
    - Ziyu Shang, Wenjun Ke, Nana Xiu, Peng Wang, Jiajun Liu, Yanhui Li, Zhizhao Luo, and Ke Ji. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Attention Satisfies: A Constraint-Satisfaction Lens on Factual Errors of Language Models.
    [pdf](https://arxiv.org/pdf/2309.15098)
    - Mert Yuksekgonul, Varun Chandrasekaran, Erik Jones, Suriya Gunasekar, Ranjita Naik, Hamid Palangi, Ece Kamar, and Besmira Nushi. *The Twelfth International Conference on Learning Representations 2024*

 - DoLa: Decoding by Contrasting Layers Improves Factuality in Large Language Models.
    [pdf](https://arxiv.org/pdf/2309.03883)
    - Yung-Sung Chuang, Yujia Xie, Hongyin Luo, Yoon Kim, James R. Glass, and Pengcheng He. *The Twelfth International Conference on Learning Representations 2024*

 - Teaching Language Models to Hallucinate Less with Synthetic Tasks.
    [pdf](https://arxiv.org/pdf/2310.06827)
    - Erik Jones, Hamid Palangi, Clarisse Simoes Ribeiro, Varun Chandrasekaran, Subhabrata Mukherjee, Arindam Mitra, Ahmed Hassan Awadallah, and Ece Kamar. *The Twelfth International Conference on Learning Representations 2024*

 - Mitigating large language model hallucinations via autonomous knowledge graph-based retrofitting.
    [pdf](https://arxiv.org/pdf/2311.13314)
    - Xinyan Guan, Yanjiang Liu, Hongyu Lin, Yaojie Lu, Ben He, Xianpei Han, and Le Sun. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Fine-Tuning Language Models for Factuality.
    [pdf](https://arxiv.org/pdf/2311.08401)
    - Katherine Tian, Eric Mitchell, Huaxiu Yao, Christopher D Manning, and Chelsea Finn. *The Twelfth International Conference on Learning Representations 2024*

 - Ontofact: Unveiling fantastic fact-skeleton of llms via ontology-driven reinforcement learning.
    [pdf](https://ojs.aaai.org/index.php/AAAI/article/download/29859/31497)
    - Ziyu Shang, Wenjun Ke, Nana Xiu, Peng Wang, Jiajun Liu, Yanhui Li, Zhizhao Luo, and Ke Ji. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Enhancing job recommendation through llm-based generative adversarial networks.
    [pdf](https://arxiv.org/pdf/2307.10747)
    - Yingpeng Du, Di Luo, Rui Yan, Xiaopei Wang, Hongzhi Liu, Hengshu Zhu, Yang Song, and Jie Zhang. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Detecting and preventing hallucinations in large vision language models.
    [pdf](https://arxiv.org/pdf/2308.06394)
    - Anisha Gunjal, Jihan Yin, and Erhan Bas. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Analyzing and Mitigating Object Hallucination in Large Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2310.00754)
    - Yiyang Zhou, Chenhang Cui, Jaehong Yoon, Linjun Zhang, Zhun Deng, Chelsea Finn, Mohit Bansal, and Huaxiu Yao. *The Twelfth International Conference on Learning Representations 2024*

 - Mitigating Object Hallucinations in Large Vision-Language Models through Visual Contrastive Decoding.
    [pdf](https://arxiv.org/pdf/2311.16922)
    - Sicong Leng, Hang Zhang, Guanzheng Chen, Xin Li, Shijian Lu, Chunyan Miao, and Lidong Bing. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - VISTA-LLAMA: Reducing Hallucination in Video Language Models via Equal Distance to Visual Tokens.
    [pdf](https://arxiv.org/pdf/2312.08870)
    - Fan Ma, Xiaojie Jin, Heng Wang, Yuchen Xian, Jiashi Feng, and Yi Yang. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - Evaluating Object Hallucination in Large Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2305.10355)
    - Yifan Li, Yifan Du, Kun Zhou, Jinpeng Wang, Wayne Xin Zhao, and Ji-Rong Wen. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Detecting and preventing hallucinations in large vision language models.
    [pdf](https://arxiv.org/pdf/2308.06394)
    - Anisha Gunjal, Jihan Yin, and Erhan Bas. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Hallucination Augmented Contrastive Learning for Multimodal Large Language Model.
    [pdf](https://arxiv.org/pdf/2312.06968)
    - Chaoya Jiang, Haiyang Xu, Mengfan Dong, Jiaxing Chen, Wei Ye, Ming Yan, Qinghao Ye, Ji Zhang, Fei Huang, and Shikun Zhang. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - RAPPER: Reinforced Rationale-Prompted Paradigm for Natural Language Explanation in Visual Question Answering.
    [pdf](https://openreview.net/pdf?id=bshfchPM9H)
    - Kai-Po Chang, Chi-Pin Huang, Wei-Yuan Cheng, Fu-En Yang, Chien-Yi Wang, Yung-Hsuan Lai, and Yu-Chiang Frank Wang. *The Twelfth International Conference on Learning Representations 2024*

 - OPERA: Alleviating Hallucination in Multi-Modal Large Language Models via Over-Trust Penalty and Retrospection-Allocation.
    [pdf](https://arxiv.org/pdf/2311.17911)
    - Qidong Huang, Xiaoyi Dong, Pan Zhang, Bin Wang, Conghui He, Jiaqi Wang, Dahua Lin, Weiming Zhang, and Nenghai Yu. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - RLHF-V: Towards Trustworthy MLLMs via Behavior Alignment from Fine-grained Correctional Human Feedback.
    [pdf](https://arxiv.org/pdf/2312.00849)
    - Tianyu Yu, Yuan Yao, Haoye Zhang, Taiwen He, Yifeng Han, Ganqu Cui, Jinyi Hu, Zhiyuan Liu, Hai-Tao Zheng, Maosong Sun, and Tat-Seng Chua. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - Identifying and mitigating spurious correlations for improving robustness in nlp models.
    [pdf](https://arxiv.org/pdf/2110.07736)
    - Tianlu Wang, Rohit Sridhar, Diyi Yang, and Xuezhi Wang. *arXiv preprint arXiv:2110.07736 2021*

 - A Cause-Effect Look at Alleviating Hallucination of Knowledge-grounded Dialogue Generation.
    [pdf](https://arxiv.org/pdf/2404.03491)
    - Jifan Yu, Xiaohan Zhang, Yifan Xu, Xuanyu Lei, Zijun Yao, Jing Zhang, Lei Hou, and Juanzi Li. *arXiv preprint arXiv:2404.03491 2024*

### Causal Enhanced Solution
 - How Do In-Context Examples Affect Compositional Generalization?.
    [pdf](https://aclanthology.org/2023.acl-long.618.pdf)
    - Shengnan An, Zeqi Lin, Qiang Fu, Bei Chen, Nanning Zheng, Jian-Guang Lou, and Dongmei Zhang. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - MAGNIFICo: Evaluating the In-Context Learning Ability of Large Language Models to Generalize to Novel Interpretations.
    [pdf](https://aclanthology.org/2023.emnlp-main.134.pdf)
    - Arkil Patel, Satwik Bhattamishra, Siva Reddy, and Dzmitry Bahdanau. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Enhancing job recommendation through llm-based generative adversarial networks.
    [pdf](https://arxiv.org/pdf/2307.10747)
    - Yingpeng Du, Di Luo, Rui Yan, Xiaopei Wang, Hongzhi Liu, Hengshu Zhu, Yang Song, and Jie Zhang. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - How Do In-Context Examples Affect Compositional Generalization?.
    [pdf](https://aclanthology.org/2023.acl-long.618.pdf)
    - Shengnan An, Zeqi Lin, Qiang Fu, Bei Chen, Nanning Zheng, Jian-Guang Lou, and Dongmei Zhang. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - RoCoIns: Enhancing Robustness of Large Language Models through Code-Style Instructions.
    [pdf](https://arxiv.org/pdf/2402.16431)
    - Yuansen Zhang, Xiao Wang, Zhiheng Xi, Han Xia, Tao Gui, Qi Zhang, and Xuanjing Huang. *arXiv preprint arXiv:2402.16431 2024*

- Detecting Cybercrimes in Accordance with Pakistani Law: Dataset and Evaluation Using PLMs.
  [pdf](https://aclanthology.org/2024.lrec-main.422.pdf)
    - Faizad Ullah, Ali Faheem, Ubaid Azam, Muhammad Sohaib Ayub, Faisal Kamiran, and Asim Karim. *Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024) 2024*

 - InstructDial: Improving Zero and Few-shot Generalization in Dialogue through Instruction Tuning.
    [pdf](https://arxiv.org/pdf/2205.12673)
    - Prakhar Gupta, Cathy Jiao, Yi-Ting Yeh, Shikib Mehri, Maxine Eskenazi, and Jeffrey P Bigham. *Proceedings of the 2022 Conference on Empirical Methods in Natural Language Processing 2022*

 - HINT: Hypernetwork Instruction Tuning for Efficient Zero-and Few-Shot Generalisation.
    [pdf](https://arxiv.org/pdf/2212.10315)
    - Hamish Ivison, Akshita Bhagia, Yizhong Wang, Hannaneh Hajishirzi, and Matthew E Peters. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - Augmentation-Adapted Retriever Improves Generalization of Language Models as Generic Plug-In.
    [pdf](https://arxiv.org/pdf/2305.17331)
    - Zichun Yu, Chenyan Xiong, Shi Yu, and Zhiyuan Liu. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - Supervising model attention with human explanations for robust natural language inference.
    [pdf](https://arxiv.org/pdf/2104.08142)
    - Joe Stacey, Yonatan Belinkov, and Marek Rei. *Proceedings of the AAAI conference on artificial intelligence 2022*

 - Multitask Prompted Training Enables Zero-Shot Task Generalization.
    [pdf](https://arxiv.org/pdf/2110.08207)
    - Victor Sanh, Albert Webson, Colin Raffel, Stephen Bach, Lintang Sutawika, Zaid Alyafeai, Antoine Chaffin, Arnaud Stiegler, Arun Raja, Manan Dey, M Saiful Bari, Canwen Xu, Urmish Thakker, Shanya Sharma Sharma, Eliza Szczechla, Taewoon Kim, Gunjan Chhablani, Nihal Nayak, Debajyoti Datta, Jonathan Chang, Mike Tian-Jian Jiang, Han Wang, Matteo Manica, Sheng Shen, Zheng Xin Yong, Harshit Pandey, Rachel Bawden, Thomas Wang, Trishala Neeraj, Jos Rozen, Abheesht Sharma, Andrea Santilli, Thibault Fevry, Jason Alan Fries, Ryan Teehan, Teven Le Scao, Stella Biderman, Leo Gao, Thomas Wolf, and Alexander M Rush. *International Conference on Learning Representations 2022*

 - What language model architecture and pretraining objective works best for zero-shot generalization?.
    [pdf](https://arxiv.org/pdf/2204.05832)
    - Thomas Wang, Adam Roberts, Daniel Hesslow, Teven Le Scao, Hyung Won Chung, Iz Beltagy, Julien Launay, and Colin Raffel. *International Conference on Machine Learning 2022*

 - Language-Driven Anchors for Zero-Shot Adversarial Robustness.
    [pdf](https://arxiv.org/pdf/2301.13096)
    - Xiao Li, Wei Zhang, Yining Liu, Zhanhao Hu, Bo Zhang, and Xiaolin Hu. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - Pre-trained Model Guided Fine-Tuning for Zero-Shot Adversarial Robustness.
    [pdf](https://arxiv.org/pdf/2401.04350)
    - Sibo Wang, Jie Zhang, Zheng Yuan, and Shiguang Shan. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - Zero-Shot Robustification of Zero-Shot Models.
    [pdf](https://arxiv.org/pdf/2309.04344)
    - Dyah Adila, Changho Shin, Linrong Cai, and Frederic Sala. *The Twelfth International Conference on Learning Representations 2024*

 - Compositional Task Representations for Large Language Models.
    [pdf](https://openreview.net/pdf?id=6axIMJA7ME3)
    - NAN SHAO, Zefan Cai, Hanwei xu, Chonghua Liao, Yanan Zheng, and Zhilin Yang. *The Eleventh International Conference on Learning Representations 2023*

 - From Images to Textual Prompts: Zero-Shot Visual Question Answering With Frozen Large Language Models.
    [pdf](https://arxiv.org/pdf/2212.10846)
    - Jiaxian Guo, Junnan Li, Dongxu Li, Anthony Meng Huat Tiong, Boyang Li, Dacheng Tao, and Steven Hoi. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2023*

 - Finetuned Language Models are Zero-Shot Learners.
    [pdf](https://arxiv.org/pdf/2109.01652)
    - Jason Wei, Maarten Bosma, Vincent Zhao, Kelvin Guu, Adams Wei Yu, Brian Lester, Nan Du, Andrew M. Dai, and Quoc V Le. *International Conference on Learning Representations 2022*

- Correcting Language Model Bias for Text Classification in True Zero-Shot Learning.
  [pdf](https://aclanthology.org/2024.lrec-main.359.pdf)
    - Feng Zhao, Wan Xianlin, Cheng Yan, and Chu Kiong Loo. *LREC-COLING 2024*

 - A comprehensive survey on test-time adaptation under distribution shifts.
    [pdf](https://arxiv.org/pdf/2303.15361)
    - Jian Liang, Ran He, and Tieniu Tan. *International Journal of Computer Vision 2024*

 - Adapting to Distribution Shift by Visual Domain Prompt Generation.
    [pdf](https://arxiv.org/pdf/2405.02797)
    - Zhixiang Chi, Li Gu, Tao Zhong, Huan Liu, YUANHAO YU, Konstantinos N Plataniotis, and Yang Wang. *The Twelfth International Conference on Learning Representations 2024*

 - Efficient Test-Time Adaptation of Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2403.18293)
    - Adilbek Karmanov, Dayan Guan, Shijian Lu, Abdulmotaleb El Saddik, and Eric Xing. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2024*

 - Align your prompts: Test-time prompting with distribution alignment for zero-shot generalization.
    [pdf](https://arxiv.org/pdf/2311.01459)
    - Jameel Abdul Samadh, Mohammad Hanan Gani, Noor Hussein, Muhammad Uzair Khattak, Muhammad Muzammal Naseer, Fahad Shahbaz Khan, and Salman H Khan. *Advances in Neural Information Processing Systems 2024*

 - Test-time prompt tuning for zero-shot generalization in vision-language models.
    [pdf](https://arxiv.org/pdf/2209.07511)
    - Manli Shu, Weili Nie, De-An Huang, Zhiding Yu, Tom Goldstein, Anima Anandkumar, and Chaowei Xiao. *Advances in Neural Information Processing Systems 2022*

 - Test-Time Adaptation with CLIP Reward for Zero-Shot Generalization in Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2305.18010)
    - Shuai Zhao, Xiaohan Wang, Linchao Zhu, and Yi Yang. *The Twelfth International Conference on Learning Representations 2024*

 - On the Test-Time Zero-Shot Generalization of Vision-Language Models: Do We Really Need Prompt Learning?.
    [pdf](https://arxiv.org/pdf/2405.02266)
    - Maxime Zanella and Ismail Ben Ayed. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - Test-time prompt tuning for zero-shot generalization in vision-language models.
    [pdf](https://arxiv.org/pdf/2209.07511)
    - Manli Shu, Weili Nie, De-An Huang, Zhiding Yu, Tom Goldstein, Anima Anandkumar, and Chaowei Xiao. *Advances in Neural Information Processing Systems 2022*

 - Efficient Test-Time Adaptation of Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2403.18293)
    - Adilbek Karmanov, Dayan Guan, Shijian Lu, Abdulmotaleb El Saddik, and Eric Xing. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2024*

 - Align your prompts: Test-time prompting with distribution alignment for zero-shot generalization.
    [pdf](https://arxiv.org/pdf/2311.01459)
    - Jameel Abdul Samadh, Mohammad Hanan Gani, Noor Hussein, Muhammad Uzair Khattak, Muhammad Muzammal Naseer, Fahad Shahbaz Khan, and Salman H Khan. *Advances in Neural Information Processing Systems 2024*

 - Test-Time Adaptation with CLIP Reward for Zero-Shot Generalization in Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2305.18010)
    - Shuai Zhao, Xiaohan Wang, Linchao Zhu, and Yi Yang. *The Twelfth International Conference on Learning Representations 2024*

 - Align your prompts: Test-time prompting with distribution alignment for zero-shot generalization.
    [pdf](https://arxiv.org/pdf/2311.01459)
    - Jameel Abdul Samadh, Mohammad Hanan Gani, Noor Hussein, Muhammad Uzair Khattak, Muhammad Muzammal Naseer, Fahad Shahbaz Khan, and Salman H Khan. *Advances in Neural Information Processing Systems 2024*

 - Test-time prompt tuning for zero-shot generalization in vision-language models.
    [pdf](https://arxiv.org/pdf/2209.07511)
    - Manli Shu, Weili Nie, De-An Huang, Zhiding Yu, Tom Goldstein, Anima Anandkumar, and Chaowei Xiao. *Advances in Neural Information Processing Systems 2022*

 - Test-Time Adaptation with CLIP Reward for Zero-Shot Generalization in Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2305.18010)
    - Shuai Zhao, Xiaohan Wang, Linchao Zhu, and Yi Yang. *The Twelfth International Conference on Learning Representations 2024*

 - On the Test-Time Zero-Shot Generalization of Vision-Language Models: Do We Really Need Prompt Learning?.
    [pdf](https://arxiv.org/pdf/2405.02266)
    - Maxime Zanella and Ismail Ben Ayed. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - Align your prompts: Test-time prompting with distribution alignment for zero-shot generalization.
    [pdf](https://arxiv.org/pdf/2311.01459)
    - Jameel Abdul Samadh, Mohammad Hanan Gani, Noor Hussein, Muhammad Uzair Khattak, Muhammad Muzammal Naseer, Fahad Shahbaz Khan, and Salman H Khan. *Advances in Neural Information Processing Systems 2024*

 - Test-time prompt tuning for zero-shot generalization in vision-language models.
    [pdf](https://arxiv.org/pdf/2209.07511)
    - Manli Shu, Weili Nie, De-An Huang, Zhiding Yu, Tom Goldstein, Anima Anandkumar, and Chaowei Xiao. *Advances in Neural Information Processing Systems 2022*

 - Test-Time Adaptation with CLIP Reward for Zero-Shot Generalization in Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2305.18010)
    - Shuai Zhao, Xiaohan Wang, Linchao Zhu, and Yi Yang. *The Twelfth International Conference on Learning Representations 2024*

 - On the Test-Time Zero-Shot Generalization of Vision-Language Models: Do We Really Need Prompt Learning?.
    [pdf](https://arxiv.org/pdf/2405.02266)
    - Maxime Zanella and Ismail Ben Ayed. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - Language-Driven Anchors for Zero-Shot Adversarial Robustness.
    [pdf](https://arxiv.org/pdf/2301.13096)
    - Xiao Li, Wei Zhang, Yining Liu, Zhanhao Hu, Bo Zhang, and Xiaolin Hu. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - Pre-trained Model Guided Fine-Tuning for Zero-Shot Adversarial Robustness.
    [pdf](https://arxiv.org/pdf/2401.04350)
    - Sibo Wang, Jie Zhang, Zheng Yuan, and Shiguang Shan. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - Language-Driven Anchors for Zero-Shot Adversarial Robustness.
    [pdf](https://arxiv.org/pdf/2301.13096)
    - Xiao Li, Wei Zhang, Yining Liu, Zhanhao Hu, Bo Zhang, and Xiaolin Hu. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - Pre-trained Model Guided Fine-Tuning for Zero-Shot Adversarial Robustness.
    [pdf](https://arxiv.org/pdf/2401.04350)
    - Sibo Wang, Jie Zhang, Zheng Yuan, and Shiguang Shan. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - What language model architecture and pretraining objective works best for zero-shot generalization?.
    [pdf](https://arxiv.org/pdf/2204.05832)
    - Thomas Wang, Adam Roberts, Daniel Hesslow, Teven Le Scao, Hyung Won Chung, Iz Beltagy, Julien Launay, and Colin Raffel. *International Conference on Machine Learning 2022*

 - Zero-Shot Robustification of Zero-Shot Models.
    [pdf](https://arxiv.org/pdf/2309.04344)
    - Dyah Adila, Changho Shin, Linrong Cai, and Frederic Sala. *The Twelfth International Conference on Learning Representations 2024*

 - Compositional Task Representations for Large Language Models.
    [pdf](https://openreview.net/pdf?id=6axIMJA7ME3)
    - NAN SHAO, Zefan Cai, Hanwei xu, Chonghua Liao, Yanan Zheng, and Zhilin Yang. *The Eleventh International Conference on Learning Representations 2023*

 - Finetuned Language Models are Zero-Shot Learners.
    [pdf](https://arxiv.org/pdf/2109.01652)
    - Jason Wei, Maarten Bosma, Vincent Zhao, Kelvin Guu, Adams Wei Yu, Brian Lester, Nan Du, Andrew M. Dai, and Quoc V Le. *International Conference on Learning Representations 2022*

 - Multitask Prompted Training Enables Zero-Shot Task Generalization.
    [pdf](https://arxiv.org/pdf/2110.08207)
    - Victor Sanh, Albert Webson, Colin Raffel, Stephen Bach, Lintang Sutawika, Zaid Alyafeai, Antoine Chaffin, Arnaud Stiegler, Arun Raja, Manan Dey, M Saiful Bari, Canwen Xu, Urmish Thakker, Shanya Sharma Sharma, Eliza Szczechla, Taewoon Kim, Gunjan Chhablani, Nihal Nayak, Debajyoti Datta, Jonathan Chang, Mike Tian-Jian Jiang, Han Wang, Matteo Manica, Sheng Shen, Zheng Xin Yong, Harshit Pandey, Rachel Bawden, Thomas Wang, Trishala Neeraj, Jos Rozen, Abheesht Sharma, Andrea Santilli, Thibault Fevry, Jason Alan Fries, Ryan Teehan, Teven Le Scao, Stella Biderman, Leo Gao, Thomas Wolf, and Alexander M Rush. *International Conference on Learning Representations 2022*

 - From Images to Textual Prompts: Zero-Shot Visual Question Answering With Frozen Large Language Models.
    [pdf](https://arxiv.org/pdf/2212.10846)
    - Jiaxian Guo, Junnan Li, Dongxu Li, Anthony Meng Huat Tiong, Boyang Li, Dacheng Tao, and Steven Hoi. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2023*

 - Enhancing job recommendation through llm-based generative adversarial networks.
    [pdf](https://arxiv.org/pdf/2307.10747)
    - Yingpeng Du, Di Luo, Rui Yan, Xiaopei Wang, Hongzhi Liu, Hengshu Zhu, Yang Song, and Jie Zhang. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Supervising model attention with human explanations for robust natural language inference.
    [pdf](https://arxiv.org/pdf/2104.08142)
    - Joe Stacey, Yonatan Belinkov, and Marek Rei. *Proceedings of the AAAI conference on artificial intelligence 2022*

 - RoCoIns: Enhancing Robustness of Large Language Models through Code-Style Instructions.
    [pdf](https://arxiv.org/pdf/2402.16431)
    - Yuansen Zhang, Xiao Wang, Zhiheng Xi, Han Xia, Tao Gui, Qi Zhang, and Xuanjing Huang. *arXiv preprint arXiv:2402.16431 2024*

- Correcting Language Model Bias for Text Classification in True Zero-Shot Learning.
  [pdf](https://aclanthology.org/2024.lrec-main.359.pdf)
    - Feng Zhao, Wan Xianlin, Cheng Yan, and Chu Kiong Loo. *LREC-COLING 2024*

- Detecting Cybercrimes in Accordance with Pakistani Law: Dataset and Evaluation Using PLMs.
  [pdf](https://aclanthology.org/2024.lrec-main.422.pdf)
    - Faizad Ullah, Ali Faheem, Ubaid Azam, Muhammad Sohaib Ayub, Faisal Kamiran, and Asim Karim. *Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024) 2024*

 - How Do In-Context Examples Affect Compositional Generalization?.
    [pdf](https://aclanthology.org/2023.acl-long.618.pdf)
    - Shengnan An, Zeqi Lin, Qiang Fu, Bei Chen, Nanning Zheng, Jian-Guang Lou, and Dongmei Zhang. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - MAGNIFICo: Evaluating the In-Context Learning Ability of Large Language Models to Generalize to Novel Interpretations.
    [pdf](https://aclanthology.org/2023.emnlp-main.134.pdf)
    - Arkil Patel, Satwik Bhattamishra, Siva Reddy, and Dzmitry Bahdanau. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - How Do In-Context Examples Affect Compositional Generalization?.
    [pdf](https://aclanthology.org/2023.acl-long.618.pdf)
    - Shengnan An, Zeqi Lin, Qiang Fu, Bei Chen, Nanning Zheng, Jian-Guang Lou, and Dongmei Zhang. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - MAGNIFICo: Evaluating the In-Context Learning Ability of Large Language Models to Generalize to Novel Interpretations.
    [pdf](https://aclanthology.org/2023.emnlp-main.134.pdf)
    - Arkil Patel, Satwik Bhattamishra, Siva Reddy, and Dzmitry Bahdanau. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Augmentation-Adapted Retriever Improves Generalization of Language Models as Generic Plug-In.
    [pdf](https://arxiv.org/pdf/2305.17331)
    - Zichun Yu, Chenyan Xiong, Shi Yu, and Zhiyuan Liu. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - HINT: Hypernetwork Instruction Tuning for Efficient Zero-and Few-Shot Generalisation.
    [pdf](https://arxiv.org/pdf/2212.10315)
    - Hamish Ivison, Akshita Bhagia, Yizhong Wang, Hannaneh Hajishirzi, and Matthew E Peters. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - InstructDial: Improving Zero and Few-shot Generalization in Dialogue through Instruction Tuning.
    [pdf](https://arxiv.org/pdf/2205.12673)
    - Prakhar Gupta, Cathy Jiao, Yi-Ting Yeh, Shikib Mehri, Maxine Eskenazi, and Jeffrey P Bigham. *Proceedings of the 2022 Conference on Empirical Methods in Natural Language Processing 2022*

 - The curious case of hallucinatory (un) answerability: Finding truths in the hidden states of over-confident large language models.
    [pdf](https://arxiv.org/pdf/2310.11877)
    - Aviv Slobodkin, Omer Goldman, Avi Caciularu, Ido Dagan, and Shauli Ravfogel. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - DoLa: Decoding by Contrasting Layers Improves Factuality in Large Language Models.
    [pdf](https://arxiv.org/pdf/2309.03883)
    - Yung-Sung Chuang, Yujia Xie, Hongyin Luo, Yoon Kim, James R. Glass, and Pengcheng He. *The Twelfth International Conference on Learning Representations 2024*

 - Teaching Language Models to Hallucinate Less with Synthetic Tasks.
    [pdf](https://arxiv.org/pdf/2310.06827)
    - Erik Jones, Hamid Palangi, Clarisse Simoes Ribeiro, Varun Chandrasekaran, Subhabrata Mukherjee, Arindam Mitra, Ahmed Hassan Awadallah, and Ece Kamar. *The Twelfth International Conference on Learning Representations 2024*

 - Mitigating large language model hallucinations via autonomous knowledge graph-based retrofitting.
    [pdf](https://arxiv.org/pdf/2311.13314)
    - Xinyan Guan, Yanjiang Liu, Hongyu Lin, Yaojie Lu, Ben He, Xianpei Han, and Le Sun. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Fine-Tuning Language Models for Factuality.
    [pdf](https://arxiv.org/pdf/2311.08401)
    - Katherine Tian, Eric Mitchell, Huaxiu Yao, Christopher D Manning, and Chelsea Finn. *The Twelfth International Conference on Learning Representations 2024*

 - Ontofact: Unveiling fantastic fact-skeleton of llms via ontology-driven reinforcement learning.
    [pdf](https://openreview.net/pdf?id=Kl2RwSP6bS)
    - Ziyu Shang, Wenjun Ke, Nana Xiu, Peng Wang, Jiajun Liu, Yanhui Li, Zhizhao Luo, and Ke Ji. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Enhancing job recommendation through llm-based generative adversarial networks.
    [pdf](https://arxiv.org/pdf/2307.10747)
    - Yingpeng Du, Di Luo, Rui Yan, Xiaopei Wang, Hongzhi Liu, Hengshu Zhu, Yang Song, and Jie Zhang. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Detecting and preventing hallucinations in large vision language models.
    [pdf](https://arxiv.org/pdf/2308.06394)
    - Anisha Gunjal, Jihan Yin, and Erhan Bas. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Analyzing and Mitigating Object Hallucination in Large Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2310.00754)
    - Yiyang Zhou, Chenhang Cui, Jaehong Yoon, Linjun Zhang, Zhun Deng, Chelsea Finn, Mohit Bansal, and Huaxiu Yao. *The Twelfth International Conference on Learning Representations 2024*

 - Mitigating Object Hallucinations in Large Vision-Language Models through Visual Contrastive Decoding.
    [pdf](https://arxiv.org/pdf/2311.16922)
    - Sicong Leng, Hang Zhang, Guanzheng Chen, Xin Li, Shijian Lu, Chunyan Miao, and Lidong Bing. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - VISTA-LLAMA: Reducing Hallucination in Video Language Models via Equal Distance to Visual Tokens.
    [pdf](https://arxiv.org/pdf/2312.08870)
    - Fan Ma, Xiaojie Jin, Heng Wang, Yuchen Xian, Jiashi Feng, and Yi Yang. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - Evaluating Object Hallucination in Large Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2305.10355)
    - Yifan Li, Yifan Du, Kun Zhou, Jinpeng Wang, Wayne Xin Zhao, and Ji-Rong Wen. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Detecting and preventing hallucinations in large vision language models.
    [pdf](https://arxiv.org/pdf/2308.06394)
    - Anisha Gunjal, Jihan Yin, and Erhan Bas. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Hallucination Augmented Contrastive Learning for Multimodal Large Language Model.
    [pdf](https://arxiv.org/pdf/2312.06968)
    - Chaoya Jiang, Haiyang Xu, Mengfan Dong, Jiaxing Chen, Wei Ye, Ming Yan, Qinghao Ye, Ji Zhang, Fei Huang, and Shikun Zhang. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - RAPPER: Reinforced Rationale-Prompted Paradigm for Natural Language Explanation in Visual Question Answering.
    [pdf](https://openreview.net/pdf?id=bshfchPM9H)
    - Kai-Po Chang, Chi-Pin Huang, Wei-Yuan Cheng, Fu-En Yang, Chien-Yi Wang, Yung-Hsuan Lai, and Yu-Chiang Frank Wang. *The Twelfth International Conference on Learning Representations 2024*

 - OPERA: Alleviating Hallucination in Multi-Modal Large Language Models via Over-Trust Penalty and Retrospection-Allocation.
    [pdf](https://arxiv.org/pdf/2311.17911)
    - Qidong Huang, Xiaoyi Dong, Pan Zhang, Bin Wang, Conghui He, Jiaqi Wang, Dahua Lin, Weiming Zhang, and Nenghai Yu. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - RLHF-V: Towards Trustworthy MLLMs via Behavior Alignment from Fine-grained Correctional Human Feedback.
    [pdf](https://arxiv.org/pdf/2312.00849)
    - Tianyu Yu, Yuan Yao, Haoye Zhang, Taiwen He, Yifeng Han, Ganqu Cui, Jinyi Hu, Zhiyuan Liu, Hai-Tao Zheng, Maosong Sun, and Tat-Seng Chua. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

- Identifying and mitigating spurious correlations for improving robustness in nlp models.
  [pdf](https://aclanthology.org/2022.findings-naacl.130.pdf)
    - Tianlu Wang, Rohit Sridhar, Diyi Yang, and Xuezhi Wang. *arXiv preprint arXiv:2110.07736 2021*

 - A Cause-Effect Look at Alleviating Hallucination of Knowledge-grounded Dialogue Generation.
    [pdf](https://arxiv.org/pdf/2404.03491)
    - Jifan Yu, Xiaohan Zhang, Yifan Xu, Xuanyu Lei, Zijun Yao, Jing Zhang, Lei Hou, and Juanzi Li. *arXiv preprint arXiv:2404.03491 2024*

 - Teaching Language Models to Hallucinate Less with Synthetic Tasks.
    [pdf](https://arxiv.org/pdf/2310.06827)
    - Erik Jones, Hamid Palangi, Clarisse Simoes Ribeiro, Varun Chandrasekaran, Subhabrata Mukherjee, Arindam Mitra, Ahmed Hassan Awadallah, and Ece Kamar. *The Twelfth International Conference on Learning Representations 2024*

 - Analyzing and Mitigating Object Hallucination in Large Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2310.00754)
    - Yiyang Zhou, Chenhang Cui, Jaehong Yoon, Linjun Zhang, Zhun Deng, Chelsea Finn, Mohit Bansal, and Huaxiu Yao. *The Twelfth International Conference on Learning Representations 2024*

 - DoLa: Decoding by Contrasting Layers Improves Factuality in Large Language Models.
    [pdf](https://arxiv.org/pdf/2309.03883)
    - Yung-Sung Chuang, Yujia Xie, Hongyin Luo, Yoon Kim, James R. Glass, and Pengcheng He. *The Twelfth International Conference on Learning Representations 2024*

 - Fine-Tuning Language Models for Factuality.
    [pdf](https://arxiv.org/pdf/2311.08401)
    - Katherine Tian, Eric Mitchell, Huaxiu Yao, Christopher D Manning, and Chelsea Finn. *The Twelfth International Conference on Learning Representations 2024*

 - Attention Satisfies: A Constraint-Satisfaction Lens on Factual Errors of Language Models.
    [pdf](https://arxiv.org/pdf/2309.15098)
    - Mert Yuksekgonul, Varun Chandrasekaran, Erik Jones, Suriya Gunasekar, Ranjita Naik, Hamid Palangi, Ece Kamar, and Besmira Nushi. *The Twelfth International Conference on Learning Representations 2024*

 - RAPPER: Reinforced Rationale-Prompted Paradigm for Natural Language Explanation in Visual Question Answering.
    [pdf](https://openreview.net/pdf?id=bshfchPM9H)
    - Kai-Po Chang, Chi-Pin Huang, Wei-Yuan Cheng, Fu-En Yang, Chien-Yi Wang, Yung-Hsuan Lai, and Yu-Chiang Frank Wang. *The Twelfth International Conference on Learning Representations 2024*

 - Hallucination Augmented Contrastive Learning for Multimodal Large Language Model.
    [pdf](https://arxiv.org/pdf/2312.06968)
    - Chaoya Jiang, Haiyang Xu, Mengfan Dong, Jiaxing Chen, Wei Ye, Ming Yan, Qinghao Ye, Ji Zhang, Fei Huang, and Shikun Zhang. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - Mitigating Object Hallucinations in Large Vision-Language Models through Visual Contrastive Decoding.
    [pdf](https://arxiv.org/pdf/2311.16922)
    - Sicong Leng, Hang Zhang, Guanzheng Chen, Xin Li, Shijian Lu, Chunyan Miao, and Lidong Bing. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - OPERA: Alleviating Hallucination in Multi-Modal Large Language Models via Over-Trust Penalty and Retrospection-Allocation.
    [pdf](https://arxiv.org/pdf/2311.17911)
    - Qidong Huang, Xiaoyi Dong, Pan Zhang, Bin Wang, Conghui He, Jiaqi Wang, Dahua Lin, Weiming Zhang, and Nenghai Yu. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - VISTA-LLAMA: Reducing Hallucination in Video Language Models via Equal Distance to Visual Tokens.
    [pdf](https://arxiv.org/pdf/2312.08870)
    - Fan Ma, Xiaojie Jin, Heng Wang, Yuchen Xian, Jiashi Feng, and Yi Yang. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - RLHF-V: Towards Trustworthy MLLMs via Behavior Alignment from Fine-grained Correctional Human Feedback.
    [pdf](https://arxiv.org/pdf/2312.00849)
    - Tianyu Yu, Yuan Yao, Haoye Zhang, Taiwen He, Yifeng Han, Ganqu Cui, Jinyi Hu, Zhiyuan Liu, Hai-Tao Zheng, Maosong Sun, and Tat-Seng Chua. *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024*

 - Enhancing job recommendation through llm-based generative adversarial networks.
    [pdf](https://arxiv.org/pdf/2307.10747)
    - Yingpeng Du, Di Luo, Rui Yan, Xiaopei Wang, Hongzhi Liu, Hengshu Zhu, Yang Song, and Jie Zhang. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Ontofact: Unveiling fantastic fact-skeleton of llms via ontology-driven reinforcement learning.
    [pdf](https://openreview.net/pdf?id=Kl2RwSP6bS)
    - Ziyu Shang, Wenjun Ke, Nana Xiu, Peng Wang, Jiajun Liu, Yanhui Li, Zhizhao Luo, and Ke Ji. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Mitigating large language model hallucinations via autonomous knowledge graph-based retrofitting.
    [pdf](https://arxiv.org/pdf/2311.13314)
    - Xinyan Guan, Yanjiang Liu, Hongyu Lin, Yaojie Lu, Ben He, Xianpei Han, and Le Sun. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Detecting and preventing hallucinations in large vision language models.
    [pdf](https://arxiv.org/pdf/2308.06394)
    - Anisha Gunjal, Jihan Yin, and Erhan Bas. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - A Cause-Effect Look at Alleviating Hallucination of Knowledge-grounded Dialogue Generation.
    [pdf](https://arxiv.org/pdf/2404.03491)
    - Jifan Yu, Xiaohan Zhang, Yifan Xu, Xuanyu Lei, Zijun Yao, Jing Zhang, Lei Hou, and Juanzi Li. *arXiv preprint arXiv:2404.03491 2024*

- Identifying and mitigating spurious correlations for improving robustness in nlp models.
  [pdf](https://aclanthology.org/2022.findings-naacl.130.pdf)
    - Tianlu Wang, Rohit Sridhar, Diyi Yang, and Xuezhi Wang. *arXiv preprint arXiv:2110.07736 2021*

 - Evaluating Object Hallucination in Large Vision-Language Models.
    [pdf](https://arxiv.org/pdf/2305.10355)
    - Yifan Li, Yifan Du, Kun Zhou, Jinpeng Wang, Wayne Xin Zhao, and Ji-Rong Wen. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - The curious case of hallucinatory (un) answerability: Finding truths in the hidden states of over-confident large language models.
    [pdf](https://arxiv.org/pdf/2310.11877)
    - Aviv Slobodkin, Omer Goldman, Avi Caciularu, Ido Dagan, and Shauli Ravfogel. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - UniSumm and SummZoo: Unified Model and Diverse Benchmark for Few-Shot Summarization.
    [pdf](https://aclanthology.org/2023.acl-long.718.pdf)
    - Yulong Chen, Yang Liu, Ruochen Xu, Ziyi Yang, Chenguang Zhu, Michael Zeng, and Yue Zhang. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - Do LLMs Understand Social Knowledge? Evaluating the Sociability of Large Language Models with SocKET Benchmark.
    [pdf](https://arxiv.org/pdf/2305.14938)
    - Minje Choi, Jiaxin Pei, Sagar Kumar, Chang Shu, and David Jurgens. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

## Robustness Evaluation
<!-- table -->
 - Promptbench: Towards evaluating the robustness of large language models on adversarial prompts.
    [pdf](https://arxiv.org/pdf/2306.04528)
    - Kaijie Zhu, Jindong Wang, Jiaheng Zhou, Zichen Wang, Hao Chen, Yidong Wang, Linyi Yang, Wei Ye, Yue Zhang, Neil Zhenqiang Gong, and others. *arXiv preprint arXiv:2306.04528 2023*

 - Evaluating commonsense in pre-trained language models.
    [pdf](https://arxiv.org/pdf/1911.11931)
    - Xuhui Zhou, Yue Zhang, Leyang Cui, and Dandan Huang. *Proceedings of the AAAI conference on artificial intelligence 2020*

 - Benchmarking Hallucination in Large Language Models based on Unanswerable Math Word Problem.
    [pdf](https://arxiv.org/pdf/2403.03558)
    - Yuhong Sun, Zhangyue Yin, Qipeng Guo, Jiawen Wu, Xipeng Qiu, and Hui Zhao. *arXiv preprint arXiv:2403.03558 2024*

 - Writing your own book: A method for going from closed to open book QA to improve robustness and performance of smaller LLMs.
    [pdf](https://arxiv.org/pdf/2305.11334)
    - Giorgi Kokaia, Pratyush Sinha, Yutong Jiang, and Nozha Boujemaa. *arXiv preprint arXiv:2305.11334 2023*

 - Robustification of multilingual language models to real-world noise in crosslingual zero-shot settings with robust contrastive pretraining.
    [pdf](https://arxiv.org/pdf/2210.04782)
    - Asa Cooper Stickland, Sailik Sengupta, Jason Krone, Saab Mansour, and He He. *arXiv preprint arXiv:2210.04782 2022*

 - Can LLM Replace Stack Overflow? A Study on Robustness and Reliability of Large Language Model Code Generation.
    [pdf](https://arxiv.org/pdf/2308.10335v5)
    - Li Zhong and Zilong Wang. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - RobuT: A Systematic Study of Table QA Robustness Against Human-Annotated Adversarial Perturbations.
    [pdf](https://arxiv.org/pdf/2306.14321)
    - Yilun Zhao, Chen Zhao, Linyong Nan, Zhenting Qi, Wenlin Zhang, Xiangru Tang, Boyu Mi, and Dragomir Radev. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*
<!-- table -->


### Dataset Construction
<!-- dataset -->
 - Evaluating commonsense in pre-trained language models.
    [pdf](https://arxiv.org/pdf/1911.11931)
    - Xuhui Zhou, Yue Zhang, Leyang Cui, and Dandan Huang. *Proceedings of the AAAI conference on artificial intelligence 2020*

 - Benchmarking Hallucination in Large Language Models based on Unanswerable Math Word Problem.
    [pdf](https://arxiv.org/pdf/2403.03558)
    - Yuhong Sun, Zhangyue Yin, Qipeng Guo, Jiawen Wu, Xipeng Qiu, and Hui Zhao. *arXiv preprint arXiv:2403.03558 2024*

 - Writing your own book: A method for going from closed to open book QA to improve robustness and performance of smaller LLMs.
    [pdf](https://arxiv.org/pdf/2305.11334)
    - Giorgi Kokaia, Pratyush Sinha, Yutong Jiang, and Nozha Boujemaa. *arXiv preprint arXiv:2305.11334 2023*

 - Robustification of multilingual language models to real-world noise in crosslingual zero-shot settings with robust contrastive pretraining.
    [pdf](https://arxiv.org/pdf/2210.04782)
    - Asa Cooper Stickland, Sailik Sengupta, Jason Krone, Saab Mansour, and He He. *arXiv preprint arXiv:2210.04782 2022*

 - End-to-end slot alignment and recognition for cross-lingual NLU.
    [pdf](https://arxiv.org/pdf/2004.14353v1)
    - Weijia Xu, Batool Haider, and Saab Mansour. *arXiv preprint arXiv:2004.14353 2020*

 - Cross-lingual name tagging and linking for 282 languages.
    [pdf](https://aclanthology.org/P17-1178.pdf)
    - Xiaoman Pan, Boliang Zhang, Jonathan May, Joel Nothman, Kevin Knight, and Heng Ji. *Proceedings of the 55th annual meeting of the association for computational linguistics (volume 1: long papers) 2017*

 - XNLI: Evaluating cross-lingual sentence representations.
    [pdf](https://arxiv.org/pdf/1809.05053)
    - Alexis Conneau, Guillaume Lample, Ruty Rinott, Adina Williams, Samuel R Bowman, Holger Schwenk, and Veselin Stoyanov. *arXiv preprint arXiv:1809.05053 2018*

 - End-to-end slot alignment and recognition for cross-lingual NLU.
    [pdf](https://arxiv.org/pdf/2004.14353v1)
    - Weijia Xu, Batool Haider, and Saab Mansour. *arXiv preprint arXiv:2004.14353 2020*

 - Cross-lingual name tagging and linking for 282 languages.
    [pdf](https://aclanthology.org/P17-1178.pdf)
    - Xiaoman Pan, Boliang Zhang, Jonathan May, Joel Nothman, Kevin Knight, and Heng Ji. *Proceedings of the 55th annual meeting of the association for computational linguistics (volume 1: long papers) 2017*

 - XNLI: Evaluating cross-lingual sentence representations.
    [pdf](https://arxiv.org/pdf/1809.05053)
    - Alexis Conneau, Guillaume Lample, Ruty Rinott, Adina Williams, Samuel R Bowman, Holger Schwenk, and Veselin Stoyanov. *arXiv preprint arXiv:1809.05053 2018*

 - Can LLM Replace Stack Overflow? A Study on Robustness and Reliability of Large Language Model Code Generation.
    [pdf](https://arxiv.org/pdf/2308.10335v5)
    - Li Zhong and Zilong Wang. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Exploring the robustness of large language models for solving programming problems.
    [pdf](https://arxiv.org/pdf/2306.14583)
    - Atsushi Shirafuji, Yutaka Watanobe, Takumi Ito, Makoto Morishita, Yuki Nakamura, Yusuke Oda, and Jun Suzuki. *arXiv preprint arXiv:2306.14583 2023*

 - RobuT: A Systematic Study of Table QA Robustness Against Human-Annotated Adversarial Perturbations.
    [pdf](https://arxiv.org/pdf/2306.14321)
    - Yilun Zhao, Chen Zhao, Linyong Nan, Zhenting Qi, Wenlin Zhang, Xiangru Tang, Boyu Mi, and Dragomir Radev. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - Compositional semantic parsing on semi-structured tables.
    [pdf](https://arxiv.org/pdf/1508.00305)
    - Panupong Pasupat and Percy Liang. *arXiv preprint arXiv:1508.00305 2015*

 - Seq2sql: Generating structured queries from natural language using reinforcement learning.
    [pdf](https://arxiv.org/pdf/1709.00103)
    - Victor Zhong, Caiming Xiong, and Richard Socher. *arXiv preprint arXiv:1709.00103 2017*

 - Search-based neural structured learning for sequential question answering.
    [pdf](https://aclanthology.org/P17-1167.pdf)
    - Mohit Iyyer, Wen-tau Yih, and Ming-Wei Chang. *Proceedings of the 55th Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2017*

 - Is ChatGPT a good translator? A preliminary study.
    [pdf](https://arxiv.org/pdf/2301.08745)
    - Wenxiang Jiao, Wenxuan Wang, Jen-tse Huang, Xing Wang, and Zhaopeng Tu. *arXiv preprint arXiv:2301.08745 2023*

 - ToxiGen: A Large-Scale Machine-Generated Dataset for Adversarial and Implicit Hate Speech Detection.
    [pdf](https://arxiv.org/pdf/2203.09509)
    - Thomas Hartvigsen, Saadia Gabriel, Hamid Palangi, Maarten Sap, Dipankar Ray, and Ece Kamar. *Proceedings of the 60th Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2022*

 - Benchmarking large language models in retrieval-augmented generation.
    [pdf](https://arxiv.org/pdf/2309.01431)
    - Jiawei Chen, Hongyu Lin, Xianpei Han, and Le Sun. *arXiv preprint arXiv:2309.01431 Unknown Year*

 - Can LLM Replace Stack Overflow? A Study on Robustness and Reliability of Large Language Model Code Generation.
    [pdf](https://arxiv.org/pdf/2308.10335v5)
    - Li Zhong and Zilong Wang. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Benchmarking large language models in retrieval-augmented generation.
    [pdf](https://arxiv.org/pdf/2309.01431)
    - Jiawei Chen, Hongyu Lin, Xianpei Han, and Le Sun. *arXiv preprint arXiv:2309.01431 Unknown Year*

 - Evaluating commonsense in pre-trained language models.
    [pdf](https://arxiv.org/pdf/1911.11931)
    - Xuhui Zhou, Yue Zhang, Leyang Cui, and Dandan Huang. *Proceedings of the AAAI conference on artificial intelligence 2020*

 - Recognizing Value Resonance with Resonance-Tuned RoBERTa Task Definition, Experimental Validation, and Robust Modeling.
    [pdf](https://aclanthology.org/2024.lrec-main.1195.pdf)
    - Noam K Benkler, Scott Friedman, Sonja Schmer-Galunder, Drisana Marissa Mosaphir, Robert P Goldman, Ruta Wheelock, Vasanth Sarathy, Pavan Kantharaju, and Matthew D McLure. *Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024) 2024*

 - Cultural value resonance in folktales: A transformer-based analysis with the world value corpus.
    [pdf](https://openreview.net/forum?id=FNNMeNDaU7)
    - Noam Benkler, Scott Friedman, Sonja Schmer-Galunder, Drisana Mosaphir, Vasanth Sarathy, Pavan Kantharaju, Matthew D McLure, and Robert P Goldman. *International Conference on Social Computing, Behavioral-Cultural Modeling and Prediction and Behavior Representation in Modeling and Simulation 2022*

 - Benchmarking Hallucination in Large Language Models based on Unanswerable Math Word Problem.
    [pdf](https://arxiv.org/pdf/2403.03558)
    - Yuhong Sun, Zhangyue Yin, Qipeng Guo, Jiawen Wu, Xipeng Qiu, and Hui Zhao. *arXiv preprint arXiv:2403.03558 2024*

 - Is ChatGPT a good translator? A preliminary study.
    [pdf](https://arxiv.org/pdf/2301.08745)
    - Wenxiang Jiao, Wenxuan Wang, Jen-tse Huang, Xing Wang, and Zhaopeng Tu. *arXiv preprint arXiv:2301.08745 2023*

 - Findings of the WMT 2019 biomedical translation shared task: Evaluation for MEDLINE abstracts and biomedical terminologies.
    [pdf](https://aclanthology.org/W19-5403.pdf)
    - Rachel Bawden, Kevin Bretonnel Cohen, Cristian Grozea, Antonio Jimeno Yepes, Madeleine Kittner, Martin Krallinger, Nancy Mah, Aurelie Neveol, Mariana Neves, Felipe Soares, and others. *ACL 2019 Fourth Conference on Machine Translation 2019*

 - Findings of the WMT 2020 shared task on machine translation robustness.
    [pdf](https://aclanthology.org/2020.wmt-1.4.pdf)
    - Lucia Specia, Zhenhao Li, Juan Pino, Vishrav Chaudhary, Francisco Guzman, Graham Neubig, Nadir Durrani, Yonatan Belinkov, Philipp Koehn, Hassan Sajjad, and others. *Proceedings of the Fifth Conference on Machine Translation 2020*

 - Writing your own book: A method for going from closed to open book QA to improve robustness and performance of smaller LLMs.
    [pdf](https://arxiv.org/pdf/2305.11334)
    - Giorgi Kokaia, Pratyush Sinha, Yutong Jiang, and Nozha Boujemaa. *arXiv preprint arXiv:2305.11334 2023*

 - RobuT: A Systematic Study of Table QA Robustness Against Human-Annotated Adversarial Perturbations.
    [pdf](https://arxiv.org/pdf/2306.14321)
    - Yilun Zhao, Chen Zhao, Linyong Nan, Zhenting Qi, Wenlin Zhang, Xiangru Tang, Boyu Mi, and Dragomir Radev. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - Compositional semantic parsing on semi-structured tables.
    [pdf](https://arxiv.org/pdf/1508.00305)
    - Panupong Pasupat and Percy Liang. *arXiv preprint arXiv:1508.00305 2015*

 - Seq2sql: Generating structured queries from natural language using reinforcement learning.
    [pdf](https://arxiv.org/pdf/1709.00103)
    - Victor Zhong, Caiming Xiong, and Richard Socher. *arXiv preprint arXiv:1709.00103 2017*

 - Search-based neural structured learning for sequential question answering.
    [pdf](https://aclanthology.org/P17-1167.pdf)
    - Mohit Iyyer, Wen-tau Yih, and Ming-Wei Chang. *Proceedings of the 55th Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2017*

 - Exploring the robustness of large language models for solving programming problems.
    [pdf](https://arxiv.org/pdf/2306.14583)
    - Atsushi Shirafuji, Yutaka Watanobe, Takumi Ito, Makoto Morishita, Yuki Nakamura, Yusuke Oda, and Jun Suzuki. *arXiv preprint arXiv:2306.14583 2023*

 - Robustification of multilingual language models to real-world noise in crosslingual zero-shot settings with robust contrastive pretraining.
    [pdf](https://arxiv.org/pdf/2210.04782)
    - Asa Cooper Stickland, Sailik Sengupta, Jason Krone, Saab Mansour, and He He. *arXiv preprint arXiv:2210.04782 2022*

 - End-to-end slot alignment and recognition for cross-lingual NLU.
    [pdf](https://arxiv.org/pdf/2004.14353v1)
    - Weijia Xu, Batool Haider, and Saab Mansour. *arXiv preprint arXiv:2004.14353 2020*

 - Cross-lingual name tagging and linking for 282 languages.
    [pdf](https://aclanthology.org/P17-1178.pdf)
    - Xiaoman Pan, Boliang Zhang, Jonathan May, Joel Nothman, Kevin Knight, and Heng Ji. *Proceedings of the 55th annual meeting of the association for computational linguistics (volume 1: long papers) 2017*

 - XNLI: Evaluating cross-lingual sentence representations.
    [pdf](https://arxiv.org/pdf/1809.05053)
    - Alexis Conneau, Guillaume Lample, Ruty Rinott, Adina Williams, Samuel R Bowman, Holger Schwenk, and Veselin Stoyanov. *arXiv preprint arXiv:1809.05053 2018*

 - ToxiGen: A Large-Scale Machine-Generated Dataset for Adversarial and Implicit Hate Speech Detection.
    [pdf](https://arxiv.org/pdf/2203.09509)
    - Thomas Hartvigsen, Saadia Gabriel, Hamid Palangi, Maarten Sap, Dipankar Ray, and Ece Kamar. *Proceedings of the 60th Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2022*

<!-- dataset -->


### Robustness Evaluation
 - Promptbench: Towards evaluating the robustness of large language models on adversarial prompts.
    [pdf](https://arxiv.org/pdf/2306.04528)
    - Kaijie Zhu, Jindong Wang, Jiaheng Zhou, Zichen Wang, Hao Chen, Yidong Wang, Linyi Yang, Wei Ye, Yue Zhang, Neil Zhenqiang Gong, and others. *arXiv preprint arXiv:2306.04528 2023*

 - Trustworthy LLMs: A survey and guideline for evaluating large language models' alignment.
    [pdf](https://arxiv.org/abs/2404.14294)
    - Yang Liu, Yuanshun Yao, Jean-Francois Ton, Xiaoying Zhang, Ruocheng Guo Hao Cheng, Yegor Klochkov, Muhammad Faaiz Taufiq, and Hang Li. *arXiv preprint arXiv:2308.05374 2023*

 - On Robustness-Accuracy Characterization of Large Language Models using Synthetic Datasets.
    [pdf](https://openreview.net/pdf?id=6iM2asNCjK)
    - Ching-Yun Ko, Pin-Yu Chen, Payel Das, Yung-Sung Chuang, and Luca Daniel. *Unknown Venue 2023*

 - Revisiting the Self-Consistency Challenges in Multi-Choice Question Formats for Large Language Model Evaluation.
    [pdf](https://aclanthology.org/2024.lrec-main.1229.pdf)
    - Wenjie Zhou, Qiang Wang, Mingzhou Xu, Ming Chen, and Xiangyu Duan. *Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024) 2024*

 - Bamboo: A comprehensive benchmark for evaluating long text modeling capacities of large language models.
    [pdf](https://arxiv.org/pdf/2309.13345)
    - Zican Dong, Tianyi Tang, Junyi Li, Wayne Xin Zhao, and Ji-Rong Wen. *arXiv preprint arXiv:2309.13345 2023*

 - Revisiting non-English Text Simplification: A Unified Multilingual Benchmark.
    [pdf](https://arxiv.org/pdf/2305.15678)
    - Michael Ryan, Tarek Naous, and Wei Xu. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - Promptbench: Towards evaluating the robustness of large language models on adversarial prompts.
    [pdf](https://arxiv.org/pdf/2306.04528)
    - Kaijie Zhu, Jindong Wang, Jiaheng Zhou, Zichen Wang, Hao Chen, Yidong Wang, Linyi Yang, Wei Ye, Yue Zhang, Neil Zhenqiang Gong, and others. *arXiv preprint arXiv:2306.04528 2023*

 - On Robustness-Accuracy Characterization of Large Language Models using Synthetic Datasets.
    [pdf](https://openreview.net/pdf?id=6iM2asNCjK)
    - Ching-Yun Ko, Pin-Yu Chen, Payel Das, Yung-Sung Chuang, and Luca Daniel. *Unknown Venue 2023*

 - Revisiting the Self-Consistency Challenges in Multi-Choice Question Formats for Large Language Model Evaluation.
    [pdf](https://aclanthology.org/2024.lrec-main.1229.pdf)
    - Wenjie Zhou, Qiang Wang, Mingzhou Xu, Ming Chen, and Xiangyu Duan. *Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024) 2024*

 - Bamboo: A comprehensive benchmark for evaluating long text modeling capacities of large language models.
    [pdf](https://arxiv.org/pdf/2309.13345)
    - Zican Dong, Tianyi Tang, Junyi Li, Wayne Xin Zhao, and Ji-Rong Wen. *arXiv preprint arXiv:2309.13345 2023*

 - Revisiting non-English Text Simplification: A Unified Multilingual Benchmark.
    [pdf](https://arxiv.org/pdf/2305.15678)
    - Michael Ryan, Tarek Naous, and Wei Xu. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - ROBBIE: Robust bias evaluation of large generative language models.
    [pdf](https://arxiv.org/pdf/2311.18140)
    - David Esiobu, Xiaoqing Tan, Saghar Hosseini, Megan Ung, Yuchen Zhang, Jude Fernandes, Jane Dwivedi-Yu, Eleonora Presani, Adina Williams, and Eric Smith. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - SLOG: A Structural Generalization Benchmark for Semantic Parsing.
    [pdf](https://aclanthology.org/2023.emnlp-main.194.pdf)
    - Bingzhi Li, Lucia Donatelli, Alexander Koller, Tal Linzen, Yuekun Yao, and Najoung Kim. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - RobustLR: A diagnostic benchmark for evaluating logical robustness of deductive reasoners.
    [pdf](https://aclanthology.org/2022.emnlp-main.653.pdf)
    - Soumya Sanyal, Zeyi Liao, and Xiang Ren. *Proceedings of the 2022 Conference on Empirical Methods in Natural Language Processing 2022*

 - Have LLMs Advanced Enough? A Challenging Problem Solving Benchmark For Large Language Models.
    [pdf](https://arxiv.org/pdf/2305.15074)
    - Daman Arora, Himanshu Singh, and others. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - SafeText: A Benchmark for Exploring Physical Safety in Language Models.
    [pdf](https://arxiv.org/pdf/2210.10045)
    - Sharon Levy, Emily Allaway, Melanie Subbiah, Lydia Chilton, Desmond Patton, Kathleen Mckeown, and William Yang Wang. *Proceedings of the 2022 Conference on Empirical Methods in Natural Language Processing 2022*

 - A causal framework to quantify the robustness of mathematical reasoning with language models.
    [pdf](https://aclanthology.org/2023.acl-long.32.pdf)
    - Alessandro Stolfo, Zhijing Jin, Kumar Shridhar, Bernhard Scholkopf, and Mrinmaya Sachan. *arXiv preprint arXiv:2210.12023 2022*

 - Cladder: Assessing causal reasoning in language models.
    [pdf](https://arxiv.org/pdf/2312.04350)
    - Zhijing Jin, Yuen Chen, Felix Leeb, Luigi Gresele, Ojasv Kamal, LYU Zhiheng, Kevin Blin, Fernando Gonzalez Adauto, Max Kleiman-Weiner, Mrinmaya Sachan, and others. *Thirty-seventh conference on neural information processing systems 2023*

 - Recode: Robustness evaluation of code generation models.
    [pdf](https://aclanthology.org/2023.acl-long.773.pdf)
    - Shiqi Wang, Zheng Li, Haifeng Qian, Chenghao Yang, Zijian Wang, Mingyue Shang, Varun Kumar, Samson Tan, Baishakhi Ray, Parminder Bhatia, and others. *arXiv preprint arXiv:2212.10264 2022*

 - White-box multi-objective adversarial attack on dialogue generation.
    [pdf](https://aclanthology.org/2023.acl-long.100.pdf)
    - Yufei Li, Zexin Li, Yingfan Gao, and Cong Liu. *arXiv preprint arXiv:2305.03655 2023*

 - MedEval: A Multi-Level, Multi-Task, and Multi-Domain Medical Benchmark for Language Model Evaluation.
    [pdf](https://aclanthology.org/2023.emnlp-main.540.pdf)
    - Zexue He, Yu Wang, An Yan, Yao Liu, Eric Chang, Amilcare Gentili, Julian McAuley, and Chun-nan Hsu. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Benchmarking Hallucination in Large Language Models based on Unanswerable Math Word Problem.
    [pdf](https://arxiv.org/pdf/2403.03558)
    - Yuhong Sun, Zhangyue Yin, Qipeng Guo, Jiawen Wu, Xipeng Qiu, and Hui Zhao. *arXiv preprint arXiv:2403.03558 2024*

 - SCITAB: A Challenging Benchmark for Compositional Reasoning and Claim Verification on Scientific Tables.
    [pdf](https://aclanthology.org/2023.emnlp-main.483.pdf)
    - Xinyuan Lu, Liangming Pan, Qian Liu, Preslav Nakov, and Min-Yen Kan. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - RobuT: A Systematic Study of Table QA Robustness Against Human-Annotated Adversarial Perturbations.
    [pdf](https://arxiv.org/pdf/2306.14321)
    - Yilun Zhao, Chen Zhao, Linyong Nan, Zhenting Qi, Wenlin Zhang, Xiangru Tang, Boyu Mi, and Dragomir Radev. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - NLPositionality: Characterizing Design Biases of Datasets and Models.
    [pdf](https://aclanthology.org/2023.acl-long.505v2.pdf)
    - Sebastin Santy, Jenny T Liang, Ronan Le Bras, Katharina Reinecke, and Maarten Sap. *The 61st Annual Meeting Of The Association For Computational Linguistics 2023*

 - WinoQueer: A Community-in-the-Loop Benchmark for Anti-LGBTQ+ Bias in Large Language Models.
    [pdf](https://aclanthology.org/2023.acl-long.507v3.pdf)
    - Virginia Felkner, Ho-Chun Herbert Chang, Eugene Jang, and Jonathan May. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - SeeGULL: A Stereotype Benchmark with Broad Geo-Cultural Coverage Leveraging Generative Models.
    [pdf](https://arxiv.org/pdf/2305.11840)
    - Akshita Jha, Aida Mostafazadeh Davani, Chandan K Reddy, Shachi Dave, Vinodkumar Prabhakaran, and Sunipa Dev. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - On the Challenges of Using Black-Box APIs for Toxicity Evaluation in Research.
    [pdf](https://aclanthology.org/2023.emnlp-main.472.pdf)
    - Luiza Pozzobon, Beyza Ermis, Patrick Lewis, and Sara Hooker. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - CHBias: Bias Evaluation and Mitigation of Chinese Conversational Language Models.
    [pdf](https://aclanthology.org/2023.acl-long.757.pdf)
    - Jiaxu Zhao, Meng Fang, Zijing Shi, Yitong Li, Ling Chen, and Mykola Pechenizkiy. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - Socialstigmaqa: A benchmark to uncover stigma amplification in generative language models.
    [pdf](https://arxiv.org/pdf/2312.07492)
    - Manish Nagireddy, Lamogha Chiazor, Moninder Singh, and Ioana Baldini. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - ROBBIE: Robust bias evaluation of large generative language models.
    [pdf](https://arxiv.org/pdf/2311.18140)
    - David Esiobu, Xiaoqing Tan, Saghar Hosseini, Megan Ung, Yuchen Zhang, Jude Fernandes, Jane Dwivedi-Yu, Eleonora Presani, Adina Williams, and Eric Smith. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - SLOG: A Structural Generalization Benchmark for Semantic Parsing.
    [pdf](https://aclanthology.org/2023.emnlp-main.194.pdf)
    - Bingzhi Li, Lucia Donatelli, Alexander Koller, Tal Linzen, Yuekun Yao, and Najoung Kim. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - RobustLR: A diagnostic benchmark for evaluating logical robustness of deductive reasoners.
    [pdf](https://aclanthology.org/2022.emnlp-main.653.pdf)
    - Soumya Sanyal, Zeyi Liao, and Xiang Ren. *Proceedings of the 2022 Conference on Empirical Methods in Natural Language Processing 2022*

 - Have LLMs Advanced Enough? A Challenging Problem Solving Benchmark For Large Language Models.
    [pdf](https://arxiv.org/pdf/2305.15074)
    - Daman Arora, Himanshu Singh, and others. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - SafeText: A Benchmark for Exploring Physical Safety in Language Models.
    [pdf](https://arxiv.org/pdf/2210.10045)
    - Sharon Levy, Emily Allaway, Melanie Subbiah, Lydia Chilton, Desmond Patton, Kathleen Mckeown, and William Yang Wang. *Proceedings of the 2022 Conference on Empirical Methods in Natural Language Processing 2022*

 - A causal framework to quantify the robustness of mathematical reasoning with language models.
    [pdf](https://aclanthology.org/2023.acl-long.32.pdf)
    - Alessandro Stolfo, Zhijing Jin, Kumar Shridhar, Bernhard Scholkopf, and Mrinmaya Sachan. *arXiv preprint arXiv:2210.12023 2022*

 - A diverse corpus for evaluating and developing English math word problem solvers.
    [pdf](https://arxiv.org/pdf/2106.15772)
    - Shen-Yun Miao, Chao-Chun Liang, and Keh-Yih Su. *arXiv preprint arXiv:2106.15772 2021*

 - MAWPS: A math word problem repository.
    [pdf](https://aclanthology.org/N16-1136.pdf)
    - Rik Koncel-Kedziorski, Subhro Roy, Aida Amini, Nate Kushman, and Hannaneh Hajishirzi. *Proceedings of the 2016 conference of the north american chapter of the association for computational linguistics: human language technologies 2016*

 - Are NLP models really able to solve simple math word problems?.
    [pdf](https://aclanthology.org/2021.naacl-main.168.pdf)
    - Arkil Patel, Satwik Bhattamishra, and Navin Goyal. *arXiv preprint arXiv:2103.07191 2021*

 - Cladder: Assessing causal reasoning in language models.
    [pdf](https://arxiv.org/pdf/2312.04350)
    - Zhijing Jin, Yuen Chen, Felix Leeb, Luigi Gresele, Ojasv Kamal, LYU Zhiheng, Kevin Blin, Fernando Gonzalez Adauto, Max Kleiman-Weiner, Mrinmaya Sachan, and others. *Thirty-seventh conference on neural information processing systems 2023*

 - Evaluating commonsense in pre-trained language models.
    [pdf](https://arxiv.org/pdf/1911.11931)
    - Xuhui Zhou, Yue Zhang, Leyang Cui, and Dandan Huang. *Proceedings of the AAAI conference on artificial intelligence 2020*

 - The Generalization and Robustness of Transformer-Based Language Models on Commonsense Reasoning.
    [pdf](https://ojs.aaai.org/index.php/AAAI/article/view/30410#:~:text=To%20gain%20deeper%20insight%20into%20diagnosing%20these%20models%27,framework%20for%20both%20discriminative%20and%20generative%20language%20models.)
    - Ke Shen. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Recode: Robustness evaluation of code generation models.
    [pdf](https://aclanthology.org/2023.acl-long.773.pdf)
    - Shiqi Wang, Zheng Li, Haifeng Qian, Chenghao Yang, Zijian Wang, Mingyue Shang, Varun Kumar, Samson Tan, Baishakhi Ray, Parminder Bhatia, and others. *arXiv preprint arXiv:2212.10264 2022*

 - White-box multi-objective adversarial attack on dialogue generation.
    [pdf](https://aclanthology.org/2023.acl-long.100.pdf)
    - Yufei Li, Zexin Li, Yingfan Gao, and Cong Liu. *arXiv preprint arXiv:2305.03655 2023*

 - MedEval: A Multi-Level, Multi-Task, and Multi-Domain Medical Benchmark for Language Model Evaluation.
    [pdf](https://aclanthology.org/2023.emnlp-main.540.pdf)
    - Zexue He, Yu Wang, An Yan, Yao Liu, Eric Chang, Amilcare Gentili, Julian McAuley, and Chun-nan Hsu. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - SCITAB: A Challenging Benchmark for Compositional Reasoning and Claim Verification on Scientific Tables.
    [pdf](https://aclanthology.org/2023.emnlp-main.483.pdf)
    - Xinyuan Lu, Liangming Pan, Qian Liu, Preslav Nakov, and Min-Yen Kan. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Benchmarking Hallucination in Large Language Models based on Unanswerable Math Word Problem.
    [pdf](https://arxiv.org/pdf/2403.03558)
    - Yuhong Sun, Zhangyue Yin, Qipeng Guo, Jiawen Wu, Xipeng Qiu, and Hui Zhao. *arXiv preprint arXiv:2403.03558 2024*

 - RobuT: A Systematic Study of Table QA Robustness Against Human-Annotated Adversarial Perturbations.
    [pdf](https://arxiv.org/pdf/2306.14321)
    - Yilun Zhao, Chen Zhao, Linyong Nan, Zhenting Qi, Wenlin Zhang, Xiangru Tang, Boyu Mi, and Dragomir Radev. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - NLPositionality: Characterizing Design Biases of Datasets and Models.
    [pdf](https://aclanthology.org/2023.acl-long.505v2.pdf)
    - Sebastin Santy, Jenny T Liang, Ronan Le Bras, Katharina Reinecke, and Maarten Sap. *The 61st Annual Meeting Of The Association For Computational Linguistics 2023*

 - WinoQueer: A Community-in-the-Loop Benchmark for Anti-LGBTQ+ Bias in Large Language Models.
    [pdf](https://aclanthology.org/2023.acl-long.507v3.pdf)
    - Virginia Felkner, Ho-Chun Herbert Chang, Eugene Jang, and Jonathan May. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - “Fifty Shades of Bias”: Normative Ratings of Gender Bias in GPT Generated English Text.
    [pdf](https://aclanthology.org/2023.emnlp-main.115.pdf)
    - Rishav Hada, Agrima Seth, Harshita Diddee, and Kalika Bali. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Evaluation of African American Language Bias in Natural Language Generation.
    [pdf](https://aclanthology.org/2023.emnlp-main.421.pdf)
    - Nicholas Deas, Jessica Grieser, Shana Kleiner, Desmond Patton, Elsbeth Turcan, and Kathleen Mckeown. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - SeeGULL: A Stereotype Benchmark with Broad Geo-Cultural Coverage Leveraging Generative Models.
    [pdf](https://arxiv.org/pdf/2305.11840)
    - Akshita Jha, Aida Mostafazadeh Davani, Chandan K Reddy, Shachi Dave, Vinodkumar Prabhakaran, and Sunipa Dev. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - Preserving Knowledge Invariance: Rethinking Robustness Evaluation of Open Information Extraction.
    [pdf](https://aclanthology.org/2023.emnlp-main.360.pdf)
    - Ji Qi, Chuchun Zhang, Xiaozhi Wang, Kaisheng Zeng, Jifan Yu, Jinxin Liu, Lei Hou, Juanzi Li, and Xu Bin. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - On the Challenges of Using Black-Box APIs for Toxicity Evaluation in Research.
    [pdf](https://aclanthology.org/2023.emnlp-main.472.pdf)
    - Luiza Pozzobon, Beyza Ermis, Patrick Lewis, and Sara Hooker. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - CHBias: Bias Evaluation and Mitigation of Chinese Conversational Language Models.
    [pdf](https://aclanthology.org/2023.acl-long.757.pdf)
    - Jiaxu Zhao, Meng Fang, Zijing Shi, Yitong Li, Ling Chen, and Mykola Pechenizkiy. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - Socialstigmaqa: A benchmark to uncover stigma amplification in generative language models.
    [pdf](https://arxiv.org/pdf/2312.07492)
    - Manish Nagireddy, Lamogha Chiazor, Moninder Singh, and Ioana Baldini. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - ROBBIE: Robust bias evaluation of large generative language models.
    [pdf](https://arxiv.org/pdf/2311.18140)
    - David Esiobu, Xiaoqing Tan, Saghar Hosseini, Megan Ung, Yuchen Zhang, Jude Fernandes, Jane Dwivedi-Yu, Eleonora Presani, Adina Williams, and Eric Smith. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - SLOG: A Structural Generalization Benchmark for Semantic Parsing.
    [pdf](https://aclanthology.org/2023.emnlp-main.194.pdf)
    - Bingzhi Li, Lucia Donatelli, Alexander Koller, Tal Linzen, Yuekun Yao, and Najoung Kim. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Detection, Diagnosis, and Explanation: A Benchmark for Chinese Medial Hallucination Evaluation.
    [pdf](https://aclanthology.org/2024.lrec-main.428.pdf)
    - Chengfeng Dou, Ying Zhang, Yanyuan Chen, Zhi Jin, Wenpin Jiao, Haiyan Zhao, and Yu Huang. *Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024) 2024*

 - HaluEval: A Large-Scale Hallucination Evaluation Benchmark for Large Language Models.
    [pdf](https://aclanthology.org/2023.emnlp-main.397.pdf)
    - Junyi Li, Xiaoxue Cheng, Wayne Xin Zhao, Jian-Yun Nie, and Ji-Rong Wen. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Benchmarking Hallucination in Large Language Models based on Unanswerable Math Word Problem.
    [pdf](https://aclanthology.org/2024.lrec-main.196.pdf)
    - Yuhong Sun, Zhangyue Yin, Qipeng Guo, Jiawen Wu, Xipeng Qiu, and Hui Zhao. *arXiv preprint arXiv:2403.03558 2024*

 - Evaluating commonsense in pre-trained language models.
    [pdf](https://arxiv.org/pdf/1911.11931)
    - Xuhui Zhou, Yue Zhang, Leyang Cui, and Dandan Huang. *Proceedings of the AAAI conference on artificial intelligence 2020*

 - The Generalization and Robustness of Transformer-Based Language Models on Commonsense Reasoning.
    [pdf](https://ojs.aaai.org/index.php/AAAI/article/view/30410#:~:text=To%20gain%20deeper%20insight%20into%20diagnosing%20these%20models%27,framework%20for%20both%20discriminative%20and%20generative%20language%20models.)
    - Ke Shen. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - RobustLR: A diagnostic benchmark for evaluating logical robustness of deductive reasoners.
    [pdf](https://aclanthology.org/2022.emnlp-main.653.pdf)
    - Soumya Sanyal, Zeyi Liao, and Xiang Ren. *Proceedings of the 2022 Conference on Empirical Methods in Natural Language Processing 2022*

 - Have LLMs Advanced Enough? A Challenging Problem Solving Benchmark For Large Language Models.
    [pdf](https://arxiv.org/pdf/2305.15074)
    - Daman Arora, Himanshu Singh, and others. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - SafeText: A Benchmark for Exploring Physical Safety in Language Models.
    [pdf](https://arxiv.org/pdf/2210.10045)
    - Sharon Levy, Emily Allaway, Melanie Subbiah, Lydia Chilton, Desmond Patton, Kathleen Mckeown, and William Yang Wang. *Proceedings of the 2022 Conference on Empirical Methods in Natural Language Processing 2022*

 - A causal framework to quantify the robustness of mathematical reasoning with language models.
    [pdf](https://aclanthology.org/2023.acl-long.32.pdf)
    - Alessandro Stolfo, Zhijing Jin, Kumar Shridhar, Bernhard Scholkopf, and Mrinmaya Sachan. *arXiv preprint arXiv:2210.12023 2022*

 - A diverse corpus for evaluating and developing English math word problem solvers.
    [pdf](https://arxiv.org/pdf/2106.15772)
    - Shen-Yun Miao, Chao-Chun Liang, and Keh-Yih Su. *arXiv preprint arXiv:2106.15772 2021*

 - MAWPS: A math word problem repository.
    [pdf](https://aclanthology.org/N16-1136.pdf)
    - Rik Koncel-Kedziorski, Subhro Roy, Aida Amini, Nate Kushman, and Hannaneh Hajishirzi. *Proceedings of the 2016 conference of the north american chapter of the association for computational linguistics: human language technologies 2016*

 - Are NLP models really able to solve simple math word problems?.
    [pdf](https://aclanthology.org/2021.naacl-main.168.pdf)
    - Arkil Patel, Satwik Bhattamishra, and Navin Goyal. *arXiv preprint arXiv:2103.07191 2021*

 - Benchmarking large language models in retrieval-augmented generation.
    [[pdf]](https://arxiv.org/pdf)
    - Jiawei Chen, Hongyu Lin, Xianpei Han, and Le Sun. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Lessons from the trenches on reproducible evaluation of language models.
    [pdf](https://arxiv.org/pdf/2405.14782)
    - Stella Biderman, Hailey Schoelkopf, Lintang Sutawika, Leo Gao, Jonathan Tow, Baber Abbasi, Alham Fikri Aji, Pawan Sasanka Ammanamanchi, Sidney Black, Jordan Clive, and others. *arXiv preprint arXiv:2405.14782 2024*

 - On the robustness of chatgpt: An adversarial and out-of-distribution perspective.
    [pdf](https://arxiv.org/abs/2302.12095)
    - Jindong Wang, Xixu Hu, Wenxin Hou, Hao Chen, Runkai Zheng, Yidong Wang, Linyi Yang, Haojun Huang, Wei Ye, Xiubo Geng, and others. *arXiv preprint arXiv:2302.12095 2023*

 - Adversarial glue: A multi-task benchmark for robustness evaluation of language models.
    [pdf](https://arxiv.org/pdf/2111.02840)
    - Boxin Wang, Chejian Xu, Shuohang Wang, Zhe Gan, Yu Cheng, Jianfeng Gao, Ahmed Hassan Awadallah, and Bo Li. *arXiv preprint arXiv:2111.02840 2021*

 - Adversarial NLI: A new benchmark for natural language understanding.
    [pdf](https://arxiv.org/pdf/1910.14599)
    - Yixin Nie, Adina Williams, Emily Dinan, Mohit Bansal, Jason Weston, and Douwe Kiela. *arXiv preprint arXiv:1910.14599 2019*

 - Benchmarking Large Language Model Capabilities for Conditional Generation.
    [pdf](https://arxiv.org/pdf/2306.16793)
    - Joshua Maynez, Priyanka Agrawal, and Sebastian Gehrmann. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - Learning Strategies for Robust Argument Mining: An Analysis of Variations in Language and Domain.
    [pdf](https://aclanthology.org/2024.lrec-main.898.pdf)
    - Ramon Ruiz-Dolz, Chung Chi Chen, Noriko Kando, Hsin Hsi Chen, and others. *Joint 30th International Conference on Computational Linguistics and 14th International Conference on Language Resources and Evaluation, LREC-COLING 2024 2024*

 - Revisiting the Self-Consistency Challenges in Multi-Choice Question Formats for Large Language Model Evaluation.
    [pdf](https://aclanthology.org/2024.lrec-main.1229.pdf)
    - Wenjie Zhou, Qiang Wang, Mingzhou Xu, Ming Chen, and Xiangyu Duan. *Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024) 2024*

 - On Robustness-Accuracy Characterization of Large Language Models using Synthetic Datasets.
    [pdf](https://openreview.net/pdf?id=6iM2asNCjK)
    - Ching-Yun Ko, Pin-Yu Chen, Payel Das, Yung-Sung Chuang, and Luca Daniel. *Unknown Venue 2023*

 - Promptbench: Towards evaluating the robustness of large language models on adversarial prompts.
    [pdf](https://arxiv.org/pdf/2306.04528)
    - Kaijie Zhu, Jindong Wang, Jiaheng Zhou, Zichen Wang, Hao Chen, Yidong Wang, Linyi Yang, Wei Ye, Yue Zhang, Neil Zhenqiang Gong, and others. *arXiv preprint arXiv:2306.04528 2023*

 - Trustworthy LLMs: A survey and guideline for evaluating large language models' alignment.
    [pdf](https://arxiv.org/abs/2404.14294)
    - Yang Liu, Yuanshun Yao, Jean-Francois Ton, Xiaoying Zhang, Ruocheng Guo Hao Cheng, Yegor Klochkov, Muhammad Faaiz Taufiq, and Hang Li. *arXiv preprint arXiv:2308.05374 2023*

 - Bamboo: A comprehensive benchmark for evaluating long text modeling capacities of large language models.
    [pdf](https://arxiv.org/pdf/2309.13345)
    - Zican Dong, Tianyi Tang, Junyi Li, Wayne Xin Zhao, and Ji-Rong Wen. *arXiv preprint arXiv:2309.13345 2023*

 - Revisiting non-English Text Simplification: A Unified Multilingual Benchmark.
    [pdf](https://arxiv.org/pdf/2305.15678)
    - Michael Ryan, Tarek Naous, and Wei Xu. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - ROBBIE: Robust bias evaluation of large generative language models.
    [pdf](https://arxiv.org/pdf/2311.18140)
    - David Esiobu, Xiaoqing Tan, Saghar Hosseini, Megan Ung, Yuchen Zhang, Jude Fernandes, Jane Dwivedi-Yu, Eleonora Presani, Adina Williams, and Eric Smith. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - SLOG: A Structural Generalization Benchmark for Semantic Parsing.
    [pdf](https://aclanthology.org/2023.emnlp-main.194.pdf)
    - Bingzhi Li, Lucia Donatelli, Alexander Koller, Tal Linzen, Yuekun Yao, and Najoung Kim. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Detection, Diagnosis, and Explanation: A Benchmark for Chinese Medial Hallucination Evaluation.
    [pdf](https://aclanthology.org/2024.lrec-main.428.pdf)
    - Chengfeng Dou, Ying Zhang, Yanyuan Chen, Zhi Jin, Wenpin Jiao, Haiyan Zhao, and Yu Huang. *Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024) 2024*

 - HaluEval: A Large-Scale Hallucination Evaluation Benchmark for Large Language Models.
    [pdf](https://aclanthology.org/2023.emnlp-main.397.pdf)
    - Junyi Li, Xiaoxue Cheng, Wayne Xin Zhao, Jian-Yun Nie, and Ji-Rong Wen. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Benchmarking Hallucination in Large Language Models based on Unanswerable Math Word Problem.
    [pdf](https://aclanthology.org/2024.lrec-main.196.pdf)
    - Yuhong Sun, Zhangyue Yin, Qipeng Guo, Jiawen Wu, Xipeng Qiu, and Hui Zhao. *arXiv preprint arXiv:2403.03558 2024*

- Evaluating commonsense in pre-trained language models.
  [pdf](https://arxiv.org/pdf/1911.11931)
    - Xuhui Zhou, Yue Zhang, Leyang Cui, and Dandan Huang. *Proceedings of the AAAI conference on artificial intelligence 2020*

 - The Generalization and Robustness of Transformer-Based Language Models on Commonsense Reasoning.
    [pdf](https://ojs.aaai.org/index.php/AAAI/article/view/30410#:~:text=To%20gain%20deeper%20insight%20into%20diagnosing%20these%20models%27,framework%20for%20both%20discriminative%20and%20generative%20language%20models.)
    - Ke Shen. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - RobustLR: A diagnostic benchmark for evaluating logical robustness of deductive reasoners.
    [pdf](https://aclanthology.org/2022.emnlp-main.653.pdf)
    - Soumya Sanyal, Zeyi Liao, and Xiang Ren. *Proceedings of the 2022 Conference on Empirical Methods in Natural Language Processing 2022*

 - Have LLMs Advanced Enough? A Challenging Problem Solving Benchmark For Large Language Models.
    [pdf](https://arxiv.org/pdf/2305.15074)
    - Daman Arora, Himanshu Singh, and others. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - SafeText: A Benchmark for Exploring Physical Safety in Language Models.
    [pdf](https://arxiv.org/pdf/2210.10045)
    - Sharon Levy, Emily Allaway, Melanie Subbiah, Lydia Chilton, Desmond Patton, Kathleen Mckeown, and William Yang Wang. *Proceedings of the 2022 Conference on Empirical Methods in Natural Language Processing 2022*

 - A causal framework to quantify the robustness of mathematical reasoning with language models.
    [pdf](https://aclanthology.org/2023.acl-long.32.pdf)
    - Alessandro Stolfo, Zhijing Jin, Kumar Shridhar, Bernhard Scholkopf, and Mrinmaya Sachan. *arXiv preprint arXiv:2210.12023 2022*

 - A diverse corpus for evaluating and developing English math word problem solvers.
    [pdf](https://arxiv.org/pdf/2106.15772)
    - Shen-Yun Miao, Chao-Chun Liang, and Keh-Yih Su. *arXiv preprint arXiv:2106.15772 2021*

 - MAWPS: A math word problem repository.
    [pdf](https://aclanthology.org/N16-1136.pdf)
    - Rik Koncel-Kedziorski, Subhro Roy, Aida Amini, Nate Kushman, and Hannaneh Hajishirzi. *Proceedings of the 2016 conference of the north american chapter of the association for computational linguistics: human language technologies 2016*

 - Are NLP models really able to solve simple math word problems?.
    [pdf](https://aclanthology.org/2021.naacl-main.168.pdf)
    - Arkil Patel, Satwik Bhattamishra, and Navin Goyal. *arXiv preprint arXiv:2103.07191 2021*

 - Benchmarking large language models in retrieval-augmented generation.
    [pdf](https://arxiv.org/pdf)
    - Jiawei Chen, Hongyu Lin, Xianpei Han, and Le Sun. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Recode: Robustness evaluation of code generation models.
    [pdf](https://aclanthology.org/2023.acl-long.773.pdf)
    - Shiqi Wang, Zheng Li, Haifeng Qian, Chenghao Yang, Zijian Wang, Mingyue Shang, Varun Kumar, Samson Tan, Baishakhi Ray, Parminder Bhatia, and others. *arXiv preprint arXiv:2212.10264 2022*

 - SCITAB: A Challenging Benchmark for Compositional Reasoning and Claim Verification on Scientific Tables.
    [pdf](https://aclanthology.org/2023.emnlp-main.483.pdf)
    - Xinyuan Lu, Liangming Pan, Qian Liu, Preslav Nakov, and Min-Yen Kan. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - RobuT: A Systematic Study of Table QA Robustness Against Human-Annotated Adversarial Perturbations.
    [pdf](https://arxiv.org/pdf/2306.14321)
    - Yilun Zhao, Chen Zhao, Linyong Nan, Zhenting Qi, Wenlin Zhang, Xiangru Tang, Boyu Mi, and Dragomir Radev. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - White-box multi-objective adversarial attack on dialogue generation.
    [pdf](https://aclanthology.org/2023.acl-long.100.pdf)
    - Yufei Li, Zexin Li, Yingfan Gao, and Cong Liu. *arXiv preprint arXiv:2305.03655 2023*

 - A Comprehensive Analysis of the Effectiveness of Large Language Models as Automatic Dialogue Evaluators.
    [pdf](https://arxiv.org/pdf/2312.15407)
    - Chen Zhang, Luis Fernando D'Haro, Yiming Chen, Malu Zhang, and Haizhou Li. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - MedEval: A Multi-Level, Multi-Task, and Multi-Domain Medical Benchmark for Language Model Evaluation.
    [pdf](https://aclanthology.org/2023.emnlp-main.540.pdf)
    - Zexue He, Yu Wang, An Yan, Yao Liu, Eric Chang, Amilcare Gentili, Julian McAuley, and Chun-nan Hsu. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - NLPositionality: Characterizing Design Biases of Datasets and Models.
    [pdf](https://aclanthology.org/2023.acl-long.505v2.pdf)
    - Sebastin Santy, Jenny T Liang, Ronan Le Bras, Katharina Reinecke, and Maarten Sap. *The 61st Annual Meeting Of The Association For Computational Linguistics 2023*

 - WinoQueer: A Community-in-the-Loop Benchmark for Anti-LGBTQ+ Bias in Large Language Models.
    [pdf](https://aclanthology.org/2023.acl-long.507v3.pdf)
    - Virginia Felkner, Ho-Chun Herbert Chang, Eugene Jang, and Jonathan May. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - “Fifty Shades of Bias”: Normative Ratings of Gender Bias in GPT Generated English Text.
    [pdf](https://aclanthology.org/2023.emnlp-main.115.pdf)
    - Rishav Hada, Agrima Seth, Harshita Diddee, and Kalika Bali. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Evaluation of African American Language Bias in Natural Language Generation.
    [pdf](https://aclanthology.org/2023.emnlp-main.421.pdf)
    - Nicholas Deas, Jessica Grieser, Shana Kleiner, Desmond Patton, Elsbeth Turcan, and Kathleen Mckeown. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - SeeGULL: A Stereotype Benchmark with Broad Geo-Cultural Coverage Leveraging Generative Models.
    [pdf](https://arxiv.org/pdf/2305.11840)
    - Akshita Jha, Aida Mostafazadeh Davani, Chandan K Reddy, Shachi Dave, Vinodkumar Prabhakaran, and Sunipa Dev. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - Preserving Knowledge Invariance: Rethinking Robustness Evaluation of Open Information Extraction.
    [pdf](https://aclanthology.org/2023.emnlp-main.360.pdf)
    - Ji Qi, Chuchun Zhang, Xiaozhi Wang, Kaisheng Zeng, Jifan Yu, Jinxin Liu, Lei Hou, Juanzi Li, and Xu Bin. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - CHBias: Bias Evaluation and Mitigation of Chinese Conversational Language Models.
    [pdf](https://aclanthology.org/2023.acl-long.757.pdf)
    - Jiaxu Zhao, Meng Fang, Zijing Shi, Yitong Li, Ling Chen, and Mykola Pechenizkiy. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - Socialstigmaqa: A benchmark to uncover stigma amplification in generative language models.
    [pdf](https://arxiv.org/pdf/2312.07492)
    - Manish Nagireddy, Lamogha Chiazor, Moninder Singh, and Ioana Baldini. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Benchmarking large language models in retrieval-augmented generation.
    [pdf](https://arxiv.org/pdf)
    - Jiawei Chen, Hongyu Lin, Xianpei Han, and Le Sun. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Learning Strategies for Robust Argument Mining: An Analysis of Variations in Language and Domain.
    [pdf](https://aclanthology.org/2024.lrec-main.898.pdf)
    - Ramon Ruiz-Dolz, Chung Chi Chen, Noriko Kando, Hsin Hsi Chen, and others. *Joint 30th International Conference on Computational Linguistics and 14th International Conference on Language Resources and Evaluation, LREC-COLING 2024 2024*

 - Bamboo: A comprehensive benchmark for evaluating long text modeling capacities of large language models.
    [pdf](https://arxiv.org/pdf/2309.13345)
    - Zican Dong, Tianyi Tang, Junyi Li, Wayne Xin Zhao, and Ji-Rong Wen. *arXiv preprint arXiv:2309.13345 2023*

 - Detection, Diagnosis, and Explanation: A Benchmark for Chinese Medial Hallucination Evaluation.
    [pdf](https://aclanthology.org/2024.lrec-main.428.pdf)
    - Chengfeng Dou, Ying Zhang, Yanyuan Chen, Zhi Jin, Wenpin Jiao, Haiyan Zhao, and Yu Huang. *Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024) 2024*

 - Socialstigmaqa: A benchmark to uncover stigma amplification in generative language models.
    [pdf](https://arxiv.org/pdf/2312.07492)
    - Manish Nagireddy, Lamogha Chiazor, Moninder Singh, and Ioana Baldini. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Revisiting the Self-Consistency Challenges in Multi-Choice Question Formats for Large Language Model Evaluation.
    [pdf](https://aclanthology.org/2024.lrec-main.1229.pdf)
    - Wenjie Zhou, Qiang Wang, Mingzhou Xu, Ming Chen, and Xiangyu Duan. *Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024) 2024*

 - Benchmarking Hallucination in Large Language Models based on Unanswerable Math Word Problem.
    [pdf](https://aclanthology.org/2024.lrec-main.196.pdf)
    - Yuhong Sun, Zhangyue Yin, Qipeng Guo, Jiawen Wu, Xipeng Qiu, and Hui Zhao. *arXiv preprint arXiv:2403.03558 2024*

 - Probing the robustness of pre-trained language models for entity matching.
    [pdf](https://arxiv.org/pdf/2004.00584)
    - Mehdi Akbarian Rastaghi, Ehsan Kamalloo, and Davood Rafiei. *Proceedings of the 31st ACM International Conference on Information & Knowledge Management 2022*

 - Promptbench: Towards evaluating the robustness of large language models on adversarial prompts.
    [pdf](https://arxiv.org/pdf/2306.04528)
    - Kaijie Zhu, Jindong Wang, Jiaheng Zhou, Zichen Wang, Hao Chen, Yidong Wang, Linyi Yang, Wei Ye, Yue Zhang, Neil Zhenqiang Gong, and others. *arXiv preprint arXiv:2306.04528 2023*

 - Trustworthy LLMs: A survey and guideline for evaluating large language models' alignment.
    [pdf](https://arxiv.org/abs/2404.14294)
    - Yang Liu, Yuanshun Yao, Jean-Francois Ton, Xiaoying Zhang, Ruocheng Guo Hao Cheng, Yegor Klochkov, Muhammad Faaiz Taufiq, and Hang Li. *arXiv preprint arXiv:2308.05374 2023*

 - On Robustness-Accuracy Characterization of Large Language Models using Synthetic Datasets.
    [pdf](https://openreview.net/pdf?id=6iM2asNCjK)
    - Ching-Yun Ko, Pin-Yu Chen, Payel Das, Yung-Sung Chuang, and Luca Daniel. *Unknown Venue 2023*

 - Recode: Robustness evaluation of code generation models.
    [pdf](https://aclanthology.org/2023.acl-long.773.pdf)
    - Shiqi Wang, Zheng Li, Haifeng Qian, Chenghao Yang, Zijian Wang, Mingyue Shang, Varun Kumar, Samson Tan, Baishakhi Ray, Parminder Bhatia, and others. *arXiv preprint arXiv:2212.10264 2022*

 - Evaluating large language models trained on code.
    [pdf](https://arxiv.org/pdf/2107.03374)
    - Mark Chen, Jerry Tworek, Heewoo Jun, Qiming Yuan, Henrique Ponde De Oliveira Pinto, Jared Kaplan, Harri Edwards, Yuri Burda, Nicholas Joseph, Greg Brockman, and others. *arXiv preprint arXiv:2107.03374 2021*

 - Program synthesis with large language models.
    [pdf](https://arxiv.org/pdf/2108.07732)
    - Jacob Austin, Augustus Odena, Maxwell Nye, Maarten Bosma, Henryk Michalewski, David Dohan, Ellen Jiang, Carrie Cai, Michael Terry, Quoc Le, and others. *arXiv preprint arXiv:2108.07732 2021*

 - A causal framework to quantify the robustness of mathematical reasoning with language models.
    [pdf](https://aclanthology.org/2023.acl-long.32.pdf)
    - Alessandro Stolfo, Zhijing Jin, Kumar Shridhar, Bernhard Scholkopf, and Mrinmaya Sachan. *arXiv preprint arXiv:2210.12023 2022*

 - A diverse corpus for evaluating and developing English math word problem solvers.
    [pdf](https://arxiv.org/pdf/2106.15772)
    - Shen-Yun Miao, Chao-Chun Liang, and Keh-Yih Su. *arXiv preprint arXiv:2106.15772 2021*

 - MAWPS: A math word problem repository.
    [pdf](https://aclanthology.org/N16-1136.pdf)
    - Rik Koncel-Kedziorski, Subhro Roy, Aida Amini, Nate Kushman, and Hannaneh Hajishirzi. *Proceedings of the 2016 conference of the north american chapter of the association for computational linguistics: human language technologies 2016*

 - Are NLP models really able to solve simple math word problems?.
    [pdf](https://aclanthology.org/2021.naacl-main.168.pdf)
    - Arkil Patel, Satwik Bhattamishra, and Navin Goyal. *arXiv preprint arXiv:2103.07191 2021*

 - White-box multi-objective adversarial attack on dialogue generation.
    [pdf](https://aclanthology.org/2023.acl-long.100.pdf)
    - Yufei Li, Zexin Li, Yingfan Gao, and Cong Liu. *arXiv preprint arXiv:2305.03655 2023*

 - Can you put it all together: Evaluating conversational agents' ability to blend skills.
    [pdf](https://arxiv.org/pdf/2004.08449)
    - Eric Michael Smith, Mary Williamson, Kurt Shuster, Jason Weston, and Y-Lan Boureau. *arXiv preprint arXiv:2004.08449 2020*

 - Personalizing dialogue agents: I have a dog, do you have pets too?.
    [pdf](https://aclanthology.org/P18-1205.pdf)
    - Saizheng Zhang, Emily Dinan, Jack Urbanek, Arthur Szlam, Douwe Kiela, and Jason Weston. *arXiv preprint arXiv:1801.07243 2018*

 - The second conversational intelligence challenge (convai2).
    [pdf](https://arxiv.org/pdf/1902.00098)
    - Emily Dinan, Varvara Logacheva, Valentin Malykh, Alexander Miller, Kurt Shuster, Jack Urbanek, Douwe Kiela, Arthur Szlam, Iulian Serban, Ryan Lowe, and others. *The NeurIPS'18 Competition: From Machine Learning to Intelligent Conversations 2020*

 - Towards empathetic open-domain conversation models: A new benchmark and dataset.
    [pdf](https://aclanthology.org/P19-1534.pdf)
    - Hannah Rashkin, Eric Michael Smith, Margaret Li, and Y-Lan Boureau. *arXiv preprint arXiv:1811.00207 2018*

 - Preserving Knowledge Invariance: Rethinking Robustness Evaluation of Open Information Extraction.
    [pdf](https://aclanthology.org/2023.emnlp-main.360.pdf)
    - Ji Qi, Chuchun Zhang, Xiaozhi Wang, Kaisheng Zeng, Jifan Yu, Jinxin Liu, Lei Hou, Juanzi Li, and Xu Bin. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - ROBBIE: Robust bias evaluation of large generative language models.
    [pdf](https://arxiv.org/pdf/2311.18140)
    - David Esiobu, Xiaoqing Tan, Saghar Hosseini, Megan Ung, Yuchen Zhang, Jude Fernandes, Jane Dwivedi-Yu, Eleonora Presani, Adina Williams, and Eric Smith. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - On the Challenges of Using Black-Box APIs for Toxicity Evaluation in Research.
    [pdf](https://aclanthology.org/2023.emnlp-main.472.pdf)
    - Luiza Pozzobon, Beyza Ermis, Patrick Lewis, and Sara Hooker. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Benchmarking Large Language Model Capabilities for Conditional Generation.
    [pdf](https://arxiv.org/pdf/2306.16793)
    - Joshua Maynez, Priyanka Agrawal, and Sebastian Gehrmann. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

### Causal Related Evaluation
 - The Generalization and Robustness of Transformer-Based Language Models on Commonsense Reasoning.
    [pdf](https://ojs.aaai.org/index.php/AAAI/article/view/30410#:~:text=To%20gain%20deeper%20insight%20into%20diagnosing%20these%20models%27,framework%20for%20both%20discriminative%20and%20generative%20language%20models.)
    - Ke Shen. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - A Comprehensive Analysis of the Effectiveness of Large Language Models as Automatic Dialogue Evaluators.
    [pdf](https://arxiv.org/pdf/2312.15407)
    - Chen Zhang, Luis Fernando D'Haro, Yiming Chen, Malu Zhang, and Haizhou Li. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Benchmarking large language models in retrieval-augmented generation.
    [pdf](https://arxiv.org/pdf)
    - Jiawei Chen, Hongyu Lin, Xianpei Han, and Le Sun. *Proceedings of the AAAI Conference on Artificial Intelligence 2024*

 - Vision transformers are robust learners.
    [pdf](https://arxiv.org/pdf/2105.07581)
    - Sayak Paul and Pin-Yu Chen. *Proceedings of the AAAI conference on Artificial Intelligence 2022*

 - Evaluating commonsense in pre-trained language models.
    [pdf](https://arxiv.org/pdf/1911.11931)
    - Xuhui Zhou, Yue Zhang, Leyang Cui, and Dandan Huang. *Proceedings of the AAAI conference on artificial intelligence 2020*

 - Learning Strategies for Robust Argument Mining: An Analysis of Variations in Language and Domain.
    [pdf](https://aclanthology.org/2024.lrec-main.898.pdf)
    - Ramon Ruiz-Dolz, Chung Chi Chen, Noriko Kando, Hsin Hsi Chen, and others. *Joint 30th International Conference on Computational Linguistics and 14th International Conference on Language Resources and Evaluation, LREC-COLING 2024 2024*

 - Bamboo: A comprehensive benchmark for evaluating long text modeling capacities of large language models.
    [pdf](https://arxiv.org/pdf/2309.13345)
    - Zican Dong, Tianyi Tang, Junyi Li, Wayne Xin Zhao, and Ji-Rong Wen. *arXiv preprint arXiv:2309.13345 2023*

 - Detection, Diagnosis, and Explanation: A Benchmark for Chinese Medial Hallucination Evaluation.
    [pdf](https://aclanthology.org/2024.lrec-main.428.pdf)
    - Chengfeng Dou, Ying Zhang, Yanyuan Chen, Zhi Jin, Wenpin Jiao, Haiyan Zhao, and Yu Huang. *Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024) 2024*

 - On the robustness of chatgpt: An adversarial and out-of-distribution perspective.
    [pdf](https://arxiv.org/abs/2302.12095)
    - Jindong Wang, Xixu Hu, Wenxin Hou, Hao Chen, Runkai Zheng, Yidong Wang, Linyi Yang, Haojun Huang, Wei Ye, Xiubo Geng, and others. *arXiv preprint arXiv:2302.12095 2023*

 - Adversarial glue: A multi-task benchmark for robustness evaluation of language models.
    [pdf](https://arxiv.org/pdf/2111.02840)
    - Boxin Wang, Chejian Xu, Shuohang Wang, Zhe Gan, Yu Cheng, Jianfeng Gao, Ahmed Hassan Awadallah, and Bo Li. *arXiv preprint arXiv:2111.02840 2021*

 - Adversarial NLI: A new benchmark for natural language understanding.
    [pdf](https://arxiv.org/pdf/1910.14599)
    - Yixin Nie, Adina Williams, Emily Dinan, Mohit Bansal, Jason Weston, and Douwe Kiela. *arXiv preprint arXiv:1910.14599 2019*

 - NLPositionality: Characterizing Design Biases of Datasets and Models.
    [pdf](https://aclanthology.org/2023.acl-long.505v2.pdf)
    - Sebastin Santy, Jenny T Liang, Ronan Le Bras, Katharina Reinecke, and Maarten Sap. *The 61st Annual Meeting Of The Association For Computational Linguistics 2023*

 - WinoQueer: A Community-in-the-Loop Benchmark for Anti-LGBTQ+ Bias in Large Language Models.
    [pdf](https://aclanthology.org/2023.acl-long.507v3.pdf)
    - Virginia Felkner, Ho-Chun Herbert Chang, Eugene Jang, and Jonathan May. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - CHBias: Bias Evaluation and Mitigation of Chinese Conversational Language Models.
    [pdf](https://aclanthology.org/2023.acl-long.757.pdf)
    - Jiaxu Zhao, Meng Fang, Zijing Shi, Yitong Li, Ling Chen, and Mykola Pechenizkiy. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - “Fifty Shades of Bias”: Normative Ratings of Gender Bias in GPT Generated English Text.
    [pdf](https://aclanthology.org/2023.emnlp-main.115.pdf)
    - Rishav Hada, Agrima Seth, Harshita Diddee, and Kalika Bali. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - Evaluation of African American Language Bias in Natural Language Generation.
    [pdf](https://aclanthology.org/2023.emnlp-main.421.pdf)
    - Nicholas Deas, Jessica Grieser, Shana Kleiner, Desmond Patton, Elsbeth Turcan, and Kathleen Mckeown. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - SeeGULL: A Stereotype Benchmark with Broad Geo-Cultural Coverage Leveraging Generative Models.
    [pdf](https://arxiv.org/pdf/2305.11840)
    - Akshita Jha, Aida Mostafazadeh Davani, Chandan K Reddy, Shachi Dave, Vinodkumar Prabhakaran, and Sunipa Dev. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - Revisiting non-English Text Simplification: A Unified Multilingual Benchmark.
    [pdf](https://arxiv.org/pdf/2305.15678)
    - Michael Ryan, Tarek Naous, and Wei Xu. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - SCITAB: A Challenging Benchmark for Compositional Reasoning and Claim Verification on Scientific Tables.
    [pdf](https://aclanthology.org/2023.emnlp-main.483.pdf)
    - Xinyuan Lu, Liangming Pan, Qian Liu, Preslav Nakov, and Min-Yen Kan. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - MedEval: A Multi-Level, Multi-Task, and Multi-Domain Medical Benchmark for Language Model Evaluation.
    [pdf](https://aclanthology.org/2023.emnlp-main.540.pdf)
    - Zexue He, Yu Wang, An Yan, Yao Liu, Eric Chang, Amilcare Gentili, Julian McAuley, and Chun-nan Hsu. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - SafeText: A Benchmark for Exploring Physical Safety in Language Models.
    [pdf](https://arxiv.org/pdf/2210.10045)
    - Sharon Levy, Emily Allaway, Melanie Subbiah, Lydia Chilton, Desmond Patton, Kathleen Mckeown, and William Yang Wang. *Proceedings of the 2022 Conference on Empirical Methods in Natural Language Processing 2022*

 - RobuT: A Systematic Study of Table QA Robustness Against Human-Annotated Adversarial Perturbations.
    [pdf](https://arxiv.org/pdf/2306.14321)
    - Yilun Zhao, Chen Zhao, Linyong Nan, Zhenting Qi, Wenlin Zhang, Xiangru Tang, Boyu Mi, and Dragomir Radev. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - ReCode: Robustness Evaluation of Code Generation Models.
    [pdf](https://aclanthology.org/2023.acl-long.773.pdf)
    - Shiqi Wang, Zheng Li, Haifeng Qian, Chenghao Yang, Zijian Wang, Mingyue Shang, Varun Kumar, Samson Tan, Baishakhi Ray, Parminder Bhatia, and others. *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) 2023*

 - HaluEval: A Large-Scale Hallucination Evaluation Benchmark for Large Language Models.
    [pdf](https://aclanthology.org/2023.emnlp-main.397.pdf)
    - Junyi Li, Xiaoxue Cheng, Wayne Xin Zhao, Jian-Yun Nie, and Ji-Rong Wen. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - RobustLR: A diagnostic benchmark for evaluating logical robustness of deductive reasoners.
    [pdf](https://aclanthology.org/2022.emnlp-main.653.pdf)
    - Soumya Sanyal, Zeyi Liao, and Xiang Ren. *Proceedings of the 2022 Conference on Empirical Methods in Natural Language Processing 2022*

 - Have LLMs Advanced Enough? A Challenging Problem Solving Benchmark For Large Language Models.
    [pdf](https://arxiv.org/pdf/2305.15074)
    - Daman Arora, Himanshu Singh, and others. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - This is not a Dataset: A Large Negation Benchmark to Challenge Large Language Models.
    [pdf](https://arxiv.org/pdf/2310.15941)
    - Iker García-Ferrero, Begoña Altuna,, Javier Alvez, Itziar Gonzalez-Dios, and German Rigau. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

 - SLOG: A Structural Generalization Benchmark for Semantic Parsing.
    [pdf](https://aclanthology.org/2023.emnlp-main.194.pdf)
    - Bingzhi Li, Lucia Donatelli, Alexander Koller, Tal Linzen, Yuekun Yao, and Najoung Kim. *Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing 2023*

#### If you find our survey useful for your research, please cite the following paper:
```
@article{llmrobust-survey,
    title={Evaluating and Improving Robustness in Large Language Models: A Survey and Future Directions},
    author={Kun Zhang, Le Wu, Kui Yu, Guangyi Lv, Dacao Zhang},
    year={2025},
    journal={arXiv preprint},
    url={https://arxiv.org/abs/2506.11111}
}
```