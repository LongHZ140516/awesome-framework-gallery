# 🖼️ awesome-framework-gallery
In an article, a project homepage or a github repository, a good-looking framework diagram often attracts more people to pay attention to the project work. But in scientific research, we often worry about how to make a good-looking framework diagram, so we always check other people's paper framework diagrams for reference and learning. But it is undeniable that although framework diagrams are not in the same field, there are often things worth learning from, such as color matching, process representation, etc.
When I was drawing pictures for the paper with my classmates at the beginning of the year, I tried to find out if anyone had sorted out good-looking framework diagrams, so that I could refer to and learn how to make good-looking pictures, but it seemed that I didn't find any. Inspired by this incident, I wondered if I could set up a github repository to store good-looking framework diagrams🤔? So there was this repository.
## 📄 Table of contents
- [LLM](#LLM)
- [Diffusion](#Diffusion)
- [3DGS](#3D-gaussian-splatting)
- [NeRF](#NeRF)

<!-- LLM part -->
## LLM

### 1.[CVPR'2024 Oral] MMMU: A Massive Multi-discipline Multimodal Understanding and Reasoning Benchmark for Expert AGI
**Authors:** Xiang Yue, Yuansheng Ni, Kai Zhang, Tianyu Zheng, Ruoqi Liu, Ge Zhang, Samuel Stevens, Dongfu Jiang, Weiming Ren, Yuxuan Sun, Cong Wei, Botao Yu, Ruibin Yuan, Renliang Sun, Ming Yin, Boyuan Zheng, Zhenzhu Yang, Yibo Liu, Wenhao Huang, Huan Sun, Yu Su, Wenhu Chen
<details span>
<summary><b>Abstract</b></summary>
We introduce MMMU: a new benchmark designed to evaluate multimodal models on massive multi-discipline tasks demanding college-level subject knowledge and deliberate reasoning. MMMU includes 11.5K meticulously collected multimodal questions from college exams, quizzes, and textbooks, covering six core disciplines: Art & Design, Business, Science, Health & Medicine, Humanities & Social Science, and Tech & Engineering. These questions span 30 subjects and 183 subfields, comprising 30 highly heterogeneous image types, such as charts, diagrams, maps, tables, music sheets, and chemical structures. Unlike existing benchmarks, MMMU focuses on advanced perception and reasoning with domain-specific knowledge, challenging models to perform tasks akin to those faced by experts. The evaluation of 14 open-source LMMs as well as the proprietary GPT-4V(ision) and Gemini highlights the substantial challenges posed by MMMU. Even the advanced GPT-4V and Gemini Ultra only achieve accuracies of 56% and 59% respectively, indicating significant room for improvement. We believe MMMU will stimulate the community to build next-generation multimodal foundation models towards expert artificial general intelligence.
</details>

[📄 Paper](https://arxiv.org/pdf/2311.16502) | [🌐 Project Page](https://mmmu-benchmark.github.io/) | [💻 Code](https://github.com/MMMU-Benchmark/MMMU)

![MMMU](images/LLM/MMMU.jpg)

### 2. UrBench: A Comprehensive Benchmark for Evaluating Large Multimodal Models in Multi-View Urban Scenarios
**Authors:** Baichuan Zhou, Haote Yang, Dairong Chen, Junyan Ye, Tianyi Bai, Jinhua Yu, Songyang Zhang, Dahua Lin, Conghui He, Weijia Li
<details span>
<summary><b>Abstract</b></summary>
Recent evaluations of Large Multimodal Models (LMMs) have explored their capabilities in various domains, with only few benchmarks specifically focusing on urban environments. Moreover, existing urban benchmarks have been limited to evaluating LMMs with basic region-level urban tasks under singular views, leading to incomplete evaluations of LMMs' abilities in urban environments. To address these issues, we present UrBench, a comprehensive benchmark designed for evaluating LMMs in complex multi-view urban scenarios. UrBench contains 11.6K meticulously curated questions at both region-level and role-level that cover 4 task dimensions: Geo-Localization, Scene Reasoning, Scene Understanding, and Object Understanding, totaling 14 task types. In constructing UrBench, we utilize data from existing datasets and additionally collect data from 11 cities, creating new annotations using a cross-view detection-matching method. With these images and annotations, we then integrate LMM-based, rule-based, and human-based methods to construct large-scale high-quality questions. Our evaluations on 21 LMMs show that current LMMs struggle in the urban environments in several aspects. Even the best performing GPT-4o lags behind humans in most tasks, ranging from simple tasks such as counting to complex tasks such as orientation, localization and object attribute recognition, with an average performance gap of 17.4%. Our benchmark also reveals that LMMs exhibit inconsistent behaviors with different urban views, especially with respect to understanding cross-view relations.
</details>

[📄 Paper](https://arxiv.org/pdf/2408.17267) | [🌐 Project Page](https://opendatalab.github.io/UrBench/) | [💻 Code](https://github.com/opendatalab/UrBench?tab=readme-ov-file)

![Urbench](images/LLM/Urbench.jpg)

### 3. SciLitLLM: How to Adapt LLMs for Scientific Literature Understanding
**Authors:** Sihang Li, Jin Huang, Jiaxi Zhuang, Yaorui Shi, Xiaochen Cai, Mingjun Xu, Xiang Wang, Linfeng Zhang, Guolin Ke, Hengxing Cai
<details span>
<summary><b>Abstract</b></summary>
Scientific literature understanding is crucial for extracting targeted information and garnering insights, thereby significantly advancing scientific discovery. Despite the remarkable success of Large Language Models (LLMs), they face challenges in scientific literature understanding, primarily due to (1) a lack of scientific knowledge and (2) unfamiliarity with specialized scientific tasks.
To develop an LLM specialized in scientific literature understanding, we propose a hybrid strategy that integrates continual pre-training (CPT) and supervised fine-tuning (SFT), to simultaneously infuse scientific domain knowledge and enhance instruction-following capabilities for domain-specific tasks.cIn this process, we identify two key challenges: (1) constructing high-quality CPT corpora, and (2) generating diverse SFT instructions. We address these challenges through a meticulous pipeline, including PDF text extraction, parsing content error correction, quality filtering, and synthetic instruction creation. Applying this strategy, we present a suite of LLMs: SciLitLLM, specialized in scientific literature understanding. These models demonstrate promising performance on scientific literature understanding benchmarks.
Our contributions are threefold: (1) We present an effective framework that integrates CPT and SFT to adapt LLMs to scientific literature understanding, which can also be easily adapted to other domains. (2) We propose an LLM-based synthesis method to generate diverse and high-quality scientific instructions, resulting in a new instruction set -- SciLitIns -- for supervised fine-tuning in less-represented scientific domains. (3) SciLitLLM achieves promising performance improvements on scientific literature understanding benchmarks.
</details>

[📄 Paper](https://arxiv.org/pdf/2408.15545)

![SciLitLLM](images/LLM/SciLitLLM.jpg)


### 4. VITA: Towards Open-Source Interactive Omni Multimodal LLM
**Authors:** Chaoyou Fu, Haojia Lin, Zuwei Long, Yunhang Shen, Meng Zhao, Yifan Zhang, Shaoqi Dong, Xiong Wang, Di Yin, Long Ma, Xiawu Zheng, Ran He, Rongrong Ji, Yunsheng Wu, Caifeng Shan, Xing Sun
<details span>
<summary><b>Abstract</b></summary>
The remarkable multimodal capabilities and interactive experience of GPT-4o underscore their necessity in practical applications, yet open-source models rarely excel in both areas. In this paper, we introduce VITA, the first-ever open-source Multimodal Large Language Model (MLLM) adept at simultaneous processing and analysis of Video, Image, Text, and Audio modalities, and meanwhile has an advanced multimodal interactive experience. Starting from Mixtral 8x7B as a language foundation, we expand its Chinese vocabulary followed by bilingual instruction tuning. We further endow the language model with visual and audio capabilities through two-stage multi-task learning of multimodal alignment and instruction tuning. VITA demonstrates robust foundational capabilities of multilingual, vision, and audio understanding, as evidenced by its strong performance across a range of both unimodal and multimodal benchmarks. Beyond foundational capabilities, we have made considerable progress in enhancing the natural multimodal human-computer interaction experience. VITA is the first step for the open-source community to explore the seamless integration of multimodal understanding and interaction. While there is still lots of work to be done on VITA to get close to close-source counterparts, we hope that its role as a pioneer can serve as a cornerstone for subsequent research.
</details>

[📄 Paper](https://arxiv.org/pdf/2408.05211) | [🌐 Project Page](https://vita-home.github.io/) | [💻 Code](https://github.com/VITA-MLLM/VITA)

![VITA](images/LLM/VITA.jpg)

### 5. TableBench: A Comprehensive and Complex Benchmark for Table Question Answering
**Authors:** Xianjie Wu, Jian Yang, Linzheng Chai, Ge Zhang, Jiaheng Liu, Xinrun Du, Di Liang, Daixin Shu, Xianfu Cheng, Tianzhen Sun, Guanglin Niu, Tongliang Li, Zhoujun Li

<details span>
<summary><b>Abstract</b></summary>
Recent advancements in Large Language Models (LLMs) have markedly enhanced the interpretation and processing of tabular data, introducing previously unimaginable capabilities. Despite these achievements, LLMs still encounter significant challenges when applied in industrial scenarios, particularly due to the increased complexity of reasoning required with real-world tabular data, underscoring a notable disparity between academic benchmarks and practical applications. To address this discrepancy, we conduct a detailed investigation into the application of tabular data in industrial scenarios and propose a comprehensive and complex benchmark TableBench, including 18 fields within four major categories of table question answering (TableQA) capabilities. Furthermore, we introduce TableLLM, trained on our meticulously constructed training set TableInstruct, achieving comparable performance with GPT-3.5. Massive experiments conducted on TableBench indicate that both open-source and proprietary LLMs still have significant room for improvement to meet real-world demands, where the most advanced model, GPT-4, achieves only a modest score compared to humans.
</details>

[📄 Paper](https://arxiv.org/pdf/2408.09174) | [🌐 Project Page](https://tablebench.github.io/) | [💻 Code](https://github.com/TableBench/TableBench)

![TableBench](images/LLM/TableBench.jpg)

### 6. I-SHEEP: Self-Alignment of LLM from Scratch through an Iterative Self-Enhancement Paradigm
**Authors:** Yiming Liang, Ge Zhang, Xingwei Qu, Tianyu Zheng, Jiawei Guo, Xinrun Du, Zhenzhu Yang, Jiaheng Liu, Chenghua Lin, Lei Ma, Wenhao Huang, Jiajun Zhang

<details span>
<summary><b>Abstract</b></summary>
Large Language Models (LLMs) have achieved significant advancements, however, the common learning paradigm treats LLMs as passive information repositories, neglecting their potential for active learning and alignment. Some approaches train LLMs using their own generated synthetic data, exploring the possibility of active alignment. However, there is still a huge gap between these one-time alignment methods and the continuous automatic alignment of humans. In this paper, we introduce \textbf{I-SHEEP}, an \textbf{I}terative \textbf{S}elf-En\textbf{H}anc\textbf{E}m\textbf{E}nt \textbf{P}aradigm.This human-like paradigm enables LLMs to \textbf{continuously self-align from scratch with nothing}. Compared to the one-time alignment method Dromedary \cite{sun2023principledriven}, which refers to the first iteration in this paper, I-SHEEP can significantly enhance capacities on both Qwen and Llama models. I-SHEEP achieves a maximum relative improvement of 78.2\% in the Alpaca Eval, 24.0\% in the MT Bench, and an absolute increase of 8.88\% in the IFEval accuracy over subsequent iterations in Qwen-1.5 72B model. Additionally, I-SHEEP surpasses the base model in various standard benchmark generation tasks, achieving an average improvement of 24.77\% in code generation tasks, 12.04\% in TrivialQA, and 20.29\% in SQuAD. We also provide new insights based on the experiment results.
</details>

[📄 Paper](https://www.arxiv.org/pdf/2408.08072) | [💻 Code](https://github.com/multimodal-art-projection/I-SHEEP)

![TableBench](images/LLM/I-SHEEP.jpg)

### 7. mPLUG-Owl3: Towards Long Image-Sequence Understanding in Multi-Modal Large Language Models
**Authors:** Jiabo Ye, Haiyang Xu, Haowei Liu, Anwen Hu, Ming Yan, Qi Qian, Ji Zhang, Fei Huang, Jingren Zhou

<details span>
<summary><b>Abstract</b></summary>
Multi-modal Large Language Models (MLLMs) have demonstrated remarkable capabilities in executing instructions for a variety of single-image tasks. Despite this progress, significant challenges remain in modeling long image sequences. In this work, we introduce the versatile multi-modal large language model, mPLUG-Owl3, which enhances the capability for long image-sequence understanding in scenarios that incorporate retrieved image-text knowledge, interleaved image-text, and lengthy videos. Specifically, we propose novel hyper attention blocks to efficiently integrate vision and language into a common language-guided semantic space, thereby facilitating the processing of extended multi-image scenarios. Extensive experimental results suggest that mPLUG-Owl3 achieves state-of-the-art performance among models with a similar size on single-image, multi-image, and video benchmarks. Moreover, we propose a challenging long visual sequence evaluation named Distractor Resistance to assess the ability of models to maintain focus amidst distractions. Finally, with the proposed architecture, mPLUG-Owl3 demonstrates outstanding performance on ultra-long visual sequence inputs. We hope that mPLUG-Owl3 can contribute to the development of more efficient and powerful multimodal large language models.
</details>

[📄 Paper](https://www.arxiv.org/pdf/2408.04840) | [💻 Code](https://github.com/X-PLUG/mPLUG-Owl)

![mPLUG-Owl3](images/LLM/mPLUG-Owl3.jpg)

### 8. GMAI-MMBench: A Comprehensive Multimodal Evaluation Benchmark Towards General Medical AI
**Authors:** Pengcheng Chen, Jin Ye, Guoan Wang, Yanjun Li, Zhongying Deng, Wei Li, Tianbin Li, Haodong Duan, Ziyan Huang, Yanzhou Su, Benyou Wang, Shaoting Zhang, Bin Fu, Jianfei Cai, Bohan Zhuang, Eric J Seibel, Junjun He, Yu Qiao

<details span>
<summary><b>Abstract</b></summary>
Large Vision-Language Models (LVLMs) are capable of handling diverse data types such as imaging, text, and physiological signals, and can be applied in various fields. In the medical field, LVLMs have a high potential to offer substantial assistance for diagnosis and treatment. Before that, it is crucial to develop benchmarks to evaluate LVLMs' effectiveness in various medical applications. Current benchmarks are often built upon specific academic literature, mainly focusing on a single domain, and lacking varying perceptual granularities. Thus, they face specific challenges, including limited clinical relevance, incomplete evaluations, and insufficient guidance for interactive LVLMs. To address these limitations, we developed the GMAI-MMBench, the most comprehensive general medical AI benchmark with well-categorized data structure and multi-perceptual granularity to date. It is constructed from 285 datasets across 39 medical image modalities, 18 clinical-related tasks, 18 departments, and 4 perceptual granularities in a Visual Question Answering (VQA) format. Additionally, we implemented a lexical tree structure that allows users to customize evaluation tasks, accommodating various assessment needs and substantially supporting medical AI research and applications. We evaluated 50 LVLMs, and the results show that even the advanced GPT-4o only achieves an accuracy of 52%, indicating significant room for improvement. Moreover, we identified five key insufficiencies in current cutting-edge LVLMs that need to be addressed to advance the development of better medical applications. We believe that GMAI-MMBench will stimulate the community to build the next generation of LVLMs toward GMAI.
</details>

[📄 Paper](https://www.arxiv.org/pdf/2408.03361) | [🌐 Project Page](https://uni-medical.github.io/GMAI-MMBench.github.io/) | [💻 Code](https://github.com/uni-medical/GMAI-MMBench)

![GMAI-MMBench](images/LLM/GMAI-MMBench.jpg)

### 9. MMIU: Multimodal Multi-image Understanding for Evaluating Large Vision-Language Models
**Authors:** Fanqing Meng, Jin Wang, Chuanhao Li, Quanfeng Lu, Hao Tian, Jiaqi Liao, Xizhou Zhu, Jifeng Dai, Yu Qiao, Ping Luo, Kaipeng Zhang, Wenqi Shao

<details span>
<summary><b>Abstract</b></summary>
The capability to process multiple images is crucial for Large Vision-Language Models (LVLMs) to develop a more thorough and nuanced understanding of a scene. Recent multi-image LVLMs have begun to address this need. However, their evaluation has not kept pace with their development. To fill this gap, we introduce the Multimodal Multi-image Understanding (MMIU) benchmark, a comprehensive evaluation suite designed to assess LVLMs across a wide range of multi-image tasks. MMIU encompasses 7 types of multi-image relationships, 52 tasks, 77K images, and 11K meticulously curated multiple-choice questions, making it the most extensive benchmark of its kind. Our evaluation of 24 popular LVLMs, including both open-source and proprietary models, reveals significant challenges in multi-image comprehension, particularly in tasks involving spatial understanding. Even the most advanced models, such as GPT-4o, achieve only 55.7% accuracy on MMIU. Through multi-faceted analytical experiments, we identify key performance gaps and limitations, providing valuable insights for future model and data improvements. We aim for MMIU to advance the frontier of LVLM research and development, moving us toward achieving sophisticated multimodal multi-image user interactions.
</details>

[📄 Paper](https://www.arxiv.org/pdf/2408.02718) | [🌐 Project Page](https://mmiu-bench.github.io/) | [💻 Code](https://github.com/OpenGVLab/MMIU)

![MMIU](images/LLM/MMIU.jpg)

### 10. Benchmarking Trustworthiness of Multimodal Large Language Models: A Comprehensive Study
**Authors:** Yichi Zhang, Yao Huang, Yitong Sun, Chang Liu, Zhe Zhao, Zhengwei Fang, Yifan Wang, Huanran Chen, Xiao Yang, Xingxing Wei, Hang Su, Yinpeng Dong, Jun Zhu

<details span>
<summary><b>Abstract</b></summary>
Despite the superior capabilities of Multimodal Large Language Models (MLLMs) across diverse tasks, they still face significant trustworthiness challenges. Yet, current literature on the assessment of trustworthy MLLMs remains limited, lacking a holistic evaluation to offer thorough insights into future improvements. In this work, we establish MultiTrust, the first comprehensive and unified benchmark on the trustworthiness of MLLMs across five primary aspects: truthfulness, safety, robustness, fairness, and privacy. Our benchmark employs a rigorous evaluation strategy that addresses both multimodal risks and cross-modal impacts, encompassing 32 diverse tasks with self-curated datasets. Extensive experiments with 21 modern MLLMs reveal some previously unexplored trustworthiness issues and risks, highlighting the complexities introduced by the multimodality and underscoring the necessity for advanced methodologies to enhance their reliability. For instance, typical proprietary models still struggle with the perception of visually confusing images and are vulnerable to multimodal jailbreaking and adversarial attacks; MLLMs are more inclined to disclose privacy in text and reveal ideological and cultural biases even when paired with irrelevant images in inference, indicating that the multimodality amplifies the internal risks from base LLMs. Additionally, we release a scalable toolbox for standardized trustworthiness research, aiming to facilitate future advancements in this important field. 
</details>

[📄 Paper](https://arxiv.org/pdf/2406.07057) | [🌐 Project Page](https://multi-trust.github.io/) | [💻 Code](https://github.com/thu-ml/MMTrustEval)

![Mult-Trust](images/LLM/Multi-Trust.jpg)


### 11. VisionUnite: A Vision-Language Foundation Model for Ophthalmology Enhanced with Clinical Knowledge
**Authors:** Zihan Li, Diping Song, Zefeng Yang, Deming Wang, Fei Li, Xiulan Zhang, Paul E. Kinahan, Yu Qiao

<details span>
<summary><b>Abstract</b></summary>
The need for improved diagnostic methods in ophthalmology is acute, especially in the less developed regions with limited access to specialists and advanced equipment. Therefore, we introduce VisionUnite, a novel vision-language foundation model for ophthalmology enhanced with clinical knowledge. VisionUnite has been pretrained on an extensive dataset comprising 1.24 million image-text pairs, and further refined using our proposed MMFundus dataset, which includes 296,379 high-quality fundus image-text pairs and 889,137 simulated doctor-patient dialogue instances. Our experiments indicate that VisionUnite outperforms existing generative foundation models such as GPT-4V and Gemini Pro. It also demonstrates diagnostic capabilities comparable to junior ophthalmologists. VisionUnite performs well in various clinical scenarios including open-ended multi-disease diagnosis, clinical explanation, and patient interaction, making it a highly versatile tool for initial ophthalmic disease screening. VisionUnite can also serve as an educational aid for junior ophthalmologists, accelerating their acquisition of knowledge regarding both common and rare ophthalmic conditions. VisionUnite represents a significant advancement in ophthalmology, with broad implications for diagnostics, medical education, and understanding of disease mechanisms.
</details>

[📄 Paper](https://www.arxiv.org/pdf/2408.02865) | [💻 Code](https://github.com/HUANGLIZI/VisionUnite)

![VisionUnite](images/LLM/VisionUnite.jpg)


### 12. MJ-Bench: Is Your Multimodal Reward Model Really a Good Judge for Text-to-Image Generation?
**Authors:** Zhaorun Chen, Yichao Du, Zichen Wen, Yiyang Zhou, Chenhang Cui, Zhenzhen Weng, Haoqin Tu, Chaoqi Wang, Zhengwei Tong, Qinglan Huang, Canyu Chen, Qinghao Ye, Zhihong Zhu, Yuqing Zhang, Jiawei Zhou, Zhuokai Zhao, Rafael Rafailov, Chelsea Finn, Huaxiu Yao

<details span>
<summary><b>Abstract</b></summary>
While text-to-image models like DALLE-3 and Stable Diffusion are rapidly proliferating, they often encounter challenges such as hallucination, bias, and the production of unsafe, low-quality output. To effectively address these issues, it is crucial to align these models with desired behaviors based on feedback from a multimodal judge. Despite their significance, current multimodal judges frequently undergo inadequate evaluation of their capabilities and limitations, potentially leading to misalignment and unsafe fine-tuning outcomes. To address this issue, we introduce MJ-Bench, a novel benchmark which incorporates a comprehensive preference dataset to evaluate multimodal judges in providing feedback for image generation models across four key perspectives: alignment, safety, image quality, and bias. Specifically, we evaluate a large variety of multimodal judges including smaller-sized CLIP-based scoring models, open-source VLMs (e.g. LLaVA family), and close-source VLMs (e.g. GPT-4o, Claude 3) on each decomposed subcategory of our preference dataset. Experiments reveal that close-source VLMs generally provide better feedback, with GPT-4o outperforming other judges in average. Compared with open-source VLMs, smaller-sized scoring models can provide better feedback regarding text-image alignment and image quality, while VLMs provide more accurate feedback regarding safety and generation bias due to their stronger reasoning capabilities. Further studies in feedback scale reveal that VLM judges can generally provide more accurate and stable feedback in natural language (Likert-scale) than numerical scales. Notably, human evaluations on end-to-end fine-tuned models using separate feedback from these multimodal judges provide similar conclusions, further confirming the effectiveness of MJ-Bench.
</details>

[📄 Paper](https://arxiv.org/pdf/2407.04842) | [🌐 Project Page](https://mj-bench.github.io/) | [💻 Code](https://github.com/MJ-Bench/MJ-Bench)

![MJ-BENCH](images/LLM/MJ-Bench.jpg)


### 13. μ-Bench: A Vision-Language Benchmark for Microscopy Understanding
**Authors:** Alejandro Lozano, Jeffrey Nirschl, James Burgess, Sanket Rajan Gupte, Yuhui Zhang, Alyssa Unell, Serena Yeung-Levy

<details span>
<summary><b>Abstract</b></summary>
Recent advances in microscopy have enabled the rapid generation of terabytes of image data in cell biology and biomedical research. Vision-language models (VLMs) offer a promising solution for large-scale biological image analysis, enhancing researchers' efficiency, identifying new image biomarkers, and accelerating hypothesis generation and scientific discovery. However, there is a lack of standardized, diverse, and large-scale vision-language benchmarks to evaluate VLMs' perception and cognition capabilities in biological image understanding. To address this gap, we introduce {\mu}-Bench, an expert-curated benchmark encompassing 22 biomedical tasks across various scientific disciplines (biology, pathology), microscopy modalities (electron, fluorescence, light), scales (subcellular, cellular, tissue), and organisms in both normal and abnormal states. We evaluate state-of-the-art biomedical, pathology, and general VLMs on {\mu}-Bench and find that: i) current models struggle on all categories, even for basic tasks such as distinguishing microscopy modalities; ii) current specialist models fine-tuned on biomedical data often perform worse than generalist models; iii) fine-tuning in specific microscopy domains can cause catastrophic forgetting, eroding prior biomedical knowledge encoded in their base model. iv) weight interpolation between fine-tuned and pre-trained models offers one solution to forgetting and improves general performance across biomedical tasks. We release {\mu}-Bench under a permissive license to accelerate the research and development of microscopy foundation models.
</details>

[📄 Paper](https://arxiv.org/pdf/2407.01791) | [🌐 Project Page](https://ale9806.github.io/uBench-website/) | [💻 Code](https://github.com/yeung-lab/Micro-Bench)

![μ-Bench](images/LLM/μ-Bench.jpg)

### 14. LLaMA-Omni: Seamless Speech Interaction with Large Language Models
**Authors:** Qingkai Fang, Shoutao Guo, Yan Zhou, Zhengrui Ma, Shaolei Zhang, Yang Feng

<details span>
<summary><b>Abstract</b></summary>
Models like GPT-4o enable real-time interaction with large language models (LLMs) through speech, significantly enhancing user experience compared to traditional text-based interaction. However, there is still a lack of exploration on how to build speech interaction models based on open-source LLMs. To address this, we propose LLaMA-Omni, a novel model architecture designed for low-latency and high-quality speech interaction with LLMs. LLaMA-Omni integrates a pretrained speech encoder, a speech adaptor, an LLM, and a streaming speech decoder. It eliminates the need for speech transcription, and can simultaneously generate text and speech responses directly from speech instructions with extremely low latency. We build our model based on the latest Llama-3.1-8B-Instruct model. To align the model with speech interaction scenarios, we construct a dataset named InstructS2S-200K, which includes 200K speech instructions and corresponding speech responses. Experimental results show that compared to previous speech-language models, LLaMA-Omni provides better responses in both content and style, with a response latency as low as 226ms. Additionally, training LLaMA-Omni takes less than 3 days on just 4 GPUs, paving the way for the efficient development of speech-language models in the future.
</details>

[📄 Paper](https://arxiv.org/pdf/2409.06666) | [💻 Code](https://github.com/ictnlp/LLaMA-Omni)

![LLaMA-Omni](images/LLM/LLaMA-Omni.jpg)

### 15. OneGen: Efficient One-Pass Unified Generation and Retrieval for LLMs
**Authors:** Jintian Zhang, Cheng Peng, Mengshu Sun, Xiang Chen, Lei Liang, Zhiqiang Zhang, Jun Zhou, Huajun Chen, Ningyu Zhang

<details span>
<summary><b>Abstract</b></summary>
Despite the recent advancements in Large Language Models (LLMs), which have significantly enhanced the generative capabilities for various NLP tasks, LLMs still face limitations in directly handling retrieval tasks. However, many practical applications demand the seamless integration of both retrieval and generation. This paper introduces a novel and efficient One-pass Generation and retrieval framework (OneGen), designed to improve LLMs' performance on tasks that require both generation and retrieval. The proposed framework bridges the traditionally separate training approaches for generation and retrieval by incorporating retrieval tokens generated autoregressively. This enables a single LLM to handle both tasks simultaneously in a unified forward pass. We conduct experiments on two distinct types of composite tasks, RAG and Entity Linking, to validate the pluggability, effectiveness, and efficiency of OneGen in training and inference. Furthermore, our results show that integrating generation and retrieval within the same context preserves the generative capabilities of LLMs while improving retrieval performance. To the best of our knowledge, OneGen is the first to enable LLMs to conduct vector retrieval during the generation.
</details>

[📄 Paper](https://arxiv.org/pdf/2409.05152) | [💻 Code](https://github.com/zjunlp/OneGen)

![LLaMA-Omni](images/LLM/OneGen.jpg)


### 16. Benchmarking Chinese Knowledge Rectification in Large Language Models
**Authors:** Tianhe Lu, Jizhan Fang, Yunzhi Yao, Xin Xu, Ningyu Zhang, Huajun Chen

<details span>
<summary><b>Abstract</b></summary>
While Large Language Models (LLMs) exhibit remarkable generative capabilities, they are not without flaws, particularly in the form of hallucinations. This issue is even more pronounced when LLMs are applied to specific languages and domains. For example, LLMs may generate nonsense information when handling Chinese ancient poetry, proverbs, or idioms, owing to the lack of specific knowledge. To this end, this paper introduces a benchmark for rectifying Chinese knowledge in LLMs via knowledge editing. Specifically, we introduce a new Chinese dataset, CKnowEdit, by collecting seven type of knowledge from various sources, including classical texts, idioms, and content from Baidu Tieba Ruozhiba, thereby accounting for the unique polyphony, antithesis, and logical constructs inherent in the Chinese language. Through the analysis of this dataset, we uncover the challenges faced by current LLMs in mastering Chinese. Furthermore, our evaluation of state-of-the-art knowledge editing techniques on this dataset unveil the substantial scope for advancement in the rectification of Chinese knowledge. 
</details>

[📄 Paper](https://arxiv.org/pdf/2409.05806) | [💻 Code](https://github.com/zjunlp/EasyEdit)

![LLaMA-Omni](images/LLM/CKnowEdit.jpg)

<!-- Diffusion part -->
## Diffusion

### 1. [CVPR'24] CityDreamer: Compositional Generative Model of Unbounded 3D Cities
**Authors**: Haozhe Xie, Zhaoxi Chen, Fangzhou Hong, Ziwei Liu

<details span>
<summary><b>Abstract</b></summary>
3D city generation is a desirable yet challenging task, since humans are more sensitive to structural distortions in urban environments. Additionally, generating 3D cities is more complex than 3D natural scenes since buildings, as objects of the same class, exhibit a wider range of appearances compared to the relatively consistent appearance of objects like trees in natural scenes. To address these challenges, we propose \textbf{CityDreamer}, a compositional generative model designed specifically for unbounded 3D cities. Our key insight is that 3D city generation should be a composition of different types of neural fields: 1) various building instances, and 2) background stuff, such as roads and green lands. Specifically, we adopt the bird's eye view scene representation and employ a volumetric render for both instance-oriented and stuff-oriented neural fields. The generative hash grid and periodic positional embedding are tailored as scene parameterization to suit the distinct characteristics of building instances and background stuff. Furthermore, we contribute a suite of CityGen Datasets, including OSM and GoogleEarth, which comprises a vast amount of real-world city imagery to enhance the realism of the generated 3D cities both in their layouts and appearances. CityDreamer achieves state-of-the-art performance not only in generating realistic 3D cities but also in localized editing within the generated cities.
</details>

[📄 Paper](https://arxiv.org/abs/2309.00610) | [💻 Code](https://github.com/hzxie/CityDreamer) 
![CityDreamer](images/Diffusion/CityDreamer_CVPR_2024.png)


### 2. [CVPR' 2024] Attention-Driven Training-Free Efficiency Enhancement of Diffusion Models
**Authors**: Hongjie Wang, Difan Liu, Yan Kang, Yijun Li, Zhe Lin, Niraj K. Jha, Yuchen Liu

<details span>
<summary><b>Abstract</b></summary>
Diffusion models (DMs) have exhibited superior performance in generating high-quality and diverse images. However this exceptional performance comes at the cost of expensive generation process particularly due to the heavily used attention module in leading models. Existing works mainly adopt a retraining process to enhance DM efficiency. This is computationally expensive and not very scalable. To this end we introduce the Attention-driven Training-free Efficient Diffusion Model (AT-EDM) framework that leverages attention maps to perform run-time pruning of redundant tokens without the need for any retraining. Specifically for single-denoising-step pruning we develop a novel ranking algorithm Generalized Weighted Page Rank (G-WPR) to identify redundant tokens and a similarity-based recovery method to restore tokens for the convolution operation. In addition we propose a Denoising-Steps-Aware Pruning (DSAP) approach to adjust the pruning budget across different denoising timesteps for better generation quality. Extensive evaluations show that AT-EDM performs favorably against prior art in terms of efficiency (e.g. 38.8% FLOPs saving and up to 1.53x speed-up over Stable Diffusion XL) while maintaining nearly the same FID and CLIP scores as the full model.
</details>

[📄 Paper](https://openaccess.thecvf.com/content/CVPR2024/papers/Wang_Attention-Driven_Training-Free_Efficiency_Enhancement_of_Diffusion_Models_CVPR_2024_paper.pdf) | [🌐 Project Page](https://atedm.github.io/)

![AT-EDM](images/Diffusion/AT-EDM_CVPR_2024.png)


### 3. [ECCV'24] AutoDIR: Automatic All-in-One Image Restoration with Latent Diffusion
**Authors**: Yitong Jiang, Zhaoyang Zhang, Tianfan Xue, Jinwei Gu

<details span>
<summary><b>Abstract</b></summary>
We present AutoDIR, an innovative all-in-one image restoration system incorporating latent diffusion. AutoDIR excels in its ability to automatically identify and restore images suffering from a range of unknown degradations. AutoDIR offers intuitive open-vocabulary image editing, empowering users to customize and enhance images according to their preferences. Specifically, AutoDIR consists of two key stages: a Blind Image Quality Assessment (BIQA) stage based on a semantic-agnostic vision-language model which automatically detects unknown image degradations for input images, an All-in-One Image Restoration (AIR) stage utilizes structural-corrected latent diffusion which handles multiple types of image degradations. Extensive experimental evaluation demonstrates that AutoDIR outperforms state-of-the-art approaches for a wider range of image restoration tasks. The design of AutoDIR also enables flexible user control (via text prompt) and generalization to new tasks as a foundation model of image restoration.
</details>

[📄 Paper](https://arxiv.org/abs/2310.10123) | [🌐 Project Page](https://atedm.github.io/) | [💻 Code](https://github.com/jiangyitong/AutoDIR) 

![AutoDIR](images/Diffusion/AutoDIR.jpg)


### 4. CrossViewDiff: A Cross-View Diffusion Model for Satellite-to-Street View Synthesis
**Authors:** Weijia Li, Jun He, Junyan Ye, Huaping Zhong, Zhimeng Zheng, Zilong Huang, Dahua Lin, Conghui He

<details span>
<summary><b>Abstract</b></summary>
Satellite-to-street view synthesis aims at generating a realistic street-view image from its corresponding satellite-view image. Although stable diffusion models have exhibit remarkable performance in a variety of image generation applications, their reliance on similar-view inputs to control the generated structure or texture restricts their application to the challenging cross-view synthesis task. In this work, we propose CrossViewDiff, a cross-view diffusion model for satellite-to-street view synthesis. To address the challenges posed by the large discrepancy across views, we design the satellite scene structure estimation and cross-view texture mapping modules to construct the structural and textural controls for street-view image synthesis. We further design a cross-view control guided denoising process that incorporates the above controls via an enhanced cross-view attention module. To achieve a more comprehensive evaluation of the synthesis results, we additionally design a GPT-based scoring method as a supplement to standard evaluation metrics. We also explore the effect of different data sources (e.g., text, maps, building heights, and multi-temporal satellite imagery) on this task. Results on three public cross-view datasets show that CrossViewDiff outperforms current state-of-the-art on both standard and GPT-based evaluation metrics, generating high-quality street-view panoramas with more realistic structures and textures across rural, suburban, and urban scenes.
</details>

[📄 Paper](https://arxiv.org/pdf/2408.01812) |  [🌐 Project Page](https://opendatalab.github.io/CrossViewDiff/)

![CrossViewDiff](images/Diffusion/CrossViewDiff_ArXiv2024.jpg)


### 5.  CrowdMoGen: Zero-Shot Text-Driven Collective Motion Generation
**Authors**: Xinying Guo, Mingyuan Zhang, Haozhe Xie, Chenyang Gu, Ziwei Liu

<details span>
<summary><b>Abstract</b></summary>
Crowd Motion Generation is essential in entertainment industries such as animation and games as well as in strategic fields like urban simulation and planning. This new task requires an intricate integration of control and generation to realistically synthesize crowd dynamics under specific spatial and semantic constraints, whose challenges are yet to be fully explored. On the one hand, existing human motion generation models typically focus on individual behaviors, neglecting the complexities of collective behaviors. On the other hand, recent methods for multi-person motion generation depend heavily on pre-defined scenarios and are limited to a fixed, small number of inter-person interactions, thus hampering their practicality. To overcome these challenges, we introduce CrowdMoGen, a zero-shot text-driven framework that harnesses the power of Large Language Model (LLM) to incorporate the collective intelligence into the motion generation framework as guidance, thereby enabling generalizable planning and generation of crowd motions without paired training data. Our framework consists of two key components: 1) Crowd Scene Planner that learns to coordinate motions and dynamics according to specific scene contexts or introduced perturbations, and 2) Collective Motion Generator that efficiently synthesizes the required collective motions based on the holistic plans. Extensive quantitative and qualitative experiments have validated the effectiveness of our framework, which not only fills a critical gap by providing scalable and generalizable solutions for Crowd Motion Generation task but also achieves high levels of realism and flexibility.
</details>

[📄 Paper](https://arxiv.org/abs/2407.06188) | [🌐 Project Page](https://gxyes.github.io/projects/CrowdMoGen.html) | [💻 Code](https://github.com/gxyes/CrowdMoGen?tab=readme-ov-file) 

![CrowdMoGen](images/Diffusion/CrowdMoGen_arxiv_2024.png)



### 6. [TGRS'24] DEMAE: Diffusion-Enhanced Masked Autoencoder for Hyperspectral Image Classification With Few Labeled Samples
**Authors**: Ziyu Li, Zhaohui Xue, Mingming Jia, Xiangyu Nie, Hao Wu, Mengxue Zhang, Hongjun Su

<details span>
<summary><b>Abstract</b></summary>
Unlike other deep learning (DL) models, Transformer has the ability to extract long-range dependency features from hyperspectral image (HSI) data. Masked autoencoder (MAE), which is based on Transformer architecture, employs a “mask-reconstruction” strategy for training, allowing the model to be effective for downstream tasks. However, existing MAE-based methods only apply spectral or spatial masking to HSI and reconstruct them for feature learning, which is too simplistic and insufficient for the model to learn robust features. Additionally, the issue of lacking labeled samples in HSI and the primary objective of MAE to reduce the reliance on labeled samples are often overlooked. To address these issues, we are inspired by diffusion-based representation learning and propose diffusion-enhanced MAE (DEMAE) for HSI classification with few labeled samples. First, an asymmetric encoder–decoder framework is constructed as the backbone by stacking both conditional and standard Transformer blocks. Second, we devise an auxiliary task aimed at simultaneous denoising and reconstruction, facilitating heuristic feature learning from HSI data. Third, the encoder of DEMAE is isolated for training with few labeled samples. Finally, the encoder is used for classification, and a novel signal-to-noise ratio enhanced (SNR-Enhanced) loss function is introduced to regularize the model training process. The performance of DEMAE is evaluated on four benchmark datasets, demonstrating its superiority in classification accuracy and mapping capabilities on unlabeled areas compared to existing state-of-the-art methods with few labeled samples.
</details>

[📄 Paper](https://ieeexplore.ieee.org/document/10639453) | [💻 Code](https://github.com/ZhaohuiXue/DEMAE) 

![DEMAE](images/Diffusion/DEMAE_TGRS2024.png)


### 7. [TPAMI'24] A New Brain Network Construction Paradigm for Brain Disorder Via Diffusion-Based Graph Contrastive Learning
**Authors**: Yongcheng Zong, Qiankun Zuo, Michael Kwok-Po Ng, Baiying Lei, Shuqiang Wang

<details span>
<summary><b>Abstract</b></summary>
Brain network analysis plays an increasingly important role in studying brain function and the exploring of disease mechanisms. However, existing brain network construction tools have some limitations, including dependency on empirical users, weak consistency in repeated experiments and time-consuming processes. In this work, a diffusion-based brain network pipeline, DGCL is designed for end-to-end construction of brain networks. Initially, the brain region-aware module (BRAM) precisely determines the spatial locations of brain regions by the diffusion process, avoiding subjective parameter selection. Subsequently, DGCL employs graph contrastive learning to optimize brain connections by eliminating individual differences in redundant connections unrelated to diseases, thereby enhancing the consistency of brain networks within the same group. Finally, the node-graph contrastive loss and classification loss jointly constrain the learning process of the model to obtain the reconstructed brain network, which is then used to analyze important brain connections. Validation on two datasets, ADNI and ABIDE, demonstrates that DGCL surpasses traditional methods and other deep learning models in predicting disease development stages. Significantly, the proposed model improves the efficiency and generalization of brain network construction. In summary, the proposed DGCL can be served as a universal brain network construction scheme, which can effectively identify important brain connections through generative paradigms and has the potential to provide disease interpretability support for neuroscience research.
</details>

[📄 Paper](https://arxiv.org/abs/2407.18329) 

![DGCL](images/Diffusion/DGCL_TPAMI_2024.png)


### 8. DiffTF++: 3D-aware Diffusion Transformer for Large-Vocabulary 3D Generation
**Authors**: Ziang Cao, Fangzhou Hong, Tong Wu, Liang Pan, Ziwei Liu

<details span>
<summary><b>Abstract</b></summary>
Generating diverse and high-quality 3D assets automatically poses a fundamental yet challenging task in 3D computer vision. Despite extensive efforts in 3D generation, existing optimization-based approaches struggle to produce large-scale 3D assets efficiently. Meanwhile, feed-forward methods often focus on generating only a single category or a few categories, limiting their generalizability. Therefore, we introduce a diffusion-based feed-forward framework to address these challenges with a single model. To handle the large diversity and complexity in geometry and texture across categories efficiently, we 1) adopt improved triplane to guarantee efficiency; 2) introduce the 3D-aware transformer to aggregate the generalized 3D knowledge with specialized 3D features; and 3) devise the 3D-aware encoder/decoder to enhance the generalized 3D knowledge. Building upon our 3D-aware Diffusion model with TransFormer, DiffTF, we propose a stronger version for 3D generation, i.e., DiffTF++. It boils down to two parts: multi-view reconstruction loss and triplane refinement. Specifically, we utilize multi-view reconstruction loss to fine-tune the diffusion model and triplane decoder, thereby avoiding the negative influence caused by reconstruction errors and improving texture synthesis. By eliminating the mismatch between the two stages, the generative performance is enhanced, especially in texture. Additionally, a 3D-aware refinement process is introduced to filter out artifacts and refine triplanes, resulting in the generation of more intricate and reasonable details. Extensive experiments on ShapeNet and OmniObject3D convincingly demonstrate the effectiveness of our proposed modules and the state-of-the-art 3D object generation performance with large diversity, rich semantics, and high quality.
</details>

[📄 Paper](https://arxiv.org/abs/2405.08055) 

![DiffTF++](images/Diffusion/DiffTF++_TPAMI_2024.png)


### 9. [CVPR'24] DPMesh: Exploiting Diffusion Prior for Occluded Human Mesh Recovery
**Authors**: Yixuan Zhu, Ao Li, Yansong Tang, Wenliang Zhao, Jie Zhou, Jiwen Lu

<details span>
<summary><b>Abstract</b></summary>
The recovery of occluded human meshes poses challenges for current methods due to the difficulty in extracting effective image features under severe occlusion. In this paper we introduce DPMesh an innovative framework for occluded human mesh recovery that capitalizes on the profound knowledge about object structure and spatial relationships embedded in a pre-trained text-to-image diffusion model. Unlike previous methods reliant on conventional backbones for vanilla feature extraction DPMesh seamlessly integrates the pre-trained denoising U-Net with potent priors as its image backbone and performs a single-step inference to provide occlusion-aware information. To enhance the perception capability for occluded poses DPMesh incorporates judicious guidance via condition injection which produces effective controls from 2D observations for the denoising U-Net. Furthermore we explore a dedicated noisy key-point reasoning approach to mitigate disturbances arising from occlusion and crowded scenarios. This strategy fully unleashes the perceptual capability of the diffusion prior thereby enhancing accuracy. Extensive quantitative and qualitative experiments affirm the efficacy of our framework as we outperform state-of-the-art methods on both occlusion-specific and standard datasets underscoring its ability to achieve precise and robust 3D human mesh recovery particularly in challenging scenarios involving occlusion and crowded scenes.
</details>

[📄 Paper](https://arxiv.org/abs/2404.01424) | [🌐 Project Page](https://eternalevan.github.io/dpmesh-proj) | [💻 Code](https://github.com/EternalEvan/DPMesh) 

![DPMesh](images/Diffusion/DPMesh_CVPR_2024_2.png)


### 9. MagicMan: Generative Novel View Synthesis of Humans with 3D-Aware Diffusion and Iterative Refinement
**Authors**: Yixuan Zhu, Ao Li, Yansong Tang, Wenliang Zhao, Jie Zhou, Jiwen Lu

<details span>
<summary><b>Abstract</b></summary>
Existing works in single-image human reconstruction suffer from weak generalizability due to insufficient training data or 3D inconsistencies for a lack of comprehensive multi-view knowledge. In this paper, we introduce MagicMan, a human-specific multi-view diffusion model designed to generate high-quality novel view images from a single reference image. As its core, we leverage a pre-trained 2D diffusion model as the generative prior for generalizability, with the parametric SMPL-X model as the 3D body prior to promote 3D awareness. To tackle the critical challenge of maintaining consistency while achieving dense multi-view generation for improved 3D human reconstruction, we first introduce hybrid multi-view attention to facilitate both efficient and thorough information interchange across different views. Additionally, we present a geometry-aware dual branch to perform concurrent generation in both RGB and normal domains, further enhancing consistency via geometry cues. Last but not least, to address ill-shaped issues arising from inaccurate SMPL-X estimation that conflicts with the reference image, we propose a novel iterative refinement strategy, which progressively optimizes SMPL-X accuracy while enhancing the quality and consistency of the generated multi-views. Extensive experimental results demonstrate that our method significantly outperforms existing approaches in both novel view synthesis and subsequent 3D human reconstruction tasks.
</details>

[📄 Paper](https://arxiv.org/abs/2408.14211) | [🌐 Project Page](https://thuhcsi.github.io/MagicMan/) | [💻 Code](https://github.com/thuhcsi/MagicMan?tab=readme-ov-file) 

![MagicMAN](images/Diffusion/MagicMAN_ArXiv2024.png)


### 10. [TIP'24] Multi-Condition Latent Diffusion Network for Scene-Aware Neural Human Motion Prediction
**Authors**: Xuehao Gao, Yang Yang, Yang Wu, Shaoyi Du, Guo-Jun Qi

<details span>
<summary><b>Abstract</b></summary>
Inferring 3D human motion is fundamental in many applications, including understanding human activity and analyzing one’s intention. While many fruitful efforts have been made to human motion prediction, most approaches focus on pose-driven prediction and inferring human motion in isolation from the contextual environment, thus leaving the body location movement in the scene behind. However, real-world human movements are goal-directed and highly influenced by the spatial layout of their surrounding scenes. In this paper, instead of planning future human motion in a “dark” room, we propose a Multi-Condition Latent Diffusion network (MCLD) that reformulates the human motion prediction task as a multi-condition joint inference problem based on the given historical 3D body motion and the current 3D scene contexts. Specifically, instead of directly modeling joint distribution over the raw motion sequences, MCLD performs a conditional diffusion process within the latent embedding space, characterizing the cross-modal mapping from the past body movement and current scene context condition embeddings to the future human motion embedding. Extensive experiments on large-scale human motion prediction datasets demonstrate that our MCLD achieves significant improvements over the state-of-the-art methods on both realistic and diverse predictions.
</details>

[📄 Paper](https://arxiv.org/abs/2405.18700)

![MCLD](images/Diffusion/MCLD_TIP2024.png)


### 11. [TIP'23] Multi-View Diffusion Process for Spectral Clustering and Image Retrieval
**Authors**: Qilin Li , Senjian An, Ling Li , Wanquan Liu, and Yanda Shao

<details span>
<summary><b>Abstract</b></summary>
This paper presents a novel approach to multi-view graph learning that combines weight learning and graph learning in an alternating optimization framework. Multi-view graph learning refers to the problem of constructing a unified affinity graph using heterogeneous sources of data representation, which is a popular technique in many learning systems where no prior knowledge of data distribution is available. Our approach is based on a fusion-and-diffusion strategy, in which multiple affinity graphs are fused together via a weight learning scheme based on the unsupervised graph smoothness and utilised as a consensus prior to the diffusion. We propose a novel multi-view diffusion process that learns a manifold-aware affinity graph by propagating affinities on tensor product graphs, leveraging high-order contextual information to enhance pairwise affinities. In contrast to existing multi-view graph learning approaches, our approach is not limited by the quality of initial graphs or the assumption of a latent common subspace among multiple views. Instead, our approach is able to identify the consistency among views and fuse multiple graphs adaptively. We formulate both weight learning and diffusion-based affinity learning in a unified framework and propose an alternating optimization solver that is guaranteed to converge. The proposed approach is applied to image retrieval and clustering tasks on 16 real-world datasets. Extensive experimental results demonstrate that our approach outperforms state-of-the-art methods for both retrieval and clustering on 13 out of 16 datasets.
</details>

[📄 Paper](https://ieeexplore.ieee.org/abstract/document/10214517) 

![MVD](images/Diffusion/MVD_TIP_2023.png)


### 12. [CVPR'24 HighLight] Taming Stable Diffusion for Text to 360° Panorama Image Generation
**Authors**: Cheng Zhang, Qianyi Wu, Camilo Cruz Gambardella, Xiaoshui Huang, Dinh Phung, Wanli Ouyang, Jianfei Cai

<details span>
<summary><b>Abstract</b></summary>
Generative models, e.g., Stable Diffusion, have enabled the creation of photorealistic images from text prompts. Yet, the generation of 360-degree panorama images from text remains a challenge, particularly due to the dearth of paired text-panorama data and the domain gap between panorama and perspective images. In this paper, we introduce a novel dual-branch diffusion model named PanFusion to generate a 360-degree image from a text prompt. We leverage the stable diffusion model as one branch to provide prior knowledge in natural image generation and register it to another panorama branch for holistic image generation. We propose a unique cross-attention mechanism with projection awareness to minimize distortion during the collaborative denoising process. Our experiments validate that PanFusion surpasses existing methods and, thanks to its dual-branch structure, can integrate additional constraints like room layout for customized panorama outputs. 
</details>

[📄 Paper](https://arxiv.org/abs/2404.07949) | [🌐 Project Page](https://chengzhag.github.io/publication/panfusion/) | [💻 Code](https://github.com/chengzhag/PanFusion) 

![PanFusion](images/Diffusion/PanFusion_CVPR_2024.png)


### 13. [CVPR'24] SDDGR: Stable Diffusion-based Deep Generative Replay for Class Incremental Object Detection
**Authors**: Junsu Kim, Hoseong Cho, Jihyeon Kim, Yihalem Yimolal Tiruneh, Seungryul Baek

<details span>
<summary><b>Abstract</b></summary>
In the field of class incremental learning (CIL), generative replay has become increasingly prominent as a method to mitigate the catastrophic forgetting, alongside the continuous improvements in generative models. However, its application in class incremental object detection (CIOD) has been significantly limited, primarily due to the complexities of scenes involving multiple labels. In this paper, we propose a novel approach called stable diffusion deep generative replay (SDDGR) for CIOD. Our method utilizes a diffusion-based generative model with pre-trained text-to-diffusion networks to generate realistic and diverse synthetic images. SDDGR incorporates an iterative refinement strategy to produce high-quality images encompassing old classes. Additionally, we adopt an L2 knowledge distillation technique to improve the retention of prior knowledge in synthetic images. Furthermore, our approach includes pseudo-labeling for old objects within new task images, preventing misclassification as background elements. Extensive experiments on the COCO 2017 dataset demonstrate that SDDGR significantly outperforms existing algorithms, achieving a new state-of-the-art in various CIOD scenarios. The source code will be made available to the public.
</details>

[📄 Paper](https://arxiv.org/abs/2402.17323) 

![SDDGR](images/Diffusion/SDDGR_CVPR_2024.png)

### 14. [CVPR'24] SemCity: Semantic Scene Generation with Triplane Diffusion
**Authors**: Jumin Lee, Sebin Lee, Changho Jo, Woobin Im, Juhyeong Seon, Sung-Eui Yoon

<details span>
<summary><b>Abstract</b></summary>
We present "SemCity," a 3D diffusion model for semantic scene generation in real-world outdoor environments. Most 3D diffusion models focus on generating a single object, synthetic indoor scenes, or synthetic outdoor scenes, while the generation of real-world outdoor scenes is rarely addressed. In this paper, we concentrate on generating a real-outdoor scene through learning a diffusion model on a real-world outdoor dataset. In contrast to synthetic data, real-outdoor datasets often contain more empty spaces due to sensor limitations, causing challenges in learning real-outdoor distributions. To address this issue, we exploit a triplane representation as a proxy form of scene distributions to be learned by our diffusion model. Furthermore, we propose a triplane manipulation that integrates seamlessly with our triplane diffusion model. The manipulation improves our diffusion model's applicability in a variety of downstream tasks related to outdoor scene generation such as scene inpainting, scene outpainting, and semantic scene completion refinements. In experimental results, we demonstrate that our triplane diffusion model shows meaningful generation results compared with existing work in a real-outdoor dataset, SemanticKITTI. We also show our triplane manipulation facilitates seamlessly adding, removing, or modifying objects within a scene. Further, it also enables the expansion of scenes toward a city-level scale. Finally, we evaluate our method on semantic scene completion refinements where our diffusion model enhances predictions of semantic scene completion networks by learning scene distribution.
</details>

[📄 Paper](https://arxiv.org/abs/2403.07773) | [🌐 Project Page](https://sglab.kaist.ac.kr/SemCity/) | [💻 Code](https://github.com/zoomin-lee/SemCity) 

![SemCity](images/Diffusion/SemCity_CVPR_2024.png)


### 15. [IJCV'24] InterGen: Diffusion-based Multi-human Motion Generation under Complex Interactions
**Authors**: Han Liang, Wenqian Zhang, Wenxuan Li, Jingyi Yu, Lan Xu

<details span>
<summary><b>Abstract</b></summary>
We have recently seen tremendous progress in diffusion advances for generating realistic human motions. Yet, they largely disregard the multi-human interactions. In this paper, we present InterGen, an effective diffusion-based approach that incorporates human-to-human interactions into the motion diffusion process, which enables layman users to customize high-quality two-person interaction motions, with only text guidance. We first contribute a multimodal dataset, named InterHuman. It consists of about 107M frames for diverse two-person interactions, with accurate skeletal motions and 23,337 natural language descriptions. For the algorithm side, we carefully tailor the motion diffusion model to our two-person interaction setting. To handle the symmetry of human identities during interactions, we propose two cooperative transformer-based denoisers that explicitly share weights, with a mutual attention mechanism to further connect the two denoising processes. Then, we propose a novel representation for motion input in our interaction diffusion model, which explicitly formulates the global relations between the two performers in the world frame. We further introduce two novel regularization terms to encode spatial relations, equipped with a corresponding damping scheme during the training of our interaction diffusion model. Extensive experiments validate the effectiveness and generalizability of InterGen. Notably, it can generate more diverse and compelling two-person motions than previous methods and enables various downstream applications for human interactions.
</details>

[📄 Paper](https://arxiv.org/abs/2304.05684) | [🌐 Project Page](https://tr3e.github.io/intergen-page/) | [💻 Code](https://github.com/tr3e/InterGen) 

![InterGen](images/Diffusion/InterGen_IJCV_2024.png)


### 16. [TGRS'24] Diffusion-Based Continuous Feature Representation for Infrared Small-Dim Target Detection
**Authors**: Fan, Linyu and Wang, Yingying and Hu, Guoliang and Li, Feifei and Dong, Yuhang and Zheng, Hui and Lin, Changqing and Huang, Yue and Ding, Xinghao

<details span>
<summary><b>Abstract</b></summary>
Infrared small-dim target detection (ISDTD) plays a pivotal role in missions involving rescue, surveillance, and early warning systems. Despite remarkable strides made by existing methods, certain limitations still hinder the detection accuracy, including deficiency in high-resolution (HR) representation, inadequacy in addressing dim targets, and difficulty in tackling low-contrast targets against complex backgrounds. To overcome these limitations, we propose a diffusion-based continuous feature representation network (DCFR-Net), comprising two crucial branches: diffusion-based continuous HR feature representation (DCHFR) and ISDTD. Specifically, to precisely capture extremely small target contours, DCHFR integrates implicit neural representation (INR) into a conditional denoising diffusion model, super-resolving infrared targets in a self-supervised strategy. ISDTD leverages the shared encoder from DCHFR to construct HR feature representation, which is fed into multiscale implicit feature alignment (MIFA) and spatial-frequency feature interaction (SFFI). To alleviate the impact of dim and vulnerable targets, MIFA delicately aggregates different-layer features in a resolution-free manner. Furthermore, to enhance the contrast between infrared targets and intricate backgrounds, SFFI achieves profound SFFI and global-local receptive field mixture. Extensive experiments conducted on three challenging datasets of NUAA-SIRST, IRSTD-1k, and NUDT-SIRST reveal that our DCFR-Net outperforms the state-of-the-art (SOTA) methods, demonstrating the superiority and robustness of our approach in ISDTD.
</details>

[📄 Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10510431) | [💻 Code](https://github.com/flyannie/DCFR-Net) 

![DCFRNET](images/Diffusion/DCFRNET_TGRS2024.png)


### 17. [IJCV'24] InterGen: Diffusion-based Multi-human Motion Generation under Complex Interactions
**Authors**: Han Liang, Wenqian Zhang, Wenxuan Li, Jingyi Yu, Lan Xu

<details span>
<summary><b>Abstract</b></summary>
We have recently seen tremendous progress in diffusion advances for generating realistic human motions. Yet, they largely disregard the multi-human interactions. In this paper, we present InterGen, an effective diffusion-based approach that incorporates human-to-human interactions into the motion diffusion process, which enables layman users to customize high-quality two-person interaction motions, with only text guidance. We first contribute a multimodal dataset, named InterHuman. It consists of about 107M frames for diverse two-person interactions, with accurate skeletal motions and 23,337 natural language descriptions. For the algorithm side, we carefully tailor the motion diffusion model to our two-person interaction setting. To handle the symmetry of human identities during interactions, we propose two cooperative transformer-based denoisers that explicitly share weights, with a mutual attention mechanism to further connect the two denoising processes. Then, we propose a novel representation for motion input in our interaction diffusion model, which explicitly formulates the global relations between the two performers in the world frame. We further introduce two novel regularization terms to encode spatial relations, equipped with a corresponding damping scheme during the training of our interaction diffusion model. Extensive experiments validate the effectiveness and generalizability of InterGen. Notably, it can generate more diverse and compelling two-person motions than previous methods and enables various downstream applications for human interactions.
</details>

[📄 Paper](https://arxiv.org/abs/2304.05684) | [🌐 Project Page](https://tr3e.github.io/intergen-page/) | [💻 Code](https://github.com/tr3e/InterGen) 

![InterGen](images/Diffusion/InterGen_IJCV_2024.png)


### 18. UrbanWorld: An Urban World Model for 3D City Generation
**Authors**: Yu Shang, Jiansheng Chen, Hangyu Fan, Jingtao Ding, Jie Feng, Yong Li

<details span>
<summary><b>Abstract</b></summary>
Cities, as the most fundamental environment of human life, encompass diverse physical elements such as buildings, roads and vegetation with complex interconnection. Crafting realistic, interactive 3D urban environments plays a crucial role in constructing AI agents capable of perceiving, decision-making, and acting like humans in real-world environments. However, creating high-fidelity 3D urban environments usually entails extensive manual labor from designers, involving intricate detailing and accurate representation of complex urban features. Therefore, how to accomplish this in an automatical way remains a longstanding challenge. Toward this problem, we propose UrbanWorld, the first generative urban world model that can automatically create a customized, realistic and interactive 3D urban world with flexible control conditions. UrbanWorld incorporates four key stages in the automatical crafting pipeline: 3D layout generation from openly accessible OSM data, urban scene planning and designing with a powerful urban multimodal large language model (Urban MLLM), controllable urban asset rendering with advanced 3D diffusion techniques, and finally the MLLM-assisted scene refinement. The crafted high-fidelity 3D urban environments enable realistic feedback and interactions for general AI and machine perceptual systems in simulations. We are working on contributing UrbanWorld as an open-source and versatile platform for evaluating and improving AI abilities in perception, decision-making, and interaction in realistic urban environments.
</details>

[📄 Paper](https://arxiv.org/abs/2407.11965) 

![UrbanWorld](images/Diffusion/UrbanWorld_ArXiv2024.png)


### 19. [CVPR'24] FreeControl: Training-Free Spatial Control of Any Text-to-Image Diffusion Model with Any Condition
**Authors**: Sicheng Mo, Fangzhou Mu, Kuan Heng Lin, Yanli Liu, Bochen Guan, Yin Li, Bolei Zhou

<details span>
<summary><b>Abstract</b></summary>
Recent approaches such as ControlNet offer users fine-grained spatial control over text-to-image (T2I) diffusion models. However auxiliary modules have to be trained for each spatial condition type model architecture and checkpoint putting them at odds with the diverse intents and preferences a human designer would like to convey to the AI models during the content creation process. In this work we present FreeControl a training-free approach for controllable T2I generation that supports multiple conditions architectures and checkpoints simultaneously. FreeControl enforces structure guidance to facilitate the global alignment with a guidance image and appearance guidance to collect visual details from images generated without control. Extensive qualitative and quantitative experiments demonstrate the superior performance of FreeControl across a variety of pre-trained T2I models. In particular FreeControl enables convenient training-free control over many different architectures and checkpoints allows the challenging input conditions on which most of the existing training-free methods fail and achieves competitive synthesis quality compared to training-based approaches.
</details>

[📄 Paper](https://arxiv.org/abs/2312.07536) | [🌐 Project Page](https://genforce.github.io/freecontrol//) | [💻 Code](https://github.com/genforce/freecontrol) 

![FreeControl](images/Diffusion/FreeControl_CVPR2024.png)


### 20. [TCCN'24] Generative AI-driven Semantic Communication Networks: Architecture, Technologies and Applications
**Authors**: Sicheng Mo, Fangzhou Mu, Kuan Heng Lin, Yanli Liu, Bochen Guan, Yin Li, Bolei Zhou

<details span>
<summary><b>Abstract</b></summary>
Generative artificial intelligence (GAI) has emerged as a rapidly burgeoning field demonstrating significant potential in creating diverse content intelligently and automatically. To support such artificial intelligence-generated content (AIGC) services, future communication systems must fulfill stringent requirements, including high data rates, throughput, and low latency, while efficiently utilizing limited spectrum resources. Semantic communication (SemCom) has been deemed as a revolutionary communication scheme to tackle this challenge by conveying the meaning of messages instead of bit reproduction. GAI algorithms serve as the foundation for enabling intelligent and efficient SemCom systems in terms of model pre-training and fine-tuning, knowledge base construction, and resource allocation. Conversely, SemCom can provide AIGC services with low latency and high reliability due to its ability to perform semantic-aware encoding and compression of data, as well as knowledge-and context-based reasoning. In this survey, we break new ground by investigating the architecture, wireless communication schemes, and network management of GAI-driven SemCom networks. We first introduce a novel architecture for GAI-driven SemCom networks, comprising the data plane, physical infrastructure, and network control plane. In turn, we provide an in-depth analysis of the transceiver design and semantic effectiveness calculation of end-to-end GAI-driven SemCom systems. Subsequently, we present innovative generation level and knowledge management strategies in the proposed networks, including knowledge construction, update, and sharing, ensuring accurate and timely knowledge-based reasoning. Finally, we explore several promising use cases, i.e., autonomous driving, smart cities, and the Metaverse, to provide a comprehensive understanding and future direction of GAI-driven SemCom networks.
</details>

[📄 Paper](https://arxiv.org/abs/2401.00124) 

![GAI-driven](images/Diffusion/GAI-driven_TCCN2024.png)

### 21. [ECCV'24] StructLDM: Structured Latent Diffusion for 3D Human Generation
**Authors**: Tao Hu, Fangzhou Hong,  Ziwei Liu

<details span>
<summary><b>Abstract</b></summary>
Recent 3D human generative models have achieved remarkable progress by learning 3D-aware GANs from 2D images. However, existing 3D human generative methods model humans in a compact 1D latent space, ignoring the articulated structure and semantics of human body topology. In this paper, we explore more expressive and higher-dimensional latent space for 3D human modeling and propose StructLDM, a diffusion-based unconditional 3D human generative model that is learned from 2D images. StructLDM solves the challenges imposed due to the high-dimensional growth of latent space with three key designs: 1) A semantic structured latent space defined on the dense surface manifold of a statistical human body template. 2) A structured 3D-aware auto-decoder that factorizes the global latent space into several semantic body parts parameterized by a set of conditional structured local NeRFs anchored to the body template, which embeds the properties learned from the 2D training data and can be decoded to render view-consistent humans under different poses and clothing styles. 3) A structured latent diffusion model for generative human appearance sampling. Extensive experiments validate StructLDM's state-of-the-art generation performance and illustrate the expressiveness of the structured latent space over the well-adopted 1D latent space. Notably, StructLDM enables different levels of controllable 3D human generation and editing, including pose/view/shape control, and high-level tasks including compositional generations, part-aware clothing editing, 3D virtual try-on, etc.
</details>

[📄 Paper](https://arxiv.org/abs/2404.01241) | [🌐 Project Page](https://taohuumd.github.io/projects/StructLDM/) | [💻 Code](https://github.com/TaoHuUMD/StructLDM) 

![StructLDM](images/Diffusion/StructLDM_ECCV2024.png)


### 22. [ECCV'24] HyperDreamer: Hyper-Realistic 3D Content Generation and Editing from a Single Image
**Authors**: Tong Wu, Zhibing Li, Shuai Yang, Pan Zhang, Xinggang Pan, Jiaqi Wang, Dahua Lin, Ziwei Liu

<details span>
<summary><b>Abstract</b></summary>
3D content creation from a single image is a long-standing yet highly desirable task. Recent advances introduce 2D diffusion priors, yielding reasonable results. However, existing methods are not hyper-realistic enough for post-generation usage, as users cannot view, render and edit the resulting 3D content from a full range. To address these challenges, we introduce HyperDreamer with several key designs and appealing properties: 1) Viewable: 360 degree mesh modeling with high-resolution textures enables the creation of visually compelling 3D models from a full range of observation points. 2) Renderable: Fine-grained semantic segmentation and data-driven priors are incorporated as guidance to learn reasonable albedo, roughness, and specular properties of the materials, enabling semantic-aware arbitrary material estimation. 3) Editable: For a generated model or their own data, users can interactively select any region via a few clicks and efficiently edit the texture with text-based guidance. Extensive experiments demonstrate the effectiveness of HyperDreamer in modeling region-aware materials with high-resolution textures and enabling user-friendly editing. We believe that HyperDreamer holds promise for advancing 3D content creation and finding applications in various domains.
</details>

[📄 Paper](https://arxiv.org/abs/2312.04543) | [🌐 Project Page](https://ys-imtech.github.io/HyperDreamer/) | [💻 Code](https://github.com/wutong16/HyperDreamer) 

![HyperDreamer_SIGGRAPH_Asia2024](images/Diffusion/HyperDreamer_SIGGRAPH_Asia2024.png)

### 23. [ECCV'24] AnyHome: Open-Vocabulary Generation of Structured and Textured 3D Homes
**Authors**: Rao Fu, Zehao Wen, Zichen Liu, Srinath Sridhar

<details span>
<summary><b>Abstract</b></summary>
Inspired by cognitive theories, we introduce AnyHome, a framework that translates any text into well-structured and textured indoor scenes at a house-scale. By prompting Large Language Models (LLMs) with designed templates, our approach converts provided textual narratives into amodal structured representations. These representations guarantee consistent and realistic spatial layouts by directing the synthesis of a geometry mesh within defined constraints. A Score Distillation Sampling process is then employed to refine the geometry, followed by an egocentric inpainting process that adds lifelike textures to it. AnyHome stands out with its editability, customizability, diversity, and realism. The structured representations for scenes allow for extensive editing at varying levels of granularity. Capable of interpreting texts ranging from simple labels to detailed narratives, AnyHome generates detailed geometries and textures that outperform existing methods in both quantitative and qualitative measures.
</details>

[📄 Paper](https://arxiv.org/abs/2312.06644) 
![AnyHome_ECCV2024](images/Diffusion/AnyHome_ECCV2024.png)


<!-- 3DGS part -->
## 3D gaussian splatting

### 1. [ECCV'24 Oral] LGM: Large Multi-View Gaussian Model for High-Resolution 3D Content Creation
**Authors:** Jiaxiang Tang, Zhaoxi Chen, Xiaokang Chen, Tengfei Wang, Gang Zeng, Ziwei Liu
<details span>
<summary><b>Abstract</b></summary>
3D content creation has achieved significant progress in terms
of both quality and speed. Although current feed-forward models can
produce 3D objects in seconds, their resolution is constrained by the
intensive computation required during training. In this paper, we introduce Large Multi-View Gaussian Model (LGM), a novel framework designed to generate high-resolution 3D models from text prompts
or single-view images. Our key insights are two-fold: (1) 3D Representation: We propose multi-view Gaussian features as an efficient yet powerful representation, which can then be fused together for differentiable
rendering. (2) 3D Backbone: We present an asymmetric U-Net as a
high-throughput backbone operating on multi-view images, which can be produced from text or single-view image input by leveraging multi-view
diffusion models. Extensive experiments demonstrate the high fidelity
and efficiency of our approach. Notably, we maintain the fast speed to
generate 3D objects within 5 seconds while boosting the training resolution to 512, thereby achieving high-resolution 3D content generation.
</details>

[📄 Paper](https://arxiv.org/pdf/2402.05054.pdf) | [🌐 Project Page](https://me.kiui.moe/lgm/) | [💻 Code](https://github.com/3DTopia/LGM) 

![LGM](images/3DGS/LGM.jpg)

### 2. GALA3D: Towards Text-to-3D Complex Scene Generation via Layout-guided Generative Gaussian Splatting
**Authors**: Xiaoyu Zhou, Xingjian Ran, Yajiao Xiong, Jinlin He, Zhiwei Lin, Yongtao Wang, Deqing Sun, Ming-Hsuan Yang  

<details span>
<summary><b>Abstract</b></summary>
We present GALA3D, generative 3D GAussians with LAyout-guided control, for effective compositional text-to-3D generation. We first utilize large language models (LLMs) to generate the initial layout and introduce a layout-guided 3D Gaussian representation for 3D content generation with adaptive geometric constraints. We then propose an object-scene compositional optimization mechanism with conditioned diffusion to collaboratively generate realistic 3D scenes with consistent geometry, texture, scale, and accurate interactions among multiple objects while simultaneously adjusting the coarse layout priors extracted from the LLMs to align with the generated scene. Experiments show that GALA3D is a user-friendly, end-to-end framework for state-of-the-art scene-level 3D content generation and controllable editing while ensuring the high fidelity of object-level entities within the scene.
</details>

[📄 Paper](https://arxiv.org/pdf/2402.07207.pdf) | [🌐 Project Page](https://gala3d.github.io/) | [💻 Code (not yet)](https://github.com/VDIGPKU/GALA3D)

![GALA3D](images/3DGS/GALA3D.jpg)

### 3. Hyper-3DG: Text-to-3D Gaussian Generation via Hypergraph
**Authors**: Donglin Di, Jiahui Yang, Chaofan Luo, Zhou Xue, Wei Chen, Xun Yang, Yue Gao 

<details span>
<summary><b>Abstract</b></summary>
Text-to-3D generation represents an exciting field that has seen rapid advancements, facilitating the transformation of textual descriptions into detailed 3D models. However, current progress often neglects the intricate high-order correlation of geometry and texture within 3D objects, leading to challenges such as over-smoothness, over-saturation and the Janus problem. In this work, we propose a method named ``3D Gaussian Generation via Hypergraph (Hyper-3DG)'', designed to capture the sophisticated high-order correlations present within 3D objects. Our framework is anchored by a well-established mainflow and an essential module, named ``Geometry and Texture Hypergraph Refiner (HGRefiner)''. This module not only refines the representation of 3D Gaussians but also accelerates the update process of these 3D Gaussians by conducting the Patch-3DGS Hypergraph Learning on both explicit attributes and latent visual features. Our framework allows for the production of finely generated 3D objects within a cohesive optimization, effectively circumventing degradation. Extensive experimentation has shown that our proposed method significantly enhances the quality of 3D generation while incurring no additional computational overhead for the underlying framework.
</details>

[📄 Paper](https://arxiv.org/pdf/2403.09236.pdf) | [💻 Code (not yet)](https://github.com/yjhboy/Hyper3DG)

![Hyper-3DG](images/3DGS/Hyper-3DG.jpg)


### 4. FDGaussian: Fast Gaussian Splatting from Single Image via Geometric-aware Diffusion Model
**Authors:** Qijun Feng, Zhen Xing, Zuxuan Wu, Yu-Gang Jiang
<details span>
<summary><b>Abstract</b></summary>
Reconstructing detailed 3D objects from single-view images
remains a challenging task due to the limited information available. In
this paper, we introduce FDGaussian, a novel two-stage framework for
single-image 3D reconstruction. Recent methods typically utilize pretrained 2D diffusion models to generate plausible novel views from the
input image, yet they encounter issues with either multi-view inconsistency or lack of geometric fidelity. To overcome these challenges, we propose an orthogonal plane decomposition mechanism to extract 3D geometric features from the 2D input, enabling the generation of consistent
multi-view images. Moreover, we further accelerate the state-of-the-art
Gaussian Splatting incorporating epipolar attention to fuse images from
different viewpoints. We demonstrate that FDGaussian generates images
with high consistency across different views and reconstructs high-quality
3D objects, both qualitatively and quantitatively. 
</details>

[📄 Paper](https://arxiv.org/pdf/2403.10242.pdf) | [🌐 Project Page](https://qjfeng.net/FDGaussian) 

![FDGaussian](images/3DGS/FDGaussian.jpg)

### 5. STAG4D: Spatial-Temporal Anchored Generative 4D Gaussians
**Authors**: Yifei Zeng, Yanqin Jiang, Siyu Zhu, Yuanxun Lu, Youtian Lin, Hao Zhu, Weiming Hu, Xun Cao, Yao Yao  

<details span>
<summary><b>Abstract</b></summary>
Recent progress in pre-trained diffusion models and 3D generation have spurred interest in 4D content creation. However, achieving high-fidelity 4D generation with spatial-temporal consistency remains a challenge. In this work, we propose STAG4D, a novel framework that combines pre-trained diffusion models with dynamic 3D Gaussian splatting for high-fidelity 4D generation. Drawing inspiration from 3D generation techniques, we utilize a multi-view diffusion model to initialize multi-view images anchoring on the input video frames, where the video can be either real-world captured or generated by a video diffusion model. To ensure the temporal consistency of the multi-view sequence initialization, we introduce a simple yet effective fusion strategy to leverage the first frame as a temporal anchor in the self-attention computation. With the almost consistent multi-view sequences, we then apply the score distillation sampling to optimize the 4D Gaussian point cloud. The 4D Gaussian spatting is specially crafted for the generation task, where an adaptive densification strategy is proposed to mitigate the unstable Gaussian gradient for robust optimization. Notably, the proposed pipeline does not require any pre-training or fine-tuning of diffusion networks, offering a more accessible and practical solution for the 4D generation task. Extensive experiments demonstrate that our method outperforms prior 4D generation works in rendering quality, spatial-temporal consistency, and generation robustness, setting a new state-of-the-art for 4D generation from diverse inputs, including text, image, and video. 
</details>

[📄 Paper](https://arxiv.org/pdf/2403.14939) | [🌐 Project Page](https://nju-3dv.github.io/projects/STAG4D/) | [💻 Code](https://github.com/zeng-yifei/STAG4D) | [🎥 Video](https://www.youtube.com/watch?v=YJkFMIV2OyQ) 

![STAG4D](images/3DGS/STAG4D.jpg)


### 6. [CVPR '24] Animatable and Relightable Gaussians for High-fidelity Human Avatar Modeling 
**Authors**: Zhe Li, Yipengjing Sun, Zerong Zheng, Lizhen Wang, Shengping Zhang, Yebin Liu
<details span>
<summary><b>Abstract</b></summary>
Modeling animatable human avatars from RGB
videos is a long-standing and challenging problem. Recent works
usually adopt MLP-based neural radiance fields (NeRF) to
represent 3D humans, but it remains difficult for pure MLPs
to regress pose-dependent garment details. To this end, we
introduce Animatable Gaussians, a new avatar representation
that leverages powerful 2D CNNs and 3D Gaussian splatting
to create high-fidelity avatars. To associate 3D Gaussians with
the animatable avatar, we learn a parametric template from the
input videos, and then parameterize the template on two front
& back canonical Gaussian maps where each pixel represents a
3D Gaussian. The learned template is adaptive to the wearing
garments for modeling looser clothes like dresses. Such templateguided 2D parameterization enables us to employ a powerful
StyleGAN-based CNN to learn the pose-dependent Gaussian
maps for modeling detailed dynamic appearances. Furthermore,
we introduce a pose projection strategy for better generalization
given novel poses. To tackle the realistic relighting of animatable
avatars, we introduce physically-based rendering into the avatar
representation for decomposing avatar materials and environment illumination. Overall, our method can create lifelike avatars
with dynamic, realistic, generalized and relightable appearances.
Experiments show that our method outperforms other state-ofthe-art approaches.
</details>

  [📄 Paper](https://arxiv.org/pdf/2311.16096.pdf) | [🌐 Project Page](https://animatable-gaussians.github.io/relight/) | [💻 Code ](https://github.com/lizhe00/AnimatableGaussians)

![Animatable Gaussians](images/3DGS/Animatable_and_Relightable_Gaussians.jpg)

### 7. HoloDreamer: Holistic 3D Panoramic World Generation from Text Descriptions
**Author:** Haiyang Zhou, Xinhua Cheng, Wangbo Yu, Yonghong Tian, Li Yuan
<details span>
<summary><b>Abstract</b></summary>
3D scene generation is in high demand across various domains, including virtual reality, gaming, and the film industry. Owing to the powerful generative capabilities of text-to-image diffusion models that provide reliable priors, the creation of 3D scenes using only text prompts has become viable, thereby significantly advancing researches in text-driven 3D scene generation. In order to obtain multiple-view supervision from 2D diffusion models, prevailing methods typically employ the diffusion model to generate an initial local image, followed by iteratively outpainting the local image using diffusion models to gradually generate scenes. Nevertheless, these outpainting-based approaches prone to produce global inconsistent scene generation results without high degree of completeness, restricting their broader applications. To tackle these problems, we introduce HoloDreamer, a framework that first generates high-definition panorama as a holistic initialization of the full 3D scene, then leverage 3D Gaussian Splatting (3D-GS) to quickly reconstruct the 3D scene, thereby facilitating the creation of view-consistent and fully enclosed 3D scenes. Specifically, we propose Stylized Equirectangular Panorama Generation, a pipeline that combines multiple diffusion models to enable stylized and detailed equirectangular panorama generation from complex text prompts. Subsequently, Enhanced Two-Stage Panorama Reconstruction is introduced, conducting a two-stage optimization of 3D-GS to inpaint the missing region and enhance the integrity of the scene. Comprehensive experiments demonstrated that our method outperforms prior works in terms of overall visual consistency and harmony as well as reconstruction quality and rendering robustness when generating fully enclosed scenes.
</details>

[📄 Paper](https://arxiv.org/abs/2407.15187) | [🌐 Project Page](https://zhouhyocean.github.io/holodreamer/) | [💻 Code (not yet)](https://zhouhyocean.github.io/holodreamer/)

![HoloDreamer](images/3DGS/HoloDreamer.jpg)


### 8. LucidDreamer: Domain-free Generation of 3D Gaussian Splatting Scenes
**Authors:** Jaeyoung Chung, Suyoung Lee, Hyeongjin Nam, Jaerin Lee, Kyoung Mu Lee
<details span>
<summary><b>Abstract</b></summary>
With the widespread usage of VR devices and contents, demands for 3D scene generation techniques become more popular. Existing 3D scene generation models, however, limit the target scene to specific domain, primarily due to their training strategies using 3D scan dataset that is far from the real-world. To address such limitation, we propose LucidDreamer, a domain-free scene generation pipeline by fully leveraging the power of existing large-scale diffusion-based generative model. Our LucidDreamer has two alternate steps: Dreaming and Alignment. First, to generate multi-view consistent images from inputs, we set the point cloud as a geometrical guideline for each image generation. Specifically, we project a portion of point cloud to the desired view and provide the projection as a guidance for inpainting using the generative model. The inpainted images are lifted to 3D space with estimated depth maps, composing a new points. Second, to aggregate the new points into the 3D scene, we propose an aligning algorithm which harmoniously integrates the portions of newly generated 3D scenes. The finally obtained 3D scene serves as initial points for optimizing Gaussian splats. LucidDreamer produces Gaussian splats that are highly-detailed compared to the previous 3D scene generation methods, with no constraint on domain of the target scene.
</details>


[📄 Paper](https://arxiv.org/pdf/2311.13384) |  [🌐 Project Page](https://luciddreamer-cvlab.github.io/) | [💻 Code](https://github.com/luciddreamer-cvlab/LucidDreamer)

![LucidDreamer](images/3DGS/LucidDreamer.jpg)

### 9. [IJCAI '24] FastScene: Text-Driven Fast 3D Indoor Scene Generation via Panoramic Gaussian Splatting
**Authors:** Yikun Ma, Dandan Zhan, Zhi Jin
<details span>
<summary><b>Abstract</b></summary>
Text-driven 3D indoor scene generation holds broad applications, ranging from gaming and smart homes to AR/VR applications. Fast and high-fidelity scene generation is paramount for ensuring user-friendly experiences. However, existing methods are characterized by lengthy generation processes or necessitate the intricate manual specification of motion parameters, which introduces inconvenience for users. Furthermore, these methods often rely on narrow-field viewpoint iterative generations, compromising global consistency and overall scene quality. To address these issues, we propose FastScene, a framework for fast and higher-quality 3D scene generation, while maintaining the scene consistency. Specifically, given a text prompt, we generate a panorama and estimate its depth, since the panorama encompasses information about the entire scene and exhibits explicit geometric constraints. To obtain high-quality novel views, we introduce the Coarse View Synthesis (CVS) and Progressive Novel View Inpainting (PNVI) strategies, ensuring both scene consistency and view quality. Subsequently, we utilize Multi-View Projection (MVP) to form perspective views, and apply 3D Gaussian Splatting (3DGS) for scene reconstruction. Comprehensive experiments demonstrate FastScene surpasses other methods in both generation speed and quality with better scene consistency. Notably, guided only by a text prompt, FastScene can generate a 3D scene within a mere 15 minutes, which is at least one hour faster than state-of-the-art methods, making it a paradigm for user-friendly scene generation.
</details>

[📄 Paper](https://arxiv.org/pdf/2405.05768) | [💻 Code](https://github.com/Mr-Ma-yikun/FastScene)

![FastScene](images/3DGS/FastScene.jpg)

### 10. [CVPR '24 HighLight] GPS-Gaussian: Generalizable Pixel-wise 3D Gaussian Splatting for Real-time Human Novel View Synthesis
**Authors:** Shunyuan Zheng, Boyao Zhou, Ruizhi Shao, Boning Liu, Shengping Zhang, Liqiang Nie, Yebin Liu
<details span>
<summary><b>Abstract</b></summary>
We present a new approach, termed GPS-Gaussian, for synthesizing novel views of a character in a real-time manner. The proposed method enables 2K-resolution rendering under a sparse-view camera setting. Unlike the original Gaussian Splatting or neural implicit rendering methods that necessitate per-subject optimizations, we introduce Gaussian parameter maps defined on the source views and regress directly Gaussian Splatting properties for instant novel view synthesis without any fine-tuning or optimization. To this end, we train our Gaussian parameter regression module on a large amount of human scan data, jointly with a depth estimation module to lift 2D parameter maps to 3D space. The proposed framework is fully differentiable and experiments on several datasets demonstrate that our method outperforms state-of-the-art methods while achieving an exceeding rendering speed.
</details>


[📄 Paper](https://arxiv.org/pdf/2312.02155) | [🌐 Project Page](https://shunyuanzheng.github.io/GPS-Gaussian) | [💻 Code](https://shunyuanzheng.github.io/GPS-Gaussian) | [🎥 Video](https://www.youtube.com/watch?v=HjnBAqjGIAo)

![GPS-Gaussian](images/3DGS/GPS-Gaussian.jpg)


### 11. [ECCV '24] HAC: Hash-grid Assisted Context for 3D Gaussian Splatting Compression
**Authors:** Yihang Chen, Qianyi Wu, Weiyao Lin, Mehrtash Harandi, Jianfei Cai
<details span>
<summary><b>Abstract</b></summary>
3D Gaussian Splatting (3DGS) has emerged as a promising framework for novel view synthesis, boasting rapid rendering speed with high fidelity. However, the substantial Gaussians and their associated attributes necessitate effective compression techniques. Nevertheless, the sparse and unorganized nature of the point cloud of Gaussians (or anchors in our paper) presents challenges for compression. To address this, we make use of the relations between the unorganized anchors and the structured hash grid, leveraging their mutual information for context modeling, and propose a Hash-grid Assisted Context (HAC) framework for highly compact 3DGS representation. Our approach introduces a binary hash grid to establish continuous spatial consistencies, allowing us to unveil the inherent spatial relations of anchors through a carefully designed context model. To facilitate entropy coding, we utilize Gaussian distributions to accurately estimate the probability of each quantized attribute, where an adaptive quantization module is proposed to enable high-precision quantization of these attributes for improved fidelity restoration. Additionally, we incorporate an adaptive masking strategy to eliminate invalid Gaussians and anchors. Importantly, our work is the pioneer to explore context-based compression for 3DGS representation, resulting in a remarkable size reduction of over 75× compared to vanilla 3DGS, while simultaneously improving fidelity, and achieving over 11× size reduction over SOTA 3DGS compression approach Scaffold-GS. 
</details>

[📄 Paper](https://arxiv.org/pdf/2403.14530) | [🌐 Project Page](https://yihangchen-ee.github.io/project_hac/) | [💻 Code](https://github.com/YihangChen-ee/HAC)

![HAC](images/3DGS/HAC.jpg)


### 12. [ECCV '24]Compact3D: Smaller and Faster Gaussian Splatting with Vector Quantization
**Authors:** K L Navaneet, Kossar Pourahmadi Meibodi ,Soroush Abbasi Koohpayegani, Hamed Pirsiavash

<details span>
<summary><b>Abstract</b></summary>
3D Gaussian Splatting (3DGS) is a new method for modeling
and rendering 3D radiance fields that achieves much faster learning and rendering time compared to SOTA NeRF methods. However, it comes with the drawback of a much larger storage demand compared to NeRF methods since it needs to store the parameters for millions of 3D Gaussians. We notice that large groups of Gaussians share similar parameters
and introduce a simple vector quantization method based on K-means algorithm to quantize the Gaussian parameters. Then, we store the small codebook along with the index of the code for each Gaussian. We compress the indices further by sorting them and using a method similar to run-length encoding. Moreover, we use a simple regularizer that encourages zero opacity (invisible Gaussians) to reduce the number of Gaussians, thereby compressing the model and speeding up the rendering. We do extensive experiments on standard benchmarks as well as an existing 3D dataset that is an order of magnitude larger than the standard benchmarks used in this field. We show that our simple yet effective method can reduce the storage costs for 3DGS by 40× to 50× and rendering time by 2× to 3× with a very small drop in the quality of rendered images.
</details>

[📄 Paper](https://arxiv.org/pdf/2311.18159) | [🌐 Project Page](https://ucdvision.github.io/compact3d/) | [💻 Code](https://github.com/UCDvision/compact3d)

![Compact3D](images/3DGS/Compact3D.jpg)


### 13. Zero-shot Point Cloud Completion Via 2D Priors
**Authors:** Tianxin Huang, Zhiwen Yan, Yuyang Zhao, Gim Hee Lee
<details span>
<summary><b>Abstract</b></summary>
3D point cloud completion is designed to recover complete shapes from partially observed point clouds. Conventional completion methods typically depend on extensive point cloud data for training %, with their effectiveness often constrained to object categories similar to those seen during training. In contrast, we propose a zero-shot framework aimed at completing partially observed point clouds across any unseen categories. Leveraging point rendering via Gaussian Splatting, we develop techniques of Point Cloud Colorization and Zero-shot Fractal Completion that utilize 2D priors from pre-trained diffusion models to infer missing regions. Experimental results on both synthetic and real-world scanned point clouds demonstrate that our approach outperforms existing methods in completing a variety of objects without any requirement for specific training data.
</details>


[📄 Paper](https://arxiv.org/pdf/2404.06814)

![Zero-shot Point Cloud Completion Via 2D Priors](images/3DGS/Zero-shot_Point_Cloud_Completion_Via_2D_Priors.jpg)


### 14. RealmDreamer: Text-Driven 3D Scene Generation with Inpainting and Depth Diffusion
**Authors:** Jaidev Shriram, Alex Trevithick, Lingjie Liu, Ravi Ramamoorthi
<details span>
<summary><b>Abstract</b></summary>
We introduce RealmDreamer, a technique for generation of general forward-facing 3D scenes from text descriptions. Our technique optimizes a 3D Gaussian Splatting representation to match complex text prompts. We initialize these splats by utilizing the state-of-the-art text-to-image generators, lifting their samples into 3D, and computing the occlusion volume. We then optimize this representation across multiple views as a 3D inpainting task with image-conditional diffusion models. To learn correct geometric structure, we incorporate a depth diffusion model by conditioning on the samples from the inpainting model, giving rich geometric structure. Finally, we finetune the model using sharpened samples from image generators. Notably, our technique does not require video or multi-view data and can synthesize a variety of high-quality 3D scenes in different styles, consisting of multiple objects. Its generality additionally allows 3D synthesis from a single image.
</details>
[📄 Paper](https://arxiv.org/pdf/2404.07199) | [🌐 Project Page](https://realmdreamer.github.io/)

![RealmDreamer](images/3DGS/RealmDreamer.jpg)

### 15. 4Real: Towards Photorealistic 4D Scene Generation via Video Diffusion Models
**Authors:** Heng Yu, Chaoyang Wang, Peiye Zhuang, Willi Menapace, Aliaksandr Siarohin, Junli Cao, Laszlo A Jeni, Sergey Tulyakov, Hsin-Ying Lee
<details span>
<summary><b>Abstract</b></summary>
Existing dynamic scene generation methods mostly rely on distilling knowledge
from pre-trained 3D generative models, which are typically fine-tuned on synthetic
object datasets. As a result, the generated scenes are often object-centric and
lack photorealism. To address these limitations, we introduce a novel pipeline
designed for photorealistic text-to-4D scene generation, discarding the dependency
on multi-view generative models and instead fully utilizing video generative
models trained on diverse real-world datasets. Our method begins by generating
a reference video using the video generation model. We then learn the canonical
3D representation of the video using a freeze-time video, delicately generated
from the reference video. To handle inconsistencies in the freeze-time video,
we jointly learn a per-frame deformation to model these imperfections. We then
learn the temporal deformation based on the canonical representation to capture
dynamic interactions in the reference video. The pipeline facilitates the generation
of dynamic scenes with enhanced photorealism and structural integrity, viewable
from multiple perspectives, thereby setting a new standard in 4D scene generation.
</details>


[📄 Paper](https://arxiv.org/pdf/2406.07472) | [🌐 Project Page](https://snap-research.github.io/4Real/)

![4Real](images/3DGS/4Real.jpg)

### 16. [ICLR'2024 Oral] DreamGaussian: Generative Gaussian Splatting for Efficient 3D Content Creation
**Authors:** Jiaxiang Tang, Jiawei Ren, Hang Zhou, Ziwei Liu, Gang Zeng

<details span>
<summary><b>Abstract</b></summary>
Recent advances in 3D content creation mostly leverage optimization-based 3D generation via score distillation sampling (SDS). Though promising results have been exhibited, these methods often suffer from slow per-sample optimization, limiting their practical usage. In this paper, we propose DreamGaussian, a novel 3D content generation framework that achieves both efficiency and quality simultaneously. Our key insight is to design a generative 3D Gaussian Splatting model with companioned mesh extraction and texture refinement in UV space. In contrast to the occupancy pruning used in Neural Radiance Fields, we demonstrate that the progressive densification of 3D Gaussians converges significantly faster for 3D generative tasks. To further enhance the texture quality and facilitate downstream applications, we introduce an efficient algorithm to convert 3D Gaussians into textured meshes and apply a fine-tuning stage to refine the details. Extensive experiments demonstrate the superior efficiency and competitive generation quality of our proposed approach. Notably, DreamGaussian produces high-quality textured meshes in just 2 minutes from a single-view image, achieving approximately 10 times acceleration compared to existing methods.
</details>
[📄 Paper](https://arxiv.org/pdf/2309.16653.pdf) | [🌐 Project Page](https://dreamgaussian.github.io/) | [💻 Code](https://github.com/dreamgaussian/dreamgaussian) | [🎥 Video](https://www.youtube.com/live/l956ye13F8M?si=ZkvFL_lsY5OQUB7e)

![DreamGaussian](images/3DGS/DreamGaussian.jpg)


### 17. [ICLR '24] Real-time Photorealistic Dynamic Scene Representation and Rendering with 4D Gaussian Splatting
**Authors:** Zeyu Yang, Hongye Yang, Zijie Pan, Xiatian Zhu, Li Zhang

<details span>
<summary><b>Abstract</b></summary>
Reconstructing dynamic 3D scenes from 2D images and generating diverse views over time is challenging due to scene complexity and temporal dynamics. Despite advancements in neural implicit models, limitations persist: (i) Inadequate Scene Structure: Existing methods struggle to reveal the spatial and temporal structure of dynamic scenes from directly learning the complex 6D plenoptic function. (ii) Scaling Deformation Modeling: Explicitly modeling scene element deformation becomes impractical for complex dynamics. To address these issues, we consider the spacetime as an entirety and propose to approximate the underlying spatio-temporal 4D volume of a dynamic scene by optimizing a collection of 4D primitives, with explicit geometry and appearance modeling. Learning to optimize the 4D primitives enables us to synthesize novel views at any desired time with our tailored rendering routine. Our model is conceptually simple, consisting of a 4D Gaussian parameterized by anisotropic ellipses that can rotate arbitrarily in space and time, as well as view-dependent and time-evolved appearance represented by the coefficient of 4D spherindrical harmonics. This approach offers simplicity, flexibility for variable-length video and end-to-end training, and efficient real-time rendering, making it suitable for capturing complex dynamic scene motions. Experiments across various benchmarks, including monocular and multi-view scenarios, demonstrate our 4DGS model's superior visual quality and efficiency.
</details>

[📄 Paper](https://arxiv.org/pdf/2310.10642) | [🌐 Project Page](https://fudan-zvg.github.io/4d-gaussian-splatting/) | [💻 Code](https://github.com/fudan-zvg/4d-gaussian-splatting)

![4DGS](images/3DGS/4DGS.jpg)

### 18. [ECCV'24] DynMF: Neural Motion Factorization for Real-time Dynamic View Synthesis with 3D Gaussian Splatting
**Authors:** Agelos Kratimenos, Jiahui Lei, Kostas Daniilidis
<details span>
<summary><b>Abstract</b></summary>
Accurately and efficiently modeling dynamic scenes and motions is considered so challenging a task due to temporal dynamics and motion complexity. To address these challenges, we propose DynMF, a compact and efficient representation that decomposes a dynamic scene into a few neural trajectories. We argue that the per-point motions of a dynamic scene can be decomposed into a small set of explicit or learned trajectories. Our carefully designed neural framework consisting of a tiny set of learned basis queried only in time allows for rendering speed similar to 3D Gaussian Splatting, surpassing 120 FPS, while at the same time, requiring only double the storage compared to static scenes. Our neural representation adequately constrains the inherently underconstrained motion field of a dynamic scene leading to effective and fast optimization. This is done by biding each point to motion coefficients that enforce the per-point sharing of basis trajectories. By carefully applying a sparsity loss to the motion coefficients, we are able to disentangle the motions that comprise the scene, independently control them, and generate novel motion combinations that have never been seen before. We can reach state-of-the-art render quality within just 5 minutes of training and in less than half an hour, we can synthesize novel views of dynamic scenes with superior photorealistic quality. Our representation is interpretable, efficient, and expressive enough to offer real-time view synthesis of complex dynamic scene motions, in monocular and multi-view scenarios.
</details>

[📄 Paper](https://arxiv.org/pdf/2312.00112.pdf) | [🌐 Project Page](https://agelosk.github.io/dynmf/) | [💻 Code (not yet)](https://github.com/agelosk/dynmf)

![DynMF](images/3DGS/DynMF.jpg)

### 19. [CVPR '24] Control4D: Efficient 4D Portrait Editing with Text
**Authors:** Ruizhi Shao, Jingxiang Sun, Cheng Peng, Zerong Zheng, Boyao Zhou, Hongwen Zhang, Yebin Liu
<details span>
<summary><b>Abstract</b></summary>
We introduce Control4D, an innovative framework for
editing dynamic 4D portraits using text instructions. Our
method addresses the prevalent challenges in 4D editing,
notably the inefficiencies of existing 4D representations and
the inconsistent editing effect caused by diffusion-based editors. We first propose GaussianPlanes, a novel 4D representation that makes Gaussian Splatting more structured by
applying plane-based decomposition in 3D space and time.
This enhances both efficiency and robustness in 4D editing. Furthermore, we propose to leverage a 4D generator to
learn a more continuous generation space from inconsistent
edited images produced by the diffusion-based editor, which
effectively improves the consistency and quality of 4D editing. Comprehensive evaluation demonstrates the superiority of Control4D, including significantly reduced training
time, high-quality rendering, and spatial-temporal consistency in 4D portrait editing. 
</details>


[📄 Paper](https://arxiv.org/pdf/2305.20082) | [🌐 Project Page](https://control4darxiv.github.io/)

![Control4D](images/3DGS/Control4D.jpg)

### 20. [CVPR '24] Neural Parametric Gaussians for Monocular Non-Rigid Object Reconstruction
**Authors:** Devikalyan Das, Christopher Wewer, Raza Yunus, Eddy Ilg, Jan Eric Lenssen
<details span>
<summary><b>Abstract</b></summary>
Reconstructing dynamic objects from monocular videos
is a severely underconstrained and challenging problem,
and recent work has approached it in various directions.
However, owing to the ill-posed nature of this problem,
there has been no solution that can provide consistent, highquality novel views from camera positions that are significantly different from the training views. In this work, we
introduce Neural Parametric Gaussians (NPGs) to take on
this challenge by imposing a two-stage approach: first, we
fit a low-rank neural deformation model, which then is used
as regularization for non-rigid reconstruction in the second
stage. The first stage learns the object’s deformations such
that it preserves consistency in novel views. The second
stage obtains high reconstruction quality by optimizing 3D
Gaussians that are driven by the coarse model. To this end,
we introduce a local 3D Gaussian representation, where
temporally shared Gaussians are anchored in and deformed
by local oriented volumes. The resulting combined model
can be rendered as radiance fields, resulting in high-quality
photo-realistic reconstructions of the non-rigidly deforming
objects. We demonstrate that NPGs achieve superior results
compared to previous works, especially in challenging scenarios with few multi-view cues.
</details>


[📄 Paper](https://arxiv.org/pdf/2312.01196) | [🌐 Project Page](https://geometric-rl.mpi-inf.mpg.de/npg/) | [💻 Code (not yet)](https://github.com/DevikalyanDas/npgs)


![NPGs](images/3DGS/NPGs.jpg)


### 21. LayerPano3D: Layered 3D Panorama for Hyper-Immersive Scene Generation
**Authos:** Shuai Yang, Jing Tan, Mengchen Zhang, Tong Wu, Yixuan Li, Gordon Wetzstein, Ziwei Liu, Dahua Lin
<details span>
<summary><b>Abstract</b></summary>
3D immersive scene generation is a challenging yet critical task in computer vision and graphics. A desired virtual 3D scene should (1) exhibit omnidirectional view consistency, and (2) allow for free exploration in complex scene hierarchies. Existing methods either rely on successive scene expansion via inpainting or employ panorama representation to represent large FOV scene environments. However, the generated scene suffers from semantic drift during expansion and is unable to handle occlusion among scene hierarchies. To tackle these challenges, we introduce LayerPano3D, a novel framework for full-view, explorable panoramic 3D scene generation from a single text prompt. Our key insight is to decompose a reference 2D panorama into multiple layers at different depth levels, where each layer reveals the unseen space from the reference views via diffusion prior. LayerPano3D comprises multiple dedicated designs: (1) we introduce a novel text-guided anchor view synthesis pipeline for high-quality, consistent panorama generation. (2) We pioneer the Layered 3D Panorama as underlying representation to manage complex scene hierarchies and lift it into 3D Gaussians to splat detailed 360-degree omnidirectional scenes with unconstrained viewing paths. Extensive experiments demonstrate that our framework generates state-of-the-art 3D panoramic scene in both full view consistency and immersive exploratory experience. We believe that LayerPano3D holds promise for advancing 3D panoramic scene creation with numerous applications.
</details>
[📄 Paper](https://arxiv.org/pdf/2408.13252) | [🌐 Project Page](https://ys-imtech.github.io/projects/LayerPano3D/) | [💻 Code (not yet)](https://github.com/3DTopia/LayerPano3D) |  [🎥 Video](https://www.youtube.com/watch?v=dXvoFRbHOiw) 

![LayerPano3D](images/3DGS/Layerpano3d.jpg)

### 22. [CVPR '24] Spacetime Gaussian Feature Splatting for Real-Time Dynamic View Synthesis 
**Authors**: Zhan Li, Zhang Chen, Zhong Li, Yi Xu 

<details span>
<summary><b>Abstract</b></summary>
Novel view synthesis of dynamic scenes has been an intriguing yet challenging problem. Despite recent advancements, simultaneously achieving high-resolution photorealistic results, real-time rendering, and compact storage remains a formidable task. To address these challenges, we propose Spacetime Gaussian Feature Splatting as a novel dynamic scene representation, composed of three pivotal components. First, we formulate expressive Spacetime Gaussians by enhancing 3D Gaussians with temporal opacity and parametric motion/rotation. This enables Spacetime Gaussians to capture static, dynamic, as well as transient content within a scene. Second, we introduce splatted feature rendering, which replaces spherical harmonics with neural features. These features facilitate the modeling of view- and time-dependent appearance while maintaining small size. Third, we leverage the guidance of training error and coarse depth to sample new Gaussians in areas that are challenging to converge with existing pipelines. Experiments on several established real-world datasets demonstrate that our method achieves state-of-the-art rendering quality and speed, while retaining compact storage. At 8K resolution, our lite-version model can render at 60 FPS on an Nvidia RTX 4090 GPU. 
</details>

[📄 Paper](https://arxiv.org/pdf/2312.16812) | [🌐 Project Page](https://oppo-us-research.github.io/SpacetimeGaussians-website/) | [💻 Code](https://github.com/oppo-us-research/SpacetimeGaussians) | [🎥 Video](https://www.youtube.com/watch?v=YsPPmf-E6Lg)

![Spacetime_GS](images/3DGS/Spacetime_GS.jpg)

### 23. [CVPR '24 Highlight] 3DGStream: On-the-Fly Training of 3D Gaussians for Efficient Streaming of Photo-Realistic Free-Viewpoint Videos
**Authors:** Jiakai Sun, Han Jiao, Guangyuan Li, Zhanjie Zhang, Lei Zhao, Wei Xing

<details span>
<summary><b>Abstract</summary>
Constructing photo-realistic Free-Viewpoint Videos
(FVVs) of dynamic scenes from multi-view videos remains
a challenging endeavor. Despite the remarkable advancements achieved by current neural rendering techniques,
these methods generally require complete video sequences
for offline training and are not capable of real-time rendering. To address these constraints, we introduce 3DGStream,
a method designed for efficient FVV streaming of real-world
dynamic scenes. Our method achieves fast on-the-fly perframe reconstruction within 12 seconds and real-time rendering at 200 FPS. Specifically, we utilize 3D Gaussians
(3DGs) to represent the scene. Instead of the na¨ıve approach of directly optimizing 3DGs per-frame, we employ
a compact Neural Transformation Cache (NTC) to model
the translations and rotations of 3DGs, markedly reducing
the training time and storage required for each FVV frame.
Furthermore, we propose an adaptive 3DG addition strategy to handle emerging objects in dynamic scenes. Experiments demonstrate that 3DGStream achieves competitive
performance in terms of rendering speed, image quality,
training time, and model storage when compared with stateof-the-art methods.
</details>
[📄 Paper](https://openaccess.thecvf.com/content/CVPR2024/papers/Sun_3DGStream_On-the-Fly_Training_of_3D_Gaussians_for_Efficient_Streaming_of_CVPR_2024_paper.pdf) | [🌐 Project Page](http://sjojok.top/3dgstream/) | [💻 Code](https://github.com/SJoJoK/3DGStream)

![3DGStream](images/3DGS/3DGStream.jpg)

### 24. [SIGGRAPH'24 ]TIP-Editor: An Accurate 3D Editor Following Both Text-Prompts And Image-Prompts
**Authors:** Jingyu Zhuang, Di Kang, Yan-Pei Cao, Guanbin Li, Liang Lin, Ying Shan

<details span>
<summary><b>Abstract</b></summary>
Text-driven 3D scene editing has gained significant attention owing to its
convenience and user-friendliness. However, existing methods still lack accurate control of the specified appearance and location of the editing result due
to the inherent limitations of the text description. To this end, we propose a
3D scene editing framework, TIP-Editor, that accepts both text and image
prompts and a 3D bounding box to specify the editing region. With the
image prompt, users can conveniently specify the detailed appearance/style
of the target content in complement to the text description, enabling accurate control of the appearance. Specifically, TIP-Editor employs a stepwise
2D personalization strategy to better learn the representation of the existing scene and the reference image, in which a localization loss is proposed
to encourage correct object placement as specified by the bounding box.
Additionally, TIP-Editor utilizes explicit and flexible 3D Gaussian splatting
(GS) as the 3D representation to facilitate local editing while keeping the
background unchanged. Extensive experiments have demonstrated that TIPEditor conducts accurate editing following the text and image prompts in
the specified bounding box region, consistently outperforming the baselines in editing quality, and the alignment to the prompts, qualitatively and
quantitatively.
</details>
[📄 Paper](https://arxiv.org/pdf/2401.14828) | [🌐 Project Page](https://zjy526223908.github.io/TIP-Editor/)

![TIP-Editor](images/3DGS/TIP-Editor.jpg)

### 25. Gaga: Group Any Gaussians via 3D-aware Memory Bank
**Authors**: Weijie Lyu, Xueting Li, Abhijit Kundu, Yi-Hsuan Tsai, Ming-Hsuan Yang

<details span>
<summary><b>Abstract</b></summary>
We introduce Gaga, a framework that reconstructs and segments open-world 3D scenes by leveraging inconsistent 2D masks predicted by zero-shot segmentation models. Contrasted to prior 3D scene segmentation approaches that heavily rely on video object tracking, Gaga utilizes spatial information and effectively associates object masks across diverse camera poses. By eliminating the assumption of continuous view changes in training images, Gaga demonstrates robustness to variations in camera poses, particularly beneficial for sparsely sampled images, ensuring precise mask label consistency. Furthermore, Gaga accommodates 2D segmentation masks from diverse sources and demonstrates robust performance with different open-world zero-shot segmentation models, significantly enhancing its versatility. Extensive qualitative and quantitative evaluations demonstrate that Gaga performs favorably against state-of-the-art methods, emphasizing its potential for real-world applications such as scene understanding and manipulation.
</details>

[📄 Paper](https://arxiv.org/pdf/2404.07977) | [🌐 Project Page](https://www.gaga.gallery/) | [💻 Code](https://github.com/weijielyu/Gaga) | [🎥 Video](https://www.youtube.com/watch?v=rqs5BuVFOok)

![Gaga](images/3DGS/Gaga.jpg)
### 26. [CVPR' 24]HiFi4G: High-Fidelity Human Performance Rendering via Compact Gaussian Splatting
**Authors**: Yuheng Jiang, Zhehao Shen, Penghao Wang, Zhuo Su, Yu Hong, Yingliang Zhang, Jingyi Yu, Lan Xu

<details span>
<summary><b>Abstract</b></summary>
We have recently seen tremendous progress in photo-real human modeling and rendering. Yet, efficiently rendering realistic human performance and integrating it into the rasterization pipeline remains challenging. In this paper, we present HiFi4G, an explicit and compact Gaussian-based approach for high-fidelity human performance rendering from dense footage. Our core intuition is to marry the 3D Gaussian representation with non-rigid tracking, achieving a compact and compression-friendly representation. We first propose a dual-graph mechanism to obtain motion priors, with a coarse deformation graph for effective initialization and a fine-grained Gaussian graph to enforce subsequent constraints. Then, we utilize a 4D Gaussian optimization scheme with adaptive spatial-temporal regularizers to effectively balance the non-rigid prior and Gaussian updating. We also present a companion compression scheme with residual compensation for immersive experiences on various platforms. It achieves a substantial compression rate of approximately 25 times, with less than 2MB of storage per frame. Extensive experiments demonstrate the effectiveness of our approach, which significantly outperforms existing approaches in terms of optimization speed, rendering quality, and storage overhead.
</details>

[📄 Paper](https://arxiv.org/pdf/2312.03461) | [🌐 Project Page](https://nowheretrix.github.io/HiFi4G/)

![HiFi4G](images/3DGS/HiFi4G.jpg)

<!-- NeRF part -->
## NeRF

### 1. [TPAMI' 24] PERF: Panoramic Neural Radiance Field from a Single Panorama
**Authors:** Guangcong Wang, Peng Wang, Zhaoxi Chen, Wenping Wang, Chen Change Loy, Ziwei Liu
<details span>
<summary><b>Abstract</b></summary>
Neural Radiance Field (NeRF) has achieved substantial progress in novel view synthesis given multi-view images.
Recently, some works have attempted to train a NeRF from a single image with 3D priors. They mainly focus on a limited field of view
with a few occlusions, which greatly limits their scalability to real-world 360-degree panoramic scenarios with large-size occlusions. In
this paper, we present PERF, a 360-degree novel view synthesis framework that trains a panoramic neural radiance field from a single
panorama. Notably, PERF allows 3D roaming in a complex scene without expensive and tedious image collection. To achieve this goal,
we propose a novel collaborative RGBD inpainting method and a progressive inpainting-and-erasing method to lift up a 360-degree 2D
scene to a 3D scene. Specifically, we first predict a panoramic depth map as initialization given a single panorama and reconstruct
visible 3D regions with volume rendering. Then we introduce a collaborative RGBD inpainting approach into a NeRF for completing
RGB images and depth maps from random views, which is derived from an RGB Stable Diffusion model and a monocular depth
estimator. Finally, we introduce an inpainting-and-erasing strategy to avoid inconsistent geometry between a newly-sampled view and
reference views. The two components are integrated into the learning of NeRFs in a unified optimization framework and achieve
promising results. Extensive experiments on Replica and a new dataset PERF-in-the-wild demonstrate the superiority of our PERF over
state-of-the-art methods. Our PERF can be widely used for real-world applications, such as panorama-to-3D, text-to-3D, and 3D scene
stylization applications.
</details>

[📄 Paper](https://arxiv.org/pdf/2310.16831) |  [🌐 Project Page](https://github.com/perf-project/PeRF?tab=readme-ov-file) | [🎥 Video](https://www.youtube.com/watch?v=4wa2h1fjh2U)

![PERF](images/NeRF/PERF.jpg)

### 2. G-NeLF: Memory- and Data-Efficient Hybrid Neural Light Field for Novel View Synthesis
**Authors:** Lutao Jiang, Lin Wang
<details span>
<summary><b>Abstract</b></summary>
Following the burgeoning interest in implicit neural representation, Neural Light Field (NeLF) has been introduced
to predict the color of a ray directly. Unlike Neural Radiance Field (NeRF), NeLF does not create a point-wise
representation by predicting color and volume density for
each point in space. However, the current NeLF methods face a challenge as they need to train a NeRF model
first and then synthesize over 10K views to train NeLF for
improved performance. Additionally, the rendering quality of NeLF methods is lower compared to NeRF methods.
In this paper, we propose G-NeLF, a versatile grid-based
NeLF approach that utilizes spatial-aware features to unleash the potential of the neural network’s inference capability, and consequently overcome the difficulties of NeLF
training. Specifically, we employ a spatial-aware feature
sequence derived from a meticulously crafted grid as the
ray’s representation. Drawing from our empirical studies
on the adaptability of multi-resolution hash tables, we introduce a novel grid-based ray representation for NeLF that
can represent the entire space with a very limited number of
parameters. To better utilize the sequence feature, we design a lightweight ray color decoder that simulates the ray
propagation process, enabling a more efficient inference of the ray’s color. G-NeLF can be trained without necessitating significant storage overhead and with the model size
of only 0.95 MB to surpass previous state-of-the-art NeLF.
Moreover, compared with grid-based NeRF methods, e.g.,
Instant-NGP, we only utilize one-tenth of its parameters to
achieve higher performance. Our code will be released
upon acceptance.
</details>

[📄 Paper](https://arxiv.org/pdf/2409.05617)

![G-NeLF](images/NeRF/G-NeLF.jpg)

### 3. [CVPR'2024 HighLight] GP-NeRF: Generalized Perception NeRF for Context-Aware 3D Scene Understanding
**Authors:** Hao Li, Dingwen Zhang, Yalun Dai, Nian Liu, Lechao Cheng, Jingfeng Li, Jingdong Wang, Junwei Han
<details span>
<summary><b>Abstract</b></summary>
Applying NeRF to downstream perception tasks for scene understanding and representation is becoming increasingly popular. Most existing methods treat semantic prediction as an additional rendering task, \textit{i.e.}, the "label rendering" task, to build semantic NeRFs. However, by rendering semantic/instance labels per pixel without considering the contextual information of the rendered image, these methods usually suffer from unclear boundary segmentation and abnormal segmentation of pixels within an object. To solve this problem, we propose Generalized Perception NeRF (GP-NeRF), a novel pipeline that makes the widely used segmentation model and NeRF work compatibly under a unified framework, for facilitating context-aware 3D scene perception. To accomplish this goal, we introduce transformers to aggregate radiance as well as semantic embedding fields jointly for novel views and facilitate the joint volumetric rendering of both fields. In addition, we propose two self-distillation mechanisms, i.e., the Semantic Distill Loss and the Depth-Guided Semantic Distill Loss, to enhance the discrimination and quality of the semantic field and the maintenance of geometric consistency. In evaluation, we conduct experimental comparisons under two perception tasks (\textit{i.e.} semantic and instance segmentation) using both synthetic and real-world datasets. Notably, our method outperforms SOTA approaches by 6.94%, 11.76%, and 8.47% on generalized semantic segmentation, finetuning semantic segmentation, and instance segmentation, respectively.
</details>

[📄 Paper](https://arxiv.org/pdf/2311.11863)

![GP-NeRF](images/NeRF/GP-NeRF.jpg)

### 4. DreaMo: Articulated 3D Reconstruction From A Single Casual Video
**Authors:** Tao Tu, Ming-Feng Li, Chieh Hubert Lin, Yen-Chi Cheng, Min Sun, Ming-Hsuan Yang
<details span>
<summary><b>Abstract</b></summary>
Articulated 3D reconstruction has valuable applications in various domains, yet it remains costly and demands intensive work from domain experts. Recent advancements in template-free learning methods show promising results with monocular videos. Nevertheless, these approaches necessitate a comprehensive coverage of all viewpoints of the subject in the input video, thus limiting their applicability to casually captured videos from online sources. In this work, we study articulated 3D shape reconstruction from a single and casually captured internet video, where the subject's view coverage is incomplete. We propose DreaMo that jointly performs shape reconstruction while solving the challenging low-coverage regions with view-conditioned diffusion prior and several tailored regularizations. In addition, we introduce a skeleton generation strategy to create human-interpretable skeletons from the learned neural bones and skinning weights. We conduct our study on a self-collected internet video collection characterized by incomplete view coverage. DreaMo shows promising quality in novel-view rendering, detailed articulated shape reconstruction, and skeleton generation. Extensive qualitative and quantitative studies validate the efficacy of each proposed component, and show existing methods are unable to solve correct geometry due to the incomplete view coverage.
</details>

[📄 Paper](https://arxiv.org/pdf/2312.02617) |  [🌐 Project Page](https://ttaoretw.github.io/DreaMo/)

![DreaMo](images/NeRF/DreaMo.jpg)

### 5. C-NERF: Representing Scene Changes as Directional Consistency Difference-based NeRF
**Authors:** Rui Huang, Binbin Jiang, Qingyi Zhao, William Wang,Yuxiang Zhang, Qing Guo
<details span>
<summary><b>Abstract</b></summary>
In this work, we aim to detect the changes caused by object variations in a scene represented by the neural radiance fields (NeRFs). Given an arbitrary view and two sets of scene images captured at different timestamps, we can predict the scene changes in that view, which has significant potential applications in scene monitoring and measuring. We conducted preliminary studies and found that such an exciting task cannot be easily achieved by utilizing existing NeRFs and 2D change detection methods with many false or missing detections. The main reason is that the 2D change detection is based on the pixel appearance difference between spatial-aligned image pairs and neglects the stereo information in the NeRF. To address the limitations, we propose the C-NERF to represent scene changes as directional consistency difference-based NeRF, which mainly contains three modules. We first perform the spatial alignment of two NeRFs captured before and after changes. Then, we identify the change points based on the direction-consistent constraint; that is, real change points have similar change representations across view directions, but fake change points do not. Finally, we design the change map rendering process based on the built NeRFs and can generate the change map of an arbitrarily specified view direction. To validate the effectiveness, we build a new dataset containing ten scenes covering diverse scenarios with different changing objects. Our approach surpasses state-of-the-art 2D change detection and NeRF-based methods by a significant margin.
</details>

[📄 Paper](https://arxiv.org/pdf/2312.02751) |  [💻 Code](https://github.com/C-NeRF/C-NeRF) 

![C-NeRF](images/NeRF/C-NeRF.jpg)

### 6. TriHuman : A Real-time and Controllable Tri-plane Representation for Detailed Human Geometry and Appearance Synthesis
**Authors:** Heming Zhu, Fangneng Zhan, Christian Theobalt, Marc Habermann
<details span>
<summary><b>Abstract</b></summary>
Creating controllable, photorealistic, and geometrically detailed digital doubles of real humans solely from video data is a key challenge in Computer Graphics and Vision, especially when real-time performance is required. Recent methods attach a neural radiance field (NeRF) to an articulated structure, e.g., a body model or a skeleton, to map points into a pose canonical space while conditioning the NeRF on the skeletal pose. These approaches typically parameterize the neural field with a multi-layer perceptron (MLP) leading to a slow runtime. To address this drawback, we propose TriHuman a novel human-tailored, deformable, and efficient tri-plane representation, which achieves real-time performance, state-of-the-art pose-controllable geometry synthesis as well as photorealistic rendering quality. At the core, we non-rigidly warp global ray samples into our undeformed tri-plane texture space, which effectively addresses the problem of global points being mapped to the same tri-plane locations. We then show how such a tri-plane feature representation can be conditioned on the skeletal motion to account for dynamic appearance and geometry changes. Our results demonstrate a clear step towards higher quality in terms of geometry and appearance modeling of humans as well as runtime performance.
</details>

[📄 Paper](https://arxiv.org/pdf/2312.05161) |  [🌐 Project Page](https://vcai.mpi-inf.mpg.de/projects/trihuman/) 

![TriHuman](images/NeRF/TriHuman.jpg)

### 7. [CVPR' 24 Highlight] SIFU: Side-view Conditioned Implicit Function for Real-world Usable Clothed Human Reconstruction
**Authors:** Zechuan Zhang, Zongxin Yang, Yi Yang
<details span>
<summary><b>Abstract</b></summary>
Creating high-quality 3D models of clothed humans from single images for real-world applications is crucial. Despite recent advancements, accurately reconstructing humans in complex poses or with loose clothing from in-the-wild images, along with predicting textures for unseen areas, remains a significant challenge. A key limitation of previous methods is their insufficient prior guidance in transitioning from 2D to 3D and in texture prediction. In response, we introduce SIFU (Side-view Conditioned Implicit Function for Real-world Usable Clothed Human Reconstruction), a novel approach combining a Side-view Decoupling Transformer with a 3D Consistent Texture Refinement pipeline.SIFU employs a cross-attention mechanism within the transformer, using SMPL-X normals as queries to effectively decouple side-view features in the process of mapping 2D features to 3D. This method not only improves the precision of the 3D models but also their robustness, especially when SMPL-X estimates are not perfect. Our texture refinement process leverages text-to-image diffusion-based prior to generate realistic and consistent textures for invisible views. Through extensive experiments, SIFU surpasses SOTA methods in both geometry and texture reconstruction, showcasing enhanced robustness in complex scenarios and achieving an unprecedented Chamfer and P2S measurement. Our approach extends to practical applications such as 3D printing and scene building, demonstrating its broad utility in real-world scenarios. 
</details>

[📄 Paper](https://arxiv.org/pdf/2312.06704) |  [🌐 Project Page](https://river-zhang.github.io/SIFU-projectpage/) |  [💻 Code](https://github.com/River-Zhang/SIFU) 

![SIFU](images/NeRF/SIFU.jpg)

### 8. [AAAI'2024] ColNeRF: Collaboration for Generalizable Sparse Input Neural Radiance Field
**Authors:** Zhangkai Ni, Peiqi Yang, Wenhan Yang, Hanli Wang, Lin Ma, Sam Kwong
<details span>
<summary><b>Abstract</b></summary>
Neural Radiance Fields (NeRF) have demonstrated impressive potential in synthesizing novel views from dense input, however, their effectiveness is challenged when dealing with sparse input. Existing approaches that incorporate additional depth or semantic supervision can alleviate this issue to an extent. However, the process of supervision collection is not only costly but also potentially inaccurate, leading to poor performance and generalization ability in diverse scenarios. In our work, we introduce a novel model: the Collaborative Neural Radiance Fields (ColNeRF) designed to work with sparse input. The collaboration in ColNeRF includes both the cooperation between sparse input images and the cooperation between the output of the neural radiation field. Through this, we construct a novel collaborative module that aligns information from various views and meanwhile imposes self-supervised constraints to ensure multi-view consistency in both geometry and appearance. A Collaborative Cross-View Volume Integration module (CCVI) is proposed to capture complex occlusions and implicitly infer the spatial location of objects. Moreover, we introduce self-supervision of target rays projected in multiple directions to ensure geometric and color consistency in adjacent regions. Benefiting from the collaboration at the input and output ends, ColNeRF is capable of capturing richer and more generalized scene representation, thereby facilitating higher-quality results of the novel view synthesis. Extensive experiments demonstrate that ColNeRF outperforms state-of-the-art sparse input generalizable NeRF methods. Furthermore, our approach exhibits superiority in fine-tuning towards adapting to new scenes, achieving competitive performance compared to per-scene optimized NeRF-based methods while significantly reducing computational costs. 
</details>

[📄 Paper](https://arxiv.org/pdf/2312.09095) | [💻 Code](https://github.com/eezkni/ColNeRF) 

![ColNeRF](images/NeRF/ColNeRF.jpg)
