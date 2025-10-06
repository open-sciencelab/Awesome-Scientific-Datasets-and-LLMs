# Awesome-Scientific-Datasets-and-LLMs

A curated collection of papers, datasets, and resources on Scientific Datasets and Large Language Models (LLMs), organized in reference to our survey: [**"A Survey of Scientific Large Language Models: From Data Foundations to Agent Frontiers"**](https://arxiv.org/abs/2508.21148)


> If you spot any mistakes or have suggestions, feel free to reach out by email: huming@pjlab.org.cn
>
> (We also recommend CC’ing clma24@m.fudan.edu.cn and litianbin@pjlab.org.cn in case of any unsuccessful delivery issue.)
>
> If you find our survey useful for your research, please cite the following paper:

## 📖 Citation
If you find this repository or our survey helpful in your research, please kindly cite our paper:
```bibtex
@article{hu2025survey,
  title={A Survey of Scientific Large Language Models: From Data Foundations to Agent Frontiers},
  author={Hu, Ming and Ma, Chenglong and Li, Wei and Xu, Wanghan and Wu, Jiamin and Hu, Jucheng and Li, Tianbin and Zhuang, Guohang and Liu, Jiaqi and Lu, Yingzhou and others},
  journal={arXiv preprint arXiv:2508.21148},
  year={2025}
}
```
In addition, [**"Awesome-Agent-Scientists"**](https://github.com/AgenticScience/Awesome-Agent-Scientists) highlights the latest advances of AI agents in scientific research, which nicely complements our work.
```bibtex
@article{wei2025ai,
  title={From AI for Science to Agentic Science: A Survey on Autonomous Scientific Discovery},
  author={Wei, Jiaqi and Yang, Yuejin and Zhang, Xiang and Chen, Yuhan and Zhuang, Xiang and Gao, Zhangyang and Zhou, Dongzhan and Wang, Guangshuai and Gao, Zhiqiang and Cao, Juntai and others},
  journal={arXiv preprint arXiv:2508.14111},
  year={2025}
}
```

## 📈 Trends in Scientific LLM Publications
![arxiv_llms](assets/trend.png)
Cumulative trend of publications on major preprint platforms whose titles or abstracts mention the keyword “language model” or the combination “language model + scientific domain” (e.g., chemistry, physics, multi-omics, medicine, etc.). Left: Results from January 2018 to August 2025, from arXiv and PubMed. For arXiv, the matching includes “language model” in combination with additional science-related keywords; PubMed results are limited to occurrences in titles and abstracts. Both platforms show rapid growth. Right: Results from 2020 to August 2025, from bioRxiv, medRxiv, and ChemRxiv, all based on direct matches of “language model” in titles and abstracts. While the overall volumes are smaller than arXiv and PubMed, all three platforms, especially bioRxiv, show rapid acceleration, reflecting growing interdisciplinary interest in large language models across biomedical, chemical, and computational sciences

## 🔬 Development of Sci-LLMs
![sci-llm_develop](assets/sci-llms_develop.png)
Evolution of Sci-LLMs reveals four paradigm shifts from 2018 to 2025, including (1) the progression from transfer learning approaches, (2) through the scaling era marked by knowledge integration in larger models, (3) instruction-following capabilities enabling flexible task adaptation, to (4) the latest paradigm introduces scientific agents—AI systems capable of autonomously conducting scientific research, from hypothesis generation and experimental design to data analysis and discovery. Note: Model positions reflect their release dates (x-axis) rather than strict paradigm classification. The four paradigms represent evolving trends in Sci-LLM development with overlaps and continuities, not mutually exclusive categories.

## 🕑 Timeline of Sci-LLMs
![sci-llms](assets/sci-llms.png)
Chronological overview of notable Sci-LLMs categorized by six scientific domains, spanning from 2019 through early 2025. Due to the rapid expansion of the field, this figure presents a selective overview.


## 📑 Table of Contents

- [Awesome-Scientific-Datasets-and-LLMs](#awesome-scientific-datasets-and-llms)
  - [📖 Citation](#-citation)
  - [📈 Trends in Scientific LLM Publications](#-trends-in-scientific-llm-publications)
  - [🔬 Development of Sci-LLMs](#-development-of-sci-llms)
  - [🕑 Timeline of Sci-LLMs](#-timeline-of-sci-llms)
  - [📑 Table of Contents](#-table-of-contents)
  - [🧪 Scientific Pretraining, SFT, Reasoning, and Agent Datasets](#-scientific-pretraining-sft-reasoning-and-agent-datasets)
    - [🧬 Life Sciences](#-life-sciences)
    - [⚗️ Chemistry](#️-chemistry)
    - [⚛️ Physics](#️-physics)
    - [🌌 Astronomy](#-astronomy)
    - [🪨 Materials Science](#-materials-science)
    - [🌍 Earth Science](#-earth-science)
    - [🔭 General Science](#-general-science)
  - [📝 Scientific Evaluation Datasets](#-scientific-evaluation-datasets)
    - [🧬 Life Science](#-life-science)
    - [⚗️ Chemistry](#️-chemistry-1)
    - [⚛️ Physics](#️-physics-1)
    - [🌌 Astronomy](#-astronomy-1)
    - [🪨 Materials Science](#-materials-science-1)
    - [🌍 Earth Science](#-earth-science-1)
    - [🔭 General Science](#-general-science-1)
  - [🤖 Scientific Models](#-scientific-models)
    - [🌐 General-purpose](#-general-purpose)
    - [⚛️ Physics](#️-physics-2)
    - [⚗️ Chemistry](#️-chemistry-2)
    - [🪨 Materials Science](#-materials-science-2)
    - [🧬 Life Sciences](#-life-sciences-1)
    - [🌌 Astronomy](#-astronomy-2)
    - [🌍 Earth Science](#-earth-science-2)
  - [📅 Star History](#-star-history)

## 🧪 Scientific Pretraining, SFT, Reasoning, and Agent Datasets

<details>
<summary>
  
### 🧬 Life Sciences

</summary>

 <a href="#-table-of-contents" style="float:right;">⬆ Back to Top</a>
  Dataset | Domain | Modality | Purpose | Type | Release | Language | Source | Annotation  Pipeline | Human   Annotators | Human Tasks | Auto-annotation  Tools | Size |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| [MIRAGE ](https://arxiv.org/abs/2506.20100) | Agriculture | Biological entity photos | SFT | VQA (multi-image) | 2025.06 | EN | Scientific databases | Semi-automated | N/A | Data generation | GPT-4.1 | 37,512 |
  | [CROP ](https://dl.acm.org/doi/10.5555/3737916.3739585) | Agriculture | Academic papers | SFT | Text QA | 2024.09 | EN, ZH | Academic and research resources | Semi-automated | N/A | Data generation | GPT-4 | 211,909 |
  | [ToT‑Biology ](https://huggingface.co/datasets/moremilk/ToT-Biology) | General Biology | Biomedical QA | SFT, CoT | Text QA with CoT | 2025.01 | EN | Academic and research resources | N/A | N/A | N/A | N/A | 23,000 |
  | [BioASQ10b-factoid ](https://huggingface.co/datasets/legacy107/bioasq10b-factoid) | General Biology | Clinical dialogue | SFT | Text QA | 2023.07 | EN | Academic and research resources | Manual | N/A | Data generation and review | N/A | 1.25K |
  | [ReasonMed ](https://huggingface.co/datasets/lingshu-medical-mllm/ReasonMed) | Healthcare and Medical Sciences | Clinical dialogue | SFT, CoT | Text QA with CoT | 2025.06 | EN | Comprehensive multi-source integration | Automated | N/A | N/A | Qwen-2.5-72B, DeepSeek-R1-Distill-Llama-70B, HuatuoGPT-o1-70B | 194,925 |
  | [Open-PMC-18M ](https://huggingface.co/datasets/vector-institute/open-pmc-18m) | Healthcare and Medical Sciences | CT, CFP | Pre-training | Image-text | 2025.06 | EN | Academic and research resources | Automated | N/A | N/A | N/A | 25,000,000 |
  | [ReXVQA ](https://huggingface.co/datasets/rajpurkarlab/ReXVQA) | Healthcare and Medical Sciences | X-ray | SFT | VQA | 2025.06 | EN | Integration of existing datasets | Semi-automated | 3 | Data review | GPT-4o, ClinicalBERT, MedEmbed | 613,277 |
  | [RexGradient-160K ](https://huggingface.co/datasets/rajpurkarlab/ReXGradient-160K) | Healthcare and Medical Sciences | X-ray | Pre-training, SFT | Image-text | 2025.05 | EN | Scientific databases | Manual | N/A | N/A | N/A | 160K |
  | [AlphaMed19K ](https://huggingface.co/datasets/che111/AlphaMed19K) | Healthcare and Medical Sciences | Biomedical QA | SFT, CoT | Text QA | 2025.05 | EN | Integration of existing datasets | Automated | N/A | Data generation and review | N/A | 19,178 |
  | [Derm1M ](https://github.com/SiyuanYan1/Derm1M) | Healthcare and Medical Sciences | Dermatological images | Pre-training | Image-text | 2025.3 | EN | Social media and forums, Academic and research resources | Automated | N/A | N/A | DenseNet, DINO, GPT-4o, Whisper | 1,029,761 |
  | [MedVideoCap-55K ](https://huggingface.co/datasets/FreedomIntelligence/MedVideoCap-55K) | Healthcare and Medical Sciences | Medical videos | Pre-training, SFT | Video-text | 2025.04 | EN | Web and Internet content | Automated | N/A | Data review | GPT-4o | 55,803 |
  | [medical-o1-reasoning-SFT ](https://huggingface.co/datasets/FreedomIntelligence/medical-o1-reasoning-SFT) | Healthcare and Medical Sciences | Clinical dialogue | SFT, CoT | Text QA with CoT | 2025.04 | EN, ZH | Comprehensive multi-source integration | Automated | N/A | N/A | DeepSeek-R1 | 90,200 |
  | [GMAI-Reasoning10K ](https://huggingface.co/datasets/General-Medical-AI/GMAI-Reasoning10K) | Healthcare and Medical Sciences | CT, Dermatology, Endoscopy, CFP, Histopathology, MRI, Microscopy, OCT, PET, US, X-ray, \etc | SFT | VQA | 2025.04 | EN | Comprehensive multi-source integration | Semi-automated | N/A | Data review | GPT-4o | 17,004 |
  | [MedReason ](https://huggingface.co/datasets/UCSC-VLAA/MedReason) | Healthcare and Medical Sciences | Clinical dialogue | SFT, CoT | Text QA with CoT | 2025.03 | EN | Comprehensive multi-source integration | Automated | N/A | N/A | N/A | 32,682 |
  | [GEMeX-VQA ](https://huggingface.co/datasets/BoKelvin/GEMeX-VQA) | Healthcare and Medical Sciences | X-ray | Pre-training, SFT | VQA | 2025.03 | EN | Integration of existing datasets | Semi-automated | N/A | Data review | OpenBioLLM-70B, GPT-4o | 1,601,615 |
  | [MIMIC-Diff-VQA ](https://physionet.org/content/medical-diff-vqa/) | Healthcare and Medical Sciences | X-ray | SFT | VQA (multi-image) | 2025.02 | EN | Scientific databases | Semi-automated | 3 | Data generation and review | ScispaCy | 630,633 |
  | [ICG-CXR ](https://progemu.github.io) | Healthcare and Medical Sciences | X-ray | SFT | VQA (multi-image) | 2025.03 | EN | Scientific databases | Automated | N/A | Data generation and review | GPT-4 | 11,439 |
  | [VL-Health ](https://huggingface.co/datasets/lintw/VL-Health) | Healthcare and Medical Sciences | CT, CFP, MRI, Microscopy, OCT, US, X-ray | Pre-training, SFT | Image-text, VQA | 2025.02 | EN, ZH | Comprehensive multi-source integration | Semi-automated | N/A | Data review | GPT-4o | 1,548,847 |
  | [BIOMEDICA ](https://huggingface.co/datasets/BIOMEDICA/biomedica_webdataset_24M) | Healthcare and Medical Sciences | Academic papers | Pre-training | Raw text | 2025.01 | EN | Academic and research resources | Semi-automated | 7 | Data review | N/A | 2,400,000 |
  | [AfriMed-QA v2 ](https://huggingface.co/datasets/intronhealth/afrimedqa_v2) | Healthcare and Medical Sciences | Clinical dialogue | SFT | Text QA | 2024.11 | EN | Comprehensive multi-source integration | Semi-automated | N/A | N/A | N/A | 15,275 |
  | [GMAI-VL-5.5M ](https://github.com/uni-medical/GMAI-VL) | Healthcare and Medical Sciences | CT, Dermatology, Endoscopy, CFP, Histopathology, MRI, Microscopy, OCT, PET, US, X-ray, \etc | SFT | VQA, Text QA | 2024.11 | EN, ZH | Comprehensive multi-source integration | Semi-automated | 5 | Data review | GPT-4o | 5.5M |
  | [OphVL ](https://github.com/minghu0830/OphCLIP) | Healthcare and Medical Sciences | Ophthalmic Surgical Video | Pre-training | Video-text | 2024.11 | EN | Web and Internet content | Automated | N/A | Data generation and review | SurgicBERTa, GPT-4o | 375,198 |
  | [Bora-v1 ](https://huggingface.co/datasets/Sweson/Bora_v1) | Healthcare and Medical Sciences | Endoscopy, MRI, Microscopy, US | SFT | Video-text | 2024.10 | EN | Integration of existing datasets | Automated | N/A | Data review | N/A | 4,897 |
  | [MedSyn ](https://huggingface.co/datasets/Glebkaa/MedSyn-synthetic) | Healthcare and Medical Sciences | Clinical documentation | Pre-training | Raw text | 2024.08 | RU | Academic and research resources | Automated | N/A | N/A | GPT-4, Medical Knowledge Graph | 41,200 |
  | [RealMedQA ](https://huggingface.co/datasets/k2141255/RealMedQA) | Healthcare and Medical Sciences | Biomedical QA | SFT | Text QA | 2024.08 | EN | Encyclopedias and knowledge bases | Semi-automated | 6 | Data generation and review | GPT-3.5-turbo | 1,200 |
  | [MedTrinity-25M ](https://huggingface.co/datasets/UCSC-VLAA/MedTrinity-25M) | Healthcare and Medical Sciences | CT, MRI, X-ray, Histopathology, \etc | Pre-training | Image-text, VQA | 2024.08 | EN | Integration of existing datasets, Scientific databases | Automated | N/A | N/A | N/A | 25,000,000 |
  | [MedPix-single ](https://medpix.nlm.nih.gov/) | Healthcare and Medical Sciences | CT, MRI, US, X-ray | Pre-training | Image-text | 2024.07 | EN | Scientific databases | Manual | N/A | Data generation | N/A | 59,000 |
  | [BIMCV-R ](https://huggingface.co/datasets/cyd0806/BIMCV-R) | Healthcare and Medical Sciences | CT | Pre-training | Image-text | 2024.07 | EN | Scientific databases | Semi-automated | 20+ | Data review | GPT-4 | 8,069 |
  | [MIMIC-Ext-MIMIC-CXR-VQA ](https://physionet.org/content/mimic-ext-mimic-cxr-vqa/1.0.0/) | Healthcare and Medical Sciences | X-ray | Pre-training, SFT | VQA | 2024.07 | EN | Integration of existing datasets | Semi-automated | 4 | Data review | GPT-4 | 377,391 |
  | [EHRXQA ](https://physionet.org/content/ehrxqa/1.0.0/) | Healthcare and Medical Sciences | X-ray | Pre-training, SFT | VQA | 2024.07 | EN | Integration of existing datasets | Semi-automated | 4 | Data review | GPT-4 | 46,152 |
  | [CheXpertPlus ](https://stanfordaimi.azurewebsites.net/datasets/5158c524-d3ab-4e02-96e9-6ee9efc110a1) | Healthcare and Medical Sciences | X-ray | Pre-training | Image-text | 2024.06 | EN | Scientific databases | Semi-automated | 10 | Data generation and review | CheXbert, Radgraph | 223,228 |
  | [PubMedVision ](https://huggingface.co/datasets/FreedomIntelligence/PubMedVision) | Healthcare and Medical Sciences | CT, Endoscopy, CFP, Infrared Reflectance, MRI, Microscopy, OCT, US, X-ray | SFT | VQA | 2024.06 | EN | Academic and research resources | Automated | N/A | N/A | GPT-4, GPT-4V, SentenceBERT | 1,294,092 |
  | [MediQ ](https://huggingface.co/datasets/stellalisy/mediQ) | Healthcare and Medical Sciences | EHR | SFT | Text QA | 2024.06 | EN | Academic and research resources | Automated | N/A | N/A | GPT-3.5, LLaMA‑3 | 2,545 |
  | [HuatuoGPT2-SFT-GPT4-140K ](https://huggingface.co/datasets/FreedomIntelligence/HuatuoGPT2-SFT-GPT4-140K) | Healthcare and Medical Sciences | Clinical dialogue | SFT | Text QA | 2024.06 | ZH | Other sources | Automated | N/A | Data generation and review | GPT-4 | 140,000 |
  | [Asclepius-Synthetic-Clinical-Notes ](https://huggingface.co/datasets/starmpcc/Asclepius-Synthetic-Clinical-Notes) | Healthcare and Medical Sciences | EHR | SFT | Text QA | 2024.06 | EN | Academic and research resources | Semi-automated | N/A | Data generation | GPT-3.5 | 158,114 |
  | [Know Medical Dialogues ](https://huggingface.co/datasets/knowrohit07/know_medical_dialoguesn) | Healthcare and Medical Sciences | Clinical dialogue | SFT | Text QA | 2024.06 | EN | Web and Internet content | Automated | N/A | N/A | N/A | 480 |
  | [Duvel ](https://huggingface.co/datasets/cnachteg/duvel) | Healthcare and Medical Sciences | Academic papers | SFT | Classification | 2024.05 | EN | Scientific databases | Semi-automated | N/A | Data generation | ALAMBIC | 6,553 |
  | [SkinCAP ](https://huggingface.co/datasets/joshuachou/SkinCAP) | Healthcare and Medical Sciences | Dermatology | Pre-training | Image-text | 2024.05 | EN | Academic and research resources | Semi-automated | N/A | N/A | N/A | 4,000 |
  | [MM-Retinal ](https://github.com/lxirich/MM-Retinal) | Healthcare and Medical Sciences | CFP, FFA, OCT | Pre-training, SFT | Image-text | 2024.05 | EN, ZH | Academic and research resources | Semi-automated | 6 | Data review | N/A | 4,349 |
  | [M3D-Data (caption) ](https://huggingface.co/datasets/GoodBaiBai88/M3D-Cap) | Healthcare and Medical Sciences | CT, Clinical reports | Pre-training, SFT | Image-text, Text QA, VQA | 2024.04 | EN | Scientific databases, Integration of existing datasets | Semi-automated | N/A | Data generation and review | GPT-4V | 120,092 |
  | [M3D-Data (instruction) ](https://huggingface.co/datasets/GoodBaiBai88/M3D-Cap) | Healthcare and Medical Sciences | CT, Clinical reports | SFT | Image-text, Text QA, VQA | 2024.04 | EN | Scientific databases, Integration of existing datasets | Semi-automated | N/A | Data generation and review | GPT-4V | 58,180 |
  | [RadGenome-Chest CT ](https://huggingface.co/datasets/RadGenome/RadGenome-ChestCT) | Healthcare and Medical Sciences | CT | Pre-training, SFT | VQA, Image-text | 2024.04 | EN | Academic and research resources | Semi-automated | N/A | Data review | SAT, GPT-4, GPT-2 | 1,965,000 |
  | [CXR-LLM ](https://huggingface.co/datasets/cheese111/cxr_llm) | Healthcare and Medical Sciences | X-ray | SFT | VQA | 2024.03 | EN | Integration of existing datasets | Semi-automated | N/A | Data generation | GPT-4 | 104,892 |
  | [MedChatZH ](https://huggingface.co/datasets/tyang816/MedChatZH) | Healthcare and Medical Sciences | Clinical dialogue | Pre-training, SFT | Text QA | 2024.03 | ZH | Comprehensive multi-source integration | Semi-automated | N/A | Data generation | N/A | 2,068,823 |
  | [Mental health chatbot dataset ](https://huggingface.co/datasets/heliosbrahma/mental_health_chatbot_dataset) | Healthcare and Medical Sciences | Clinical dialogue | SFT | Text QA | 2024.02 | EN | Web and Internet content | Automated | N/A | N/A | N/A | 172 |
  | [StatPearls ](https://huggingface.co/datasets/MedRAG/statpearls) | Healthcare and Medical Sciences | Academic papers | Pre-training | Raw text | 2024.02 | EN | Scientific databases | Automated | N/A | N/A | N/A | 301,202 |
  | [Quilt-Instruct ](https://huggingface.co/datasets/wisdomik/QUILT-LLaVA-Instruct-107K) | Healthcare and Medical Sciences | Histopathology | SFT | VQA | 2024.02 | EN | Web and Internet content | Semi-automated | N/A | Data review | GPT-4-turbo | 107,131 |
  | [SHADR ](https://huggingface.co/datasets/m720/SHADR) | Healthcare and Medical Sciences | EHR | SFT | Classification | 2024.01 | EN | Scientific databases | Semi-automated | N/A | Data review | GPT-3.5 | 446 |
  | [RJUA-QA ](http://data.openkg.cn/dataset/rjua-qadatasets) | Healthcare and Medical Sciences | Dianosis report, Clinical dialogue | SFT | Text QA | 2023.12 | ZH | Other sources | Manual | N/A | Data generation and review | N/A | 1,705 |
  | [RP3D-DiagDS ](https://huggingface.co/datasets/QiaoyuZheng/RP3D-DiagDS) | Healthcare and Medical Sciences | CT, MRI, X-ray US, Fluoroscopy, \etc | Pre-training | Classification | 2023.12 | EN | Scientific databases | Semi-automated | N/A | Data generation and review | Custom crawlers, GPT-4 | 40,936 |
  | [PMC-Inline ](https://huggingface.co/datasets/chaoyi-wu/PMC-Inline/tree/main) | Healthcare and Medical Sciences | CT, MRI, PET, US, X-ray | Pre-training | Image-text | 2023.11 | EN | Academic and research resources | Automated | N/A | N/A | N/A | 11,000,000 |
  | [ROCOv2 ](https://huggingface.co/datasets/eltorio/ROCOv2-radiology) | Healthcare and Medical Sciences | CT, MRI, PET, US, X-ray | Pre-training, SFT | Image-text | 2023.11 | EN | Academic and research resources | Semi-automated | N/A | N/A | fastText, MedCAT | 80,080 |
  | [PMC-CaseReport ](https://huggingface.co/datasets/chaoyi-wu/PMC-CaseReport) | Healthcare and Medical Sciences | X-ray | SFT | Image-text, VQA | 2023.11 | EN | Academic and research resources | Automated | N/A | N/A | N/A | 1,100,000 |
  | [MedMD ](https://github.com/chaoyi-wu/RadFM) | Healthcare and Medical Sciences | CT, MRI, PET, US, X-ray | Pre-training, SFT | Image-text, VQA | 2023.11 | EN | Academic and research resources | Semi-automated | 8 | Data review | ChatGPT | 16,000,000 |
  | [Taiyi-Instruction-Data-001 ](https://github.com/DUTIR-BioNLP/Taiyi-LLM/blob/main/data_file/dataset_inf.md) | Healthcare and Medical Sciences | Dianosis report, Clinical dialogue, EMR, Academic papers, \etc | Pre-training, SFT | Text QA | 2023.11 | EN, ZH | Integration of existing datasets | Automated | N/A | Data review | N/A | 1,114,315 |
  | [MTS-DIALOG ](https://huggingface.co/datasets/beanham/medsum) | Healthcare and Medical Sciences | Clinical dialogue | Pre-training | Text QA | 2023.11 | EN | Academic and research resources | Semi-automated | 12 | Data generation and review | GPT-4o | 23,977 |
  | [MTS-Dialog ](https://huggingface.co/datasets/beanham/medsum) | Healthcare and Medical Sciences | Clinical dialogue | Pre-training | Raw text | 2023.11 | EN | Patent databases | Semi-automated | 9 | Data generation and review | OPUS-MT, BART | 1,701 |
  | [Clinical Guidelines ](https://huggingface.co/datasets/epfl-llm/guidelines) | Healthcare and Medical Sciences | Clinical guidelines | Pre-training | Text QA with CoT | 2023.11 | EN | Scientific databases | Semi-automated | N/A | Data review | S2ORC, GROBID | 38,000 |
  | [INSPECT ](https://som-shahlab.github.io/inspect-website/) | Healthcare and Medical Sciences | CT | Pre-training | Image-text | 2023.11 | EN | Scientific databases | Semi-automated | N/A | Data review, Data generation | Clinical Longformer | 23,248 |
  | [AeroPath ](https://huggingface.co/datasets/andreped/AeroPath) | Healthcare and Medical Sciences | CT | Agent | Segmentation | 2023.11 | EN | Scientific databases | Semi-automated | 2 | Data review | 3D Slicer | 27 (CT scans) |
  | [MORFITT ](https://huggingface.co/datasets/qanastek/MORFITT) | Healthcare and Medical Sciences | Clinical papers | Pre-training | Classification | 2023.11 | FR | Academic and research resources | Manual | N/A | Data review | N/A | 3,556 |
  | [NoteChat ](https://huggingface.co/datasets/akemiH/NoteChat) | Healthcare and Medical Sciences | Clinical dialogue | SFT | Text QA | 2023.10 | EN | Integration of existing datasets | Automated | N/A | N/A | N/A | 207,000 |
  | [ChiMed-VL ](https://huggingface.co/datasets/williamliu/ChiMed-VL) | Healthcare and Medical Sciences | X-ray, CT, MRI, \etc | Pre-training, SFT | Image-text, Text QA | 2023.10 | ZH, EN | Integration of existing datasets | Automated | N/A | N/A | GPT-3.5 | 1,049,455 |
  | [OncQA ](https://huggingface.co/datasets/shanchen/OncQA) | Healthcare and Medical Sciences | Dianosis report | SFT | Text QA | 2023.10 | EN | Other sources | Manual | 6 | Data generation and review | GPT-4 | 156 |
  | [SDOH-NLI ](https://huggingface.co/datasets/davanstrien/SDOH-NLI) | Healthcare and Medical Sciences | Clinical notes | Pre-training | Classification | 2023.10 | EN | Integration of existing datasets | Manual | N/A | Data generation | N/A | 21.1K |
  | [CMtMedQA ](https://github.com/SupritYoung/Zhongjing) | Healthcare and Medical Sciences | Clinical dialogue | SFT | Text QA | 2023.08 | ZH | Other sources | Automated | N/A | Data review | N/A | 68,000 |
  | [DISC-Med-SFT ](https://huggingface.co/datasets/Flmc/DISC-Med-SFT) | Healthcare and Medical Sciences | Clinical dialogue | SFT | Text QA | 2023.08 | ZH | Integration of existing datasets | Semi-automated | N/A | Data review | GPT-3.5, GPT-4 | 470,000 |
  | [Healix-V1 ](https://huggingface.co/datasets/health360/Healix-V1) | Healthcare and Medical Sciences | Clinical dialogue | SFT | Text QA | 2023.07 | EN | Comprehensive multi-source integration | N/A | N/A | N/A | N/A | 796,239 |
  | [Medical Cord19 ](https://huggingface.co/datasets/mystic-leung/medical_cord19) | Healthcare and Medical Sciences | Academic papers | Pre-training | Raw text | 2023.07 | EN | Academic and research resources | Automated | N/A | N/A | N/A | 250,000 |
  | [Pile-PubMed Central ](https://opendatalab.com/OpenDataLab/Pile-PubMed_Central) | Healthcare and Medical Sciences | Academic papers | Pre-training | Raw text | 2023.07 | EN | Academic and research resources | Automated | N/A | Data generation | N/A | N/A |
  | [AGCT ](https://huggingface.co/datasets/FremyCompany/AGCT-Dataset) | Healthcare and Medical Sciences | Biomedical knowledge base | Pre-training | Raw text | 2023.07 | EN, FR | Scientific databases | Automated | N/A | N/A | Custom generation | 421,216 |
  | [Synthetic CSAW 100k Mammograms ](https://huggingface.co/datasets/SinKove/synthetic_mammography_csaw) | Healthcare and Medical Sciences | Mammography | SFT | Image-text | 2023.07 | EN | Scientific databases | Automated | N/A | N/A | Diffusion Model | 100K |
  | [Quilt-1M ](https://quilt1m.github.io/) | Healthcare and Medical Sciences | Histopathology | Pre-training, SFT | Image-text | 2023.06 | EN | Academic and research resources, Web and Internet content, Other sources | Automated | N/A | N/A | N/A | 1,000,000 |
  | [LLaVA-Med ](https://github.com/microsoft/LLaVA-Med) | Healthcare and Medical Sciences | CT, Histopathology, MRI, Microscopy, PET, US, X-ray | Pre-training, SFT | VQA, Image-text | 2023.06 | EN | Comprehensive multi-source integration | Automated | N/A | N/A | GPT-4 | 630,000 |
  | [ShenNong-TCM-Dataset ](https://github.com/michael-wzhu/ShenNong-TCM-LLM?tab=readme-ov-file) | Healthcare and Medical Sciences | Clinical dialogue | SFT, CoT | Text QA | 2023.06 | ZH | Comprehensive multi-source integration | Automated | N/A | Data generation | ChatGPT | 113,000 |
  | [PMC-VQA ](https://huggingface.co/datasets/RadGenome/PMC-VQA) | Healthcare and Medical Sciences | CT, CFP, Histopathology, MRI, Microscopy, US, X-ray | SFT | VQA | 2023.05 | EN | Academic and research resources | Automated | N/A | N/A | N/A | 226,946 |
  | [ChatMed-Consult-Dataset ](https://github.com/michael-wzhu/ChatMed) | Healthcare and Medical Sciences | Clinical dialogue | SFT | Text QA | 2023.05 | ZH | Web and Internet content | Automated | N/A | Data generation | GPT-3.5-Turbo | 549,000 |
  | [QiZhenGPT-20k ](https://github.com/CMKRG/QiZhenGPT/tree/main?tab=readme-ov-file) | Healthcare and Medical Sciences | Clinical dialogue | SFT | Text QA | 2023.05 | ZH | Other sources | Automated | N/A | Data generation | N/A | 20,000 |
  | [Huatuo-26M ](https://huggingface.co/datasets/FreedomIntelligence/huatuo_encyclopedia_qa) | Healthcare and Medical Sciences | Biomedical QA | Pre-training, SFT | Text QA | 2023.05 | EN | Encyclopedias and knowledge bases | Semi-automated | N/A | Data review | Bert, T5 | 26,000,000 |
  | [Huatuo26M-Lite ](https://huggingface.co/datasets/FreedomIntelligence/Huatuo26M-Lite) | Healthcare and Medical Sciences | Clinical dialogue, Dianosis report | Pre-training, SFT | Text QA | 2023.05 | ZH | Web and Internet content | Semi-automated | N/A | Data review | ChatGPT | 177,703 |
  | [Visual Med-Alpaca ](https://github.com/cambridgeltl/visual-med-alpaca) | Healthcare and Medical Sciences | CT, CFP, Histopathology, MRI, Microscopy, US, X-ray | SFT | VQA | 2023.04 | EN | Scientific databases | Automated | N/A | N/A | GPT-3.5 | 54,000 |
  | [MedAlpaca ](https://github.com/kbressem/medAlpaca#data-overview) | Healthcare and Medical Sciences | Clinical dialogue, Academic papers | Pre-training, SFT | Raw text, Text QA | 2023.04 | EN | Comprehensive multi-source integration | Automated | N/A | Data generation and review | N/A | 860,076 |
  | [Med-ChatGLM ](https://github.com/SCIR-HI/Med-ChatGLM/tree/main) | Healthcare and Medical Sciences | Biomedical knowledge base | SFT | Text QA | 2023.04 | ZH | Integration of existing datasets | Automated | N/A | Data generation | GPT-3.5 | 7,622 |
  | [PMC-OA ](https://huggingface.co/datasets/axiong/pmc_oa) | Healthcare and Medical Sciences | CT, Dermatology, Endoscopy, Histopathology, Microscopy, MRI, OCT, PET, X-ray | Pre-training | Image-text | 2023.03 | EN | Academic and research resources | Automated | N/A | Data generation and review | ResNet101 (DocFigure), ResNet34 (DETR MedICaT), PMC-CLIP | 1,646,592 |
  | [ChatDoctor ](https://github.com/Kent0n-Li/ChatDoctor) | Healthcare and Medical Sciences | Clinical dialogue | SFT | Text QA | 2023.03 | EN | Other sources | Semi-automated | N/A | Data generation and review | N/A | 115,000 |
  | [WikiMedQA ](https://huggingface.co/datasets/sileod/wikimedqa) | Healthcare and Medical Sciences | Clinical Reports | SFT | Text QA | 2023.03 | EN | Web and Internet content | Semi-automated | N/A | N/A | SentenceBERT, BioLinkBERT | 111,895 |
  | [MIMIC-IV ](https://physionet.org/content/mimiciv/3.1/) | Healthcare and Medical Sciences | EHR | Pre-training, SFT | Raw text | 2023.01 | EN | Scientific databases | Semi-automated | N/A | N/A | Transformer-DeID | 364,627 |
  | [BioRED ](https://ftp.ncbi.nlm.nih.gov/pub/lu/BioRED/) | Healthcare and Medical Sciences | Academic papers | Pre-training | Classification | 2022.09 | EN | Scientific databases | Semi-automated | 6 | Data generation and review | PubTator | 500 |
  | [ViHealthQA ](https://huggingface.co/datasets/tarudesu/ViHealthQA) | Healthcare and Medical Sciences | Biomedical QA | SFT | Text QA | 2022.06 | VI | Social media and forums | Manual | N/A | Data generation | N/A | 10,015 |
  | [MedMCQA ](https://github.com/MedMCQA/MedMCQA) | Healthcare and Medical Sciences | Medical exams | SFT | Text QA | 2022.03 | EN | Books and literary works | Automated | N/A | Data generation | N/A | 193,155 |
  | [PMC-Patients-ReCDS ](https://huggingface.co/datasets/zhengyun21/PMC-Patients-ReCDS) | Healthcare and Medical Sciences | Clinical dialogue | SFT | Text QA | 2022.02 | EN | Academic and research resources | Automated | N/A | N/A | N/A | 293,000 |
  | [PMC-Patients ](https://huggingface.co/datasets/zhengyun21/PMC-Patients) | Healthcare and Medical Sciences | Clinical report | Pre-training | Raw text | 2022.02 | EN | Scientific databases | Semi-automated | N/A | Data review | PubMedBERT, BioLinkBERT | 167,000 |
  | [CMCQA ](https://github.com/WENGSYX/CMCQA) | Healthcare and Medical Sciences | Clinical dialogue | SFT | Text QA | 2022.01 | ZH | Web and Internet content | Automated | N/A | Data review | N/A | 1,294,753 |
  | [IMCS-V2 ](https://github.com/lemuria-wchen/imcs21-cblue) | Healthcare and Medical Sciences | Clinical dialogue | SFT | Text QA | 2022.01 | ZH | Other sources | Manual | N/A | Data generation and review | N/A | 4,116 |
  | [MLEC-QA ](https://github.com/Judenpech/MLEC-QA) | Healthcare and Medical Sciences | Biomedical QA | SFT | Raw text | 2021.11 | ZH | Academic and research resources | Semi-automated | N/A | Data generation and review | N/A | 136,236 |
  | [ImageClef-VQA Med 2021 ](https://github.com/abachaa/VQA-Med-2021) | Healthcare and Medical Sciences | CT, MRI, US, X-ray | SFT | VQA | 2021.09 | EN | Academic and research resources | Automated | N/A | N/A | N/A | 4,500 |
  | [BioLeaflets ](https://huggingface.co/datasets/ruslan/bioleaflets-biomedical-ner) | Healthcare and Medical Sciences | Package leaflets | Pre-training | Raw text | 2021.09 | EN | Web and Internet content | Semi-automated | N/A | Data generation | Stanza, Amazon Comprehend Medical | 1,067 |
  | [MedGPT-5k-ko ](https://huggingface.co/datasets/mncai/MedGPT-5k-ko) | Healthcare and Medical Sciences | Clinical trials, EHR, Medical forum, Medical textbooks | SFT | Classification, Text QA | 2021.06 | ZH | Scientific databases, Books and literary works, Web and Internet content, Comprehensive multi-source integration | Manual | 3 | Data generation and review | N/A | 149,141 |
  | [CBLUE ](https://github.com/CBLUEbenchmark/CBLUE) | Healthcare and Medical Sciences | Clinical trials, EHR, Medical forum, Medical textbooks | SFT | Classification, Text QA | 2021.06 | ZH | Scientific databases, Books and literary works, Web and Internet content, Comprehensive multi-source integration | Manual | 3 | Data generation and review | N/A | 149,141 |
  | [MedDG ](https://github.com/lwgkzl/MedDG) | Healthcare and Medical Sciences | Clinical dialogue | SFT | Text QA | 2021.05 | ZH | Web and Internet content | Automated | N/A | Data generation and review | N/A | 100,000 |
  | [SLAKE ](https://huggingface.co/datasets/BoKelvin/SLAKE) | Healthcare and Medical Sciences | CT, MRI, X-ray | SFT | VQA | 2021.02 | EN, ZH | Academic and research resources | Automated | N/A | N/A | N/A | 11,958 |
  | [Chinese-medical-dialogue-data ](https://github.com/Toyhom/Chinese-medical-dialogue-data) | Healthcare and Medical Sciences | Clinical dialogue | SFT | Text QA | 2021.02 | ZH | Other sources | N/A | N/A | N/A | N/A | 792,099 |
  | [DeepEyeNet ](https://github.com/Jhhuangkay/DeepOpht-Medical-Report-Generation-for-Retinal-Images-via-Deep-Models-and-Visual-Explanation) | Healthcare and Medical Sciences | CFP, FFA | Pre-training | Image-text | 2021.01 | EN | Scientific databases | Manual | N/A | Data generation | N/A | 15,709 |
  | [AIforCOVID ](https://aiforcovid.radiomica.it/) | Healthcare and Medical Sciences | X-ray | Pre-training, SFT | Image-text | 2020.12 | EN | Scientific databases | Manual | N/A | Data generation | N/A | 820 |
  | [MedICaT ](https://github.com/allenai/medicat) | Healthcare and Medical Sciences | CT, Endoscopy, Histopathology, MRI, Microscopy, PET, US, X-ray | Pre-training, SFT | Image-text | 2020.10 | EN | Academic and research resources | Semi-automated | 7 | Data generation | ResNet101-DocFigure, ScispaCy | 217,060 |
  | [ImageClef-VQA Med 2020 ](https://github.com/abachaa/VQA-Med-2020) | Healthcare and Medical Sciences | CT, MRI, US, X-ray | SFT | VQA | 2020.09 | EN | Academic and research resources | Automated | N/A | N/A | N/A | 4,000 |
  | [MedQA ](https://github.com/jind11/MedQA) | Healthcare and Medical Sciences | Medical exams | SFT | Text QA | 2020.09 | EN, ZH | Scientific databases | Manual | N/A | Data generation and review | N/A | 61,097 |
  | [MedDialog-CN ](https://drive.google.com/drive/folders/1r09_i8nJ9c1nliXVGXwSqRYqklcHd9e2) | Healthcare and Medical Sciences | Clinical dialogue | SFT | Text QA | 2020.07 | ZH | Web and Internet content | Automated | N/A | Data review | N/A | 1,100,000 |
  | [MEDIQA-AnS ](https://github.com/saverymax/qdriven-chiqa-summarization) | Healthcare and Medical Sciences | Consumer health QA | SFT | Text QA | 2020.05 | EN, ZH | Web and Internet content | Semi-automated | 2 | Data generation | Custom crawlers | 156 |
  | [MedDialog ](https://github.com/sidney1994/Medical-Dialogue-System) | Healthcare and Medical Sciences | Clinical dialogue | SFT | Text QA | 2020.04 | EN, ZH | Web and Internet content | Automated | N/A | N/A | Custom crawlers | 14,668,058 |
  | [PathVQA ](https://huggingface.co/datasets/flaviagiammarino/path-vqa) | Healthcare and Medical Sciences | Histopathology | SFT | VQA | 2020.03 | EN | Academic and research resources | Automated | N/A | N/A | N/A | 19,654 |
  | [RetinaRocks ](https://www.retinarocks.org/) | Healthcare and Medical Sciences | CFP | Pre-training, SFT | Image-text | 2019.12 | EN | Other sources | Manual | N/A | Data generation | N/A | 4,000 |
  | [MedQuAD ](https://huggingface.co/datasets/lavita/MedQuAD) | Healthcare and Medical Sciences | Clinical dialogue | SFT | Text QA | 2019.10 | EN | Web and Internet content | Automated | N/A | N/A | Custom crawlers | 47,441 |
  | [ImageClef-VQA Med 2019 ](https://github.com/abachaa/VQA-Med-2019) | Healthcare and Medical Sciences | CT, MRI, US, X-ray | SFT | VQA | 2019.09 | EN | Academic and research resources | Automated | N/A | N/A | N/A | 15,292 |
  | [PubMedQA ](https://github.com/pubmedqa/pubmedqa) | Healthcare and Medical Sciences | Academic papers | SFT | Text QA | 2019.09 | EN | Web and Internet content | Semi-automated | N/A | Data generation and review | N/A | 212,300 |
  | [PubMedQA instruction ](https://huggingface.co/datasets/fedml/PubMedQA_instruction) | Healthcare and Medical Sciences | Academic papers | SFT | Text QA | 2019.09 | EN | Academic and research resources | Manual | N/A | Data generation | N/A | 1K |
  | [MIMIC-CXR ](https://physionet.org/content/mimic-cxr/2.1.0/) | Healthcare and Medical Sciences | X-ray | Pre-training | Image-text | 2019.08 | EN | Scientific databases | Manual | N/A | Data generation | N/A | 227,835 |
  | MIMIC-Extract | Healthcare and Medical Sciences | EHR | Pre-training | Text QA | 2019.07 | EN | Scientific databases | Automated | N/A | N/A | N/A | 2,000,000 |
  | [webMedQA ](https://github.com/hejunqing/webMedQA) | Healthcare and Medical Sciences | Clinical dialogue | SFT | Text QA | 2019.03 | ZH | Web and Internet content | Automated | N/A | Data review | N/A | 63,284 |
  | [VQA-RAD ](https://huggingface.co/datasets/flaviagiammarino/vqa-rad) | Healthcare and Medical Sciences | CT, MRI, PET, US, X-ray | SFT | VQA | 2018.11 | EN | Academic and research resources | Manual | N/A | Data generation | N/A | 1,793 |
  | [cMedQA2 ](https://github.com/zhangsheng93/cMedQA2) | Healthcare and Medical Sciences | Clinical dialogue | SFT | Text QA | 2018.11 | ZH | Web and Internet content | Automated | N/A | Data review | N/A | 108,000 |
  | [ROCO ](https://github.com/razorx89/roco-dataset) | Healthcare and Medical Sciences | CT, MRI, PET, US, X-ray | Pre-training, SFT | Image-text | 2018.09 | EN | Academic and research resources | Automated | N/A | N/A | N/A | 81,000 |
  | [emrQA ](https://github.com/panushri25/emrQA) | Healthcare and Medical Sciences | Clinical dialogue | SFT | Text QA | 2018.09 | EN | Integration of existing datasets | Semi-automated | N/A | N/A | N/A | 455,000 |
  | [ImageClef-VQA Med 2018 ](https://www.imageclef.org/2018) | Healthcare and Medical Sciences | CT, MRI, US, Unknown, X-ray | SFT | VQA | 2018.06 | EN | Academic and research resources | Automated | N/A | N/A | N/A | 6,413 |
  | [LiveQA ](https://github.com/abachaa/LiveQA_MedicalTask_TREC2017) | Healthcare and Medical Sciences | Consumer health QA | SFT | Text QA | 2018.02 | EN | Scientific databases | Automated | N/A | Data review | N/A | 634 |
  | [LiveQA trec2017 ](https://huggingface.co/datasets/katielink/liveqa_trec2017) | Healthcare and Medical Sciences | Clinical dialogue | SFT | Text QA | 2017.08 | EN | Academic and research resources | Semi-automated | N/A | Data review | N/A | 634 |
  | [OpenI ](https://openi.nlm.nih.gov/faq) | Healthcare and Medical Sciences | X-ray | Pre-training | Image-text | 2016.03 | EN | Scientific databases | Manual | N/A | Data generation | N/A | 3,955 |
  | [Retina Image Bank ](https://imagebank.asrs.org/) | Healthcare and Medical Sciences | CFP, FFA | Pre-training, SFT | Image-text | 2012.08 | EN | Other sources | Manual | N/A | Data generation | N/A | 30,452 |
  | [William Hoyt ImageText ](https://novel.utah.edu/collection/william-f-hoyt/#tab-collection) | Healthcare and Medical Sciences | CFP | Pre-training | Image-text | 2004.03 | EN | Scientific databases | Manual | N/A | Data generation | N/A | 856 |
  | [Pima ](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database) | Healthcare and Medical Sciences | EHR | SFT | Classification | 1988.11 | EN | Scientific databases | Manual | N/A | N/A | N/A | 691 |
  | [COVID-19-Data-Hub ](https://covid19datahub.io/articles/data.html) | Healthcare and Medical Sciences | Global pandemic data (cases, vaccines, policies, \etc) | Pre-training, RAG | Classification, Regression | 2020.07 | EN | Comprehensive multi-source integration | Automated | N/A | N/A | R package | N/A |
  | [BEACON ](https://github.com/terry-r123/RNABenchmark) | Molecular and Cellular Biology | RNA sequence | SFT | Raw text | 2024.06 | EN | Comprehensive multi-source integration | Semi-automated | N/A | Data generation and review | N/A | 870,883 |
  | [SPICE ](https://zenodo.org/records/10975225) | Molecular and Cellular Biology | SMILES | Pre-training, RAG | Classification, Regression | 2024.03 | EN | Scientific databases | Semi-automated | N/A | Data generation and review | N/A | 113,999 |
  | [PubChemSTM ](https://github.com/chao1224/MoleculeSTM) | Molecular and Cellular Biology | SMILES | Pre-training, SFT | Raw text | 2024.01 | EN | Academic and research resources | Semi-automated | N/A | Data generation | SciBERT, spaCy | 281,000 |
  | [SourceData ](https://huggingface.co/datasets/EMBO/SourceData) | Molecular and Cellular Biology | Academic papers | Pre-training | VQA | 2023.10 | EN | Academic and research resources | Semi-automated | N/A | Data review | PubMedBERT, BioLinkBERT, GPT-4o | 62,543 |
  | [Mol-Instructions ](https://huggingface.co/datasets/zjunlp/Mol-Instructions) | Molecular and Cellular Biology | Biomolecular instructions | SFT | Text QA | 2023.06 | EN | Comprehensive multi-source integration | Automated | N/A | Data review | GPT-3.5 | 2,043,000 |
  | [PCdes ](https://github.com/thunlp/KV-PLM) | Molecular and Cellular Biology | SMILES | Pre-training, SFT | Raw text | 2022.12 | EN | Academic and research resources | Automated | N/A | N/A | Custom crawlers | 12,000 |
  | [MoMu ](https://github.com/ddz16/MoMu) | Molecular and Cellular Biology | Graph | Pre-training, SFT | Raw text | 2022.12 | EN | Academic and research resources | Automated | N/A | N/A | OGB | 15,613 |
  | [PEER ](https://github.com/DeepGraphLearning/PEER_Benchmark) | Molecular and Cellular Biology | Protein sequence | SFT | Classification, Regression | 2022.10 | EN | Comprehensive multi-source integration | Semi-automated | N/A | Data generation and review | N/A | 329,922 |
  | [BioGPT ](https://github.com/microsoft/BioGPT) | Molecular and Cellular Biology, Healthcare and Medical Sciences | Biomedical domain pretraining corpus | Pre-training, SFT | Raw text | 2022.08 | EN | Scientific databases, Academic and research resources | Automated | N/A | N/A | Moses tokenizer, fastBPE | 15M |
  | [DISEASES ](https://diseases.jensenlab.org/Downloads) | Molecular and Cellular Biology, Healthcare and Medical Sciences, Multi-omics | Disease-gene associations | SFT, RAG | Classification | 2015.01 | EN | Academic and research resources, Integration of existing datasets, Scientific databases | Semi-automated | N/A | Data generation and review | NER tagger | 8,336,442 |
  | [BioReason ](https://github.com/bowang-lab/BioReason) | Molecular and Cellular Biology, Multi-omics | DNA sequence, KEGG pathways, Gene variants | SFT, CoT | Text QA with CoT | 2025.05 | EN | Scientific databases, Academic and research resources | Semi‑automated | N/A | N/A | Custom scripts | 87,620 |
  | [GeneChat ](https://drive.google.com/drive/folders/1CM4jSkQkEUhyaofDR1KKDRD2vOPsWLG5) | Multi-omics | Nucleotide sequence | Pre-training | Text QA | 2025.06 | EN | Scientific databases | N/A | N/A | Data generation | N/A | 47,275 |
  | [Genomics instructions ](https://huggingface.co/InstaDeepAI/ChatNT) | Multi-omics | Nucleotide sequence | SFT | Text QA | 2025.04 | EN | Academic and research resources | N/A | N/A | Data generation | N/A | 4,954,234 |
  | [scMMGPT data ](https://github.com/syr-cn/scMMGPT) | Multi-omics | scRNA-seq | Pre-training, SFT | scRNA-seq-text | 2025.03 | EN | Academic and research resources | Automated | N/A | N/A | N/A | 467K |
  | [OPI ](https://huggingface.co/datasets/BAAI/OPI) | Multi-omics | Protein | SFT | Text QA | 2025.03 | EN | Scientific databases | Semi-automated | N/A | Data generation | GPT-3.5 | 1,640,000 |
  | [OpenGenome2 ](https://huggingface.co/datasets/arcinstitute/opengenome2) | Multi-omics | Nucleotide sequence | Pre-training | Raw text | 2025.02 | EN | Integration of existing datasets | N/A | N/A | N/A | N/A | 8,800B (nucleotides) |
  | [Seq2Func ](https://huggingface.co/collections/zehui127/omni-dna-67a2230c352d4fd8f4d1a4bd) | Multi-omics | Nucleotide sequence | SFT | Text QA | 2025.02 | EN | Scientific databases | Automated | N/A | Data generation | N/A | 297,000 |
  | [DNA2Image ](https://huggingface.co/collections/zehui127/omni-dna-67a2230c352d4fd8f4d1a4bd) | Multi-omics | Nucleotide sequence | SFT | Generation | 2025.02 | EN | Scientific databases | Automated | N/A | Data generation | N/A | 43,200 |
  | [LLaMA-Gene (protein) ](https://huggingface.co/dnagpt/llama-gene-train-data) | Multi-omics | Protein sequence | Pre-training, SFT | Text QA | 2024.12 | EN | Scientific databases | N/A | N/A | Data generation | N/A | 62,918 |
  | [LLaMA-Gene (DNA) ](https://huggingface.co/dnagpt/llama-gene-train-data) | Multi-omics | DNA sequence | Pre-training, SFT | Text QA | 2024.12 | EN | Scientific databases | N/A | N/A | Data generation | N/A | 178,551 |
  | [OpenGenome ](https://huggingface.co/datasets/LongSafari/open-genome) | Multi-omics | Nucleotide sequence | Pre-training | Raw text | 2024.11 | EN | Integration of existing datasets | N/A | N/A | N/A | N/A | 300B (nucleotides) |
  | [The 1000G ](http://ftp.1000genomes.ebi.ac.uk/vol1/ftp/data_collections/1000G_2504_high_coverage/working/20201028_3202_phased/) | Multi-omics | Nucleotide sequence | Pre-training | Raw text | 2024.10 | EN | Scientific databases | N/A | N/A | N/A | N/A | 20,500B (nucleotides) |
  | [Multispecies dataset ](https://ftp.ncbi.nlm.nih.gov/genomes/refseq/) | Multi-omics | Nucleotide sequence | Pre-training | Raw text | 2024.10 | EN | Scientific databases | N/A | N/A | N/A | N/A | 174B (nucleotides) |
  | [NT Benchmark ](https://huggingface.co/datasets/InstaDeepAI/nucleotide_transformer_downstream_tasks_revised) | Multi-omics | Nucleotide sequence | SFT | Classification | 2024.10 | EN | Academic and research resources | N/A | N/A | N/A | N/A | 493,242 |
  | [ProteinLMDataset ](https://huggingface.co/datasets/tsynbio/ProteinLMDataset) | Multi-omics | Protein sequence | Pre-training | Raw text | 2024.06 | EN | Academic and research resources | Automated | N/A | N/A | N/A | 893,000 |
  | [RNAcentral ](https://rna-gpt.github.io/) | Multi-omics | RNA sequence | Pre-training | Raw text | 2024.05 | EN | Scientific databases | N/A | N/A | N/A | N/A | 23M |
  | [RNA-QA ](https://rna-gpt.github.io/) | Multi-omics | RNA sequence | SFT | Text QA | 2024.05 | EN | Academic and research resources | Automated | N/A | N/A | GPT-4o | 407,616 |
  | [ProCoT ](https://github.com/MingyuJ666/ProLLM) | Multi-omics | Biomedical QA | SFT, CoT | Text QA with CoT | 2024.05 | EN | Scientific databases, Academic and research resources | Semi‑automated | N/A | Data generation and review | embedding‑based filtering | 4,967,723 |
  | UniProtKB/Swiss-Prot | Multi-omics | Protein sequence | Pre-training | Raw text | 2023.11 | EN | Scientific databases | N/A | N/A | N/A | N/A | 570K |
  | [Multi-species genome ](https://drive.usercontent.google.com/download?id=1dSXJfwGpDSJ59ry9KAp8SugQLK35V83f) | Multi-omics | Nucleotide sequence | Pre-training | Raw text | 2023.06 | EN | Integration of existing datasets | N/A | N/A | N/A | N/A | 32.49B (nucleotides) |
  | [Genomic Benchmark ](https://github.com/ML-Bioinfo-CEITEC/genomic_benchmarks) | Multi-omics | Nucleotide sequence | SFT | Classification | 2023.05 | EN | Academic and research resources | N/A | N/A | N/A | N/A | 699,116 |
  | [CELLxGENE scRNA-seq Collection ](https://cellxgene.cziscience.com/) | Multi-omics | scRNA-seq | Pre-training | Gene Expression-pretrain | 2023.05 | EN | Scientific databases | N/A | N/A | N/A | N/A | 33 M |
  | [Human Pancreas ](https://github.com/JackieHanLab/TOSICA) | Multi-omics | scRNA-seq | SFT | Classification | 2023.01 | EN | Academic and research resources | N/A | N/A | N/A | N/A | 10,600 |
  | [scFoundation Dataset ](https://www.nature.com/articles/s41592-024-02305-7) | Multi-omics | scRNA-seq | Pre-training | Gene Expression-pretrain | 2022.10 | EN | Scientific databases | N/A | N/A | N/A | N/A | 50M |
  | [Human genome ](https://drive.usercontent.google.com/download?id=1dSXJfwGpDSJ59ry9KAp8SugQLK35V83f) | Multi-omics | Nucleotide sequence | Pre-training | Raw text | 2021.02 | EN | Scientific databases | N/A | N/A | N/A | N/A | 2.75B (nucleotides) |
  | [GPD ](https://www.sanger.ac.uk/data/gut-phage-database/) | Multi-omics | Nucleotide sequence | Pre-training | Raw text | 2021.02 | EN | Scientific databases | N/A | N/A | N/A | N/A | 142,809 |
  | [Myeloid ](http://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE154763) | Multi-omics | scRNA-seq | SFT | Classification | 2021.02 | EN | Academic and research resources | N/A | N/A | N/A | N/A | 9,748 |
  | [Human Cell Atlas Dataset ](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE159929) | Multi-omics | scRNA-seq | SFT | Classification | 2021.02 | EN | Academic and research resources | N/A | N/A | N/A | N/A | 84,363 |
  | [GVD ](https://de.cyverse.org/dl/d/E83EFBFF-2A23-4794-8819-ADD34160D018/FINAL_Gut_Viral_Database_GVD_1.7.2018.fna) | Multi-omics | Nucleotide sequence | Pre-training | Raw text | 2019.07 | EN | Scientific databases | N/A | N/A | N/A | N/A | 13,203B |
  | [Multiple Sclerosis ](https://www.ebi.ac.uk/gxa/sc/experiments/E-HCAD-35) | Multi-omics | scRNA-seq | SFT | Classification | 2019.07 | EN | Academic and research resources | N/A | N/A | N/A | N/A | 7,844 |
  | [PanglaoDB ](https://panglaodb.se/) | Multi-omics | scRNA-seq | Pre-training | Gene Expression-pretrain | 2018.11 | EN | Scientific databases | N/A | N/A | N/A | N/A | 1,126,580 |
  | [Zheng68k ](https://support.10xgenomics.com/single-cell-gene-expression/datasets) | Multi-omics | scRNA-seq | SFT | Classification | 2016.07 | EN | Academic and research resources | N/A | N/A | N/A | N/A | 68,450 |
  | [GRCh38/hg38 ](https://www.ncbi.nlm.nih.gov/datasets/genome/GCF_000001405.26/) | Multi-omics | Nucleotide sequence | Pre-training | Raw text | 2013.12 | EN | Scientific databases | N/A | N/A | N/A | N/A | 3.1B (nucleotides) |
  | [Biology-Instructions ](https://github.com/hhnqqq/Biology-Instructions) | Multi-omics | DNA, RNA, Protein sequence | SFT | Text QA | 2024.12 | EN | Academic and research resources | Semi-automated | N/A | Data generation | GPT-4o, Claude-3.5-sunnet | 3.3 M |
  | [TCPA ](https://tcpaportal.org/) | Multi-omics | Protein sequence | Pre-training | Raw text | 2013.09 | EN | Academic and research resources | N/A | N/A | N/A | N/A | 4,379 |
  | [NCBI-GenBank ](https://www.ncbi.nlm.nih.gov/genbank/) | Multi-omics | Nucleotide sequence | Pre-training | Raw text | 2012.11 | EN | Scientific databases | N/A | N/A | N/A | N/A | 5,000B (nucleotides) |
  | [GRCh37/hg19 ](https://www.ncbi.nlm.nih.gov/datasets/genome/GCF_000001405.13/) | Multi-omics | Nucleotide sequence | Pre-training | Raw text | 2009.02 | EN | Scientific databases | N/A | N/A | N/A | N/A | 3.1B (nucleotides) |
  | [Neuro-3D ](https://huggingface.co/datasets/guozq21/neuro-3D) | Neuroscience | EEG | Pre-training, SFT | Classification | 2025.03 | EN | Academic and research resources | Semi-automated | N/A | N/A | N/A | 720 |
  | [Things-MEG ](https://openneuro.org/datasets/ds004212/versions/3.0.0) | Neuroscience | MEG | Pre-training, SFT | Classification | 2023.04 | EN | Academic and research resources | Semi-automated | N/A | N/A | N/A | 22,248 |
  | [Things-EEG2 ](https://osf.io/3jk45/) | Neuroscience | EEG | Pre-training, SFT | Classification | 2022.11 | EN | Academic and research resources | Semi-automated | N/A | N/A | N/A | 16,740 |
  | [SHU ](https://figshare.com/articles/code/shu_dataset/19228725) | Neuroscience | EEG | Pre-training, SFT | Classification | 2022.08 | EN | Academic and research resources | Semi-automated | N/A | N/A | N/A | 11,988 |
  | [Things-fMRI ](https://openneuro.org/datasets/ds004192/versions/1.0.1) | Neuroscience | fMRI | Pre-training, SFT | Classification | 2022.07 | EN | Academic and research resources | Semi-automated | N/A | N/A | N/A | 8,740 |
  | [NSD-Imagery ](https://openneuro.org/datasets/ds004192/versions/1.0.1) | Neuroscience | fMRI | Pre-training, SFT | Classification | 2022.07 | EN | Academic and research resources | Semi-automated | N/A | N/A | N/A | 2,304 |
  | [HMC ](https://physionet.org/content/hmc-sleep-staging/1.1/) | Neuroscience | EEG | Pre-training, SFT | Classification | 2022.03 | EN | Academic and research resources | Semi-automated | N/A | N/A | N/A | 154 |
  | [Things-EEG1 ](https://osf.io/hd6zk/) | Neuroscience | EEG | Pre-training, SFT | Classification | 2022.01 | EN | Academic and research resources | Semi-automated | N/A | N/A | N/A | 22,248 |
  | [NSD ](https://naturalscenesdataset.org) | Neuroscience | fMRI | Pre-training, SFT | Classification | 2021.09 | EN | Academic and research resources | Semi-automated | N/A | N/A | N/A | 70,566 |
  | [ZuCo2 ](https://osf.io/2urht/) | Neuroscience | EEG | Pre-training, SFT | Text QA | 2019.11 | EN | Academic and research resources | Semi-automated | N/A | N/A | N/A | 739 |
  | [DIR ](https://openneuro.org/datasets/ds001506/versions/1.3.1) | Neuroscience | fMRI | Pre-training, SFT | Classification | 2019.01 | EN | Academic and research resources | Semi-automated | N/A | N/A | N/A | 6,000 |
  | [Workload ](https://physionet.org/content/eegmat/1.0.0/) | Neuroscience | EEG | Pre-training, SFT | Classification | 2018.12 | EN | Academic and research resources | Semi-automated | N/A | N/A | N/A | 1080 |
  | [ZuCo1 ](https://osf.io/q3zws/) | Neuroscience | EEG | Pre-training, SFT | Text QA | 2018.11 | EN | Academic and research resources | Semi-automated | N/A | N/A | N/A | 1,107 |
  | [SEED-IV ](https://bcmi.sjtu.edu.cn/home/seed/seed-iv.html) | Neuroscience | EEG | Pre-training, SFT | Classification | 2018.02 | EN | Academic and research resources | Semi-automated | N/A | N/A | N/A | 143,610 |
  | [TUSL ](https://isip.piconepress.com/projects/nedc/html/tuh_eeg/#c_tusl) | Neuroscience | EEG | Pre-training, SFT | Classification | 2018.01 | EN | Academic and research resources | Semi-automated | N/A | N/A | N/A | 245 |
  | [TUEV ](https://isip.piconepress.com/projects/nedc/html/tuh_eeg/#c_tusl) | Neuroscience | EEG | Pre-training, SFT | Classification | 2015.12 | EN | Academic and research resources | Semi-automated | N/A | N/A | N/A | 112,237 |
  | [TUAB ](https://isip.piconepress.com/projects/nedc/html/tuh_eeg/#c_tusl) | Neuroscience | EEG | Pre-training, SFT | Classification | 2015.12 | EN | Academic and research resources | Semi-automated | N/A | N/A | N/A | 409,083 |
  | [SEED ](https://bcmi.sjtu.edu.cn/home/seed/) | Neuroscience | EEG | Pre-training, SFT | Classification | 2015.05 | EN | Academic and research resources | Semi-automated | N/A | N/A | N/A | 144,851 |
  | [Sleep-EDF ](https://www.physionet.org/content/sleep-edf/1.0.0/) | Neuroscience | EEG | Pre-training, SFT | Classification | 2013.10 | EN | Academic and research resources | Semi-automated | N/A | N/A | N/A | 197 |
  | [SHHS ](https://sleepdata.org/datasets/shhs) | Neuroscience | EEG | Pre-training, SFT | Classification | 1998.01 | EN | Academic and research resources | Semi-automated | N/A | N/A | N/A | 6,441 |
  | [repoDB ](https://unmtid-shinyapps.net/shiny/repodb/) | Pharmacy, Healthcare and Medical Sciences | Drug-disease relationships, Clinical trials | RAG | Classification, Text QA | 2017.03 | EN | Scientific databases | Automated | N/A | N/A | scripts | 15,648 |
  | [MedMax Train ](https://huggingface.co/datasets/mint-medmax/medmax_data) | Curated Version of Several Biomedical Datasets | Academic papers, YouTube Videos | Pre-training, SFT | VQA, Visual Chat, Interleaved Vision-Language Data, Image Generation, and Captioning | 2024.12 | EN | Academic and research resources | Automated | N/A | N/A | GPT-4o-mini and GPT-4o | 1,470,000 |
</details>

<details>
<summary>
  
### ⚗️ Chemistry

</summary>

 <a href="#-table-of-contents" style="float:right;">⬆ Back to Top</a>
  Dataset | Domain | Modality | Purpose | Type | Release | Language | Source | Annotation  Pipeline | Human   Annotators | Human Tasks | Auto-annotation  Tools | Size |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| [MOSES ](https://tdcommons.ai/generation_tasks/molgen/) | Biochemistry | SMILES | Pre-training | Raw text | 2020.07 | EN | Academic and research resources | Automated | N/A | Data generation and review | N/A | 1,936,962 |
| [ChemBL ](https://www.ebi.ac.uk/chembl/) | Biochemistry | SMILES | Pre-training | Raw text | 2012.01 | EN | Academic and research resources | Automated | N/A | Data generation and review | N/A | 1,961,462 |
| [ChemRxivQuest ](https://arxiv.org/pdf/2505.05232) | General Chemistry | Academic papers | Pre-training, SFT | Text QA | 2025.05 | EN | Academic and research resources | Manual | N/A | Data generation and review | N/A | 970 |
| [ScholarChemQA ](https://github.com/iriscxy/chemmatch) | General Chemistry | Academic papers | Pre-training, SFT | Text QA | 2025.02 | EN | Academic and research resources | Manual | N/A | Data generation and review | N/A | 40K |
| [SMolInstruct ](https://huggingface.co/datasets/osunlp/SMolInstruct) | General Chemistry | SMILES | SFT | Text QA | 2024.08 | EN | Scientific databases | Semi-automated | N/A | Data generation and review | GPT-4 | 3.3M |
| [ChemNLP ](https://huggingface.co/datasets/lavita/medical-qa-shared-task-v1-all) | General Chemistry | Text | Pre-training, SFT | Classification | 2023.01 | EN | Academic and research resources | Manual | N/A | Data generation and review | N/A | 110,342 |
| [PMO ](https://github.com/wenhao-gao/mol_opt) | General Chemistry | SMILES | Pre-training, SFT | Raw text | 2022.05 | EN | Academic and research resources | Automated | N/A | Data generation and review | N/A | 10K |
| [ZINC ](https://zinc.docking.org/) | General Chemistry | SMILES | Pre-training | Raw text | 2012.10 | EN | Academic and research resources | Automated | N/A | Data generation and review | N/A | 250K |
| [DeepProtein ](https://github.com/jiaqingxie/DeepProtein) | Pharmacy | Protein sequence, SMILES | Pre-training, SFT | Raw text | 2025.05 | EN | Academic and research resources | Automated | N/A | Data generation and review | N/A | 78K |
| [TrialBench ](https://huyjj.github.io/Trialbench/) | Pharmacy | SMILES, Disease code | Pre-training, SFT | Raw text | 2024.09 | EN | Academic and research resources | Automated | N/A | Data generation and review | N/A | 470K |
| [TDC2 ](https://tdcommons.ai/) | Pharmacy | SMILES, Protein sequence, Genome sequence | Pre-training, SFT | Classification, Regression, Generation | 2024.09 | EN | Academic and research resources | Manual | N/A | Data generation and review | N/A | 3.4B (tokens) |
| [SBDDBench ](https://github.com/futianfan/reinforced-genetic-algorithm) | Pharmacy | Text, Protein sequence, SMILES | Pre-training, SFT | Protein-ligand | 2022.06 | EN | Academic and research resources | Automated | N/A | Data generation and review | N/A | 5K |
| [TOP ](https://github.com/futianfan/HINT) | Pharmacy | SMILES | Pre-training, SFT | Raw text | 2022.02 | EN | Academic and research resources | Automated | N/A | Data generation and review | N/A | 12K |
| [TDC ](https://tdcommons.ai/) | Pharmacy | SMILES, Protein sequence, Genome sequence | Pre-training, SFT | Classification, Regression, Generation | 2021.06 | EN | Academic and research resources | Manual | N/A | Data generation and review | N/A | 0.2B (tokens) |
| [DeepPurpose ](https://github.com/kexinhuang12345/DeepPurpose) | Pharmacy | Protein sequence, SMILES | Pre-training, SFT | Raw text | 2020.12 | EN | Academic and research resources | Automated | N/A | Data generation and review | N/A | 5,074 |
| [DrugBank ](https://go.drugbank.com/) | Pharmacy | SMILES | Pre-training, SFT | Raw text | 2018.01 | EN | Academic and research resources | Manual | N/A | Data generation and review | N/A | 18K |
| [DrugCentral ](https://drugcentral.org/) | Pharmacy | SMILES | Pre-training, SFT | Raw text | 2017.01 | EN | Academic and research resources | Automated | N/A | Data generation and review | N/A | 4,995 |
| USPTO | Synthetic Chemistry | SMILES | Pre-training, SFT | Generation | 2015.07 | EN | Patent databases | Manual | N/A | Data generation and review | N/A | 1,939,253 |
</details>

<details>
<summary>
  
### ⚛️ Physics

</summary>

 <a href="#-table-of-contents" style="float:right;">⬆ Back to Top</a>
  Dataset | Domain | Modality | Purpose | Type | Release | Language | Source | Annotation  Pipeline | Human   Annotators | Human Tasks | Auto-annotation  Tools | Size |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| [MM-PhyQA ](https://arxiv.org/pdf/2404.08704) | General Physics | High-school exams | SFT, CoT | VQA with CoT | 2024.04 | EN | Web and Internet content | Manual | N/A | Data generation and review | AFL 3.0 | 3,825 |
| [PIQA ](https://yonatanbisk.com/piqa/) | General Physics | Text | SFT | Text QA | 2020.01 | EN | Other sources | Semi-automated | AFLite | Data generation and review | N/A | 19,838 |

</details>

<details>
<summary>
  
### 🌌 Astronomy

</summary>

 <a href="#-table-of-contents" style="float:right;">⬆ Back to Top</a>
  Dataset | Domain | Modality | Purpose | Type | Release | Language | Source | Annotation  Pipeline | Human   Annotators | Human Tasks | Auto-annotation  Tools | Size |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| [AstroLLaVA ](https://github.com/UniverseTBD/AstroLLaVA) | Astronomy | General dialog, Astronomical images | SFT | VQA | 2025.04 | EN | Comprehensive multi-source integration | Semi-automated | N/A | Data review | GPT-4 | 29,783 |
| [AstroPT ](https://www.github.com/Smith42/astroPT) | Astronomy | Astronomical images | Pre-training | Regression | 2024.05 | EN | Web and Internet content, Scientific databases | Automated | N/A | Data review | DESI Legacy Survey API | 8.6M (tokens) |
| [Astro-NER ](https://arxiv.org/pdf/2405.02602?) | Astronomy | Academic papers | SFT | Text QA | 2024.05 | EN | Academic and research resources | Semi-automated | 4 | Data generation and review | GPT-3.5 | 5000 |
| [AstroLLaMA-chat ](https://huggingface.co/UniverseTBD) | Astronomy | Academic papers | SFT | Text QA | 2024.01 | EN | Academic and research resources | Manual | N/A | Data review | N/A | 10,356 |
| [AstroLLaMA ](https://huggingface.co/UniverseTBD/astrollama) | Astronomy | Academic papers | SFT | Text QA | 2023.09 | EN | Academic and research resources, Web and Internet content | Manual | N/A | Data review | N/A | 9.5M |
| [ATel ](https://github.com/JetBrains/lm-astronomy) | Astronomy | Academic papers | SFT | Text QA | 2023.05 | EN | Academic and research resources | Manual | N/A | Data review | N/A | 234 |
| [AstroBERT ](https://arxiv.org/pdf/2112.00590) | Astronomy | Academic papers | Pre-training | Raw text | 2022.11 | EN | Academic and research resources | Automated | 12 | Data generation and review | N/A | 3.8B (tokens) |
| [AstroMLab 4 ](https://huggingface.co/AstroMLab) | Astronomy | Academic papers | SFT | Text QA | 2025.05 | EN | Integration of existing datasets | Automated | N/A | Data generation and review | Gemini-1.5-Pro | 250,000 arXiv preprints |
| [AstroMLab 3 ](https://huggingface.co/AstroMLab) | Astronomy | Academic papers | SFT | Text QA | 2025.04 | EN | Academic and research resources | Automated | N/A | Data generation and review | Gemini-1.5-Pro | 3.3B (tokens) |
| [AstroMLab 2 ](https://huggingface.co/datasets/UniverseTBD/arxiv-qa-astro-ph) | Astronomy | Academic papers | SFT | Text QA | 2024.09 | EN | Academic and research resources | Automated | N/A | Data generation and review | Gemini-1.5-Pro | 10,356 |
| [Starwhisper-pilsar ](https://github.com/ACMISLab/StarWhisper-Pulsar) | Astrophysics | Text, pulsar diagnostic plots, pulsars signals | SFT | Classification | 2024.04 | EN | Integration of existing datasets | Manual | N/A | Data generation and review | DeepSeek-VL-7B, InternVL2-40B | 106,674 |
| [PAPERCLIP ](https://www.github.com/smsharma/PAPERCLIP-Hubble) | Astrophysics | synthetic conversation text, Astronomical images | SFT | Image-text | 2024.03 | EN | Academic and research resources | Automated | N/A | Data review | Mixtral-8x7B-Instruct | 31,859 |

</details>

<details>
<summary>
  
### 🪨 Materials Science

</summary>

 <a href="#-table-of-contents" style="float:right;">⬆ Back to Top</a>
| Dataset | Domain | Modality | Purpose | Type | Release | Language | Source | Annotation  Pipeline | Human   Annotators | Human Tasks | Auto-annotation  Tools | Size |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| [ChEBI-20-MM ](https://huggingface.co/datasets/liupf/ChEBI-20-MM) | Materials Science | InChI, IUPAC, SELFIES, Molecular image | SFT | Text QA | 2025.01 | EN | Integration of existing datasets | Manual | N/A | Data generation and review | N/A | 29,706 |
| [Materials Project Trajectory ](https://figshare.com/articles/dataset/Materials_Project_Trjectory_MPtrj_Dataset/23713842?file=41619375) | Materials Science | CIF | Pre-training | Raw text | 2023.07 | EN | Scientific databases | Manual | N/A | Data generation and review | N/A | 1,580,395 |
| [DigiMOF ](https://github.com/peymanzmoghadam/DigiMOF-database-master-main) | Materials Science | CIF | Pre-training | Raw text | 2023.05 | EN | Academic and research resources | Manual | N/A | Data generation and review | N/A | 15,501 |
| [Novel Materials Discovery (NOMAD) ](https://nomad-lab.eu) | Materials Science | CIF | Pre-training | Raw text | 2023.03 | EN | Scientific databases | Manual | N/A | Data generation and review | N/A | 4,341,443 |
| [MOFX-DB (hMOF) ](https://mof.tech.northwestern.edu/databases) | Materials Science | CIF | Pre-training | Raw text | 2023.02 | EN | Integration of existing datasets | Manual | N/A | Data generation and review | N/A | 160,000 |
| [MatScholar ](https://github.com/materialsintelligence/mat2vec) | Materials Science | Academic papers | Pre-training | Raw text | 2022.07 | EN | Academic and research resources | Manual | N/A | Data generation and review | N/A | 5M |
| [Pfeiffer et al. Chemical composition ](https://github.com/olivettigroup/table_extractor) | Materials Science | Chemical Composition | Pre-training | Raw text | 2022.03 | EN | Comprehensive multi-source integration | Manual | N/A | Data generation and review | N/A | 14,884 |
| [Pfeiffer et al. Mechanical Properties ](https://github.com/olivettigroup/table_extractor) | Materials Science | Numerical property | Pre-training | Raw text | 2022.03 | EN | Comprehensive multi-source integration | Manual | N/A | Data generation and review | N/A | 1,278 |
| [ChEBI-20 ](https://github.com/cnedwards/text2mol) | Materials Science | Scientific instruction | SFT | Text QA | 2021.11 | EN | Integration of existing datasets | Manual | N/A | Data generation and review | N/A | 29709 |
| [ZINC ](https://zinc.docking.org/) | Materials Science | SMILES | Pre-training | Raw text | 2020.12 | EN | Scientific databases | Manual | N/A | Data generation and review | N/A | 230M |
| [JARVIS-DFT ](https://jarvis.nist.gov/) | Materials Science | InChI, IUPAC, SELFIES | Pre-training | Raw text | 2020.11 | EN | Integration of existing datasets | Manual | N/A | Data generation and review | N/A | 41,000 |
| [MOSES ](https://github.com/molecularsets/moses) | Materials Science | SMILES | SFT | Text QA | 2020.11 | EN | Integration of existing datasets | Manual | N/A | Data generation and review | N/A | 1.6M |
| [QMOF ](https://figshare.com/articles/dataset/QMOF_Database/13147324) | Materials Science | CIF | Pre-training | Raw text | 2020.05 | EN | Academic and research resources | Manual | N/A | Data generation and review | N/A | 20,000 |
| [Warwick Electron Microscopy Datasets ](https://github.com/Jeffrey-Ede/datasets?tab=readme-ov-file) | Materials Science | STEM image, TEM image, TEM exit wavefunction | SFT | VQA | 2020.05 | EN | Academic and research resources | Manual | N/A | Data generation and review | N/A | 135395 |
| [CoRE MOF 2019 ](https://zenodo.org/records/3370144#.X2Ao4Wgzb-g) | Materials Science | CIF | Pre-training | Raw text | 2019.12 | EN | Integration of existing datasets | Manual | N/A | Data generation and review | N/A | 14,000 |
| [Inorganic Crystal Structure Database (ICSD) ](https://icsd.products.fiz-karlsruhe.de/) | Materials Science | CIF | Pre-training | Raw text | 2019.10 | EN | Scientific databases | Manual | N/A | Data generation and review | N/A | 318,901 |
| [US Patent Office (USPTO) ](https://figshare.com/articles/dataset/Chemical_reactions_from_US_patents_1976-Sep2016_/5104873) | Materials Science | SMILES | Pre-training | Raw text | 2017.06 | EN | Patent databases | Manual | N/A | Data generation and review | N/A | 2,830,616 |
| [Open Quantum Materials Database (OQMD) ](https://oqmd.org/) | Materials Science | CIF | Pre-training | Raw text | 2014.11 | EN | Scientific databases | Manual | N/A | Data generation and review | N/A | 1,317,811 |
| [Materials Project ](https://next-gen.materialsproject.org/) | Materials Science | CIF | Pre-training | Raw text | 2013.07 | EN | Scientific databases | Manual | N/A | Data generation and review | N/A | 577,813 |
</details>

<details>
<summary>

### 🌍 Earth Science

</summary>

 <a href="#-table-of-contents" style="float:right;">⬆ Back to Top</a>
  Dataset | Domain | Modality | Purpose | Type | Release | Language | Source | Annotation  Pipeline | Human   Annotators | Human Tasks | Auto-annotation  Tools | Size |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| [WeatherQA ](https://huggingface.co/datasets/ZhanxiangHua/WeatherQA_SFT) | Atmosphere | Remote sensing, Science QA | SFT | VQA | 2024.06 | EN | Scientific databases | Semi-automated | 4 | Data review | GPT-4 | 8,511 |
| [SeafloorAI ](https://github.com/deep-real/SeafloorAI) | Hydrosphere | Sonar images, Text | SFT | VQA | 2024.11 | EN | Scientific databases | Semi-automated | 4 | Data review | GPT-4 | 7M |
| [TEOChatlas ](https://huggingface.co/datasets/jirvin16/TEOChatlas) | Lithosphere | Remote sensing | SFT | VQA | 2025.01 | EN | Scientific databases | Automated | N/A | Data generation | N/A | 554K |
| [EarthVQA ](https://github.com/Junjue-Wang/EarthVQA) | Lithosphere | Remote sensing, Science QA | SFT | VQA | 2023.12 | EN | Scientific databases | Automated | N/A | Data generation | ArcGIS toolbox | 208K |
| [Geochat ](https://huggingface.co/datasets/MBZUAI/GeoChat_Instruct) | Lithosphere | Remote sensing, Science QA | SFT | VQA | 2023.11 | EN | Scientific databases | Automated | N/A | Data generation | Vicuna-v1.5 | 306K |
| [FloodNet ](https://github.com/BinaLab/FloodNet-Challenge-EARTHVISION2021) | Lithosphere | Remote sensing, Science QA | SFT | VQA | 2021.05 | EN | Scientific databases | Manual | N/A | Data generation and review | N/A | 11K |
| [GeoSignal ](https://huggingface.co/datasets/daven3/geosignal) | Lithosphere, Hydrosphere, Atmosphere | Remote sensing, Science QA | SFT | Text QA | 2023.06 | EN | Encyclopedias and knowledge bases, Academic and research resources, Scientific databases, Comprehensive multi-source integration | Semi-automated | 10 | Data review | GPT-4 | 39,749 |
| [GeoLLaVA-8k ](https://github.com/MiliLab/GeoLLaVA-8K) | Remote Sensing | Remote sensing | SFT | Image-text, VQA | 2025.05 | EN | Academic and research resources | Semi-automated | 35 | Data generation and review | GPT-4o | 81,367 |
| [EVAttrs-95k ](https://github.com/XiangTodayEatsWhat/EagleVision) | Remote Sensing | Remote sensing, Object property | SFT | Image-text, VQA | 2025.03 | EN | Academic and research resources | Semi-automated | N/A | Data generation and review | Qwen2-VL-72B, GPT-4o | 95.1K |
| [VersaD ](https://github.com/opendatalab/VHM) | Remote Sensing | Remote sensing | Pre-training | Image-text | 2024.11 | EN | Academic and research resources | Automated | N/A | N/A | Gemini-Vision | 1.4M |
| [RSVP ](https://github.com/lx709/VRSBench) | Remote Sensing | Remote sensing | SFT | Image-text, VQA | 2024.10 | EN | Integration of existing datasets, Academic and research resources | Automated | N/A | N/A | GPT-4V, DINOv2-ViT L/14, CLIP-ConvNeXt | 3.65M |
| [FIT-RS ](https://github.com/Luo-Z13/SkySenseGPT) | Remote Sensing | Remote sensing, Relation graph, \etc | SFT | Image-text, VQA | 2024.07 | EN | Integration of existing datasets, Academic and research resources | Semi-automated | N/A | Data generation | TinyLLaVA-3.1B, GPT-4, GPT-3.5, CLIP-ViT-L14 | 1,415K |
| [VRSBench ](https://github.com/lx709/VRSBench) | Remote Sensing | Remote sensing | SFT | Image-text, VQA | 2024.06 | EN | Academic and research resources | Semi-automated | N/A | Data review | GPT-4V | 142,390 |
| [MMRS-1M ](https://github.com/wivizhang/EarthGPT) | Remote Sensing | Remote sensing, Optical, SAR, Infrared, \etc | SFT | Image-text, VQA | 2024.03 | EN | Integration of existing datasets | Automated | N/A | N/A | N/A | 1.06M |
| [ChatEarthNet ](https://github.com/zhu-xlab/ChatEarthNet) | Remote Sensing | Remote sensing, Optical, Multi-band | SFT | Image-text | 2024.02 | EN | Scientific databases | Semi-automated | N/A | Data review | GPT-3.5, GPT-4V | 173,488 |
| [LHRS-Align ](https://github.com/NJU-LHRS/LHRS-Bot) | Remote Sensing | Remote sensing | Pre-training | Image-text | 2024.02 | EN | Scientific databases | Automated | N/A | N/A | Vicuna-v1.5-13B | 1.15M |
| [LHRS-Instruct ](https://github.com/NJU-LHRS/LHRS-Bot) | Remote Sensing | Remote sensing | SFT | Image-text, VQA | 2024.02 | EN | Integration of existing datasets, Academic and research resources | Semi-automated | N/A | Data review | Vicuna-v1.5-13B, GPT-4 | 12K |
| [RS5M ](https://github.com/om-ai-lab/RS5M) | Remote Sensing | Remote sensing | Pre-training | Image-text | 2024.01 | EN | Scientific databases | Automated | N/A | N/A | CLIP | 5.07M |
| [SkyEye-968k ](https://github.com/ZhanYang-nwpu/SkyEyeGPT) | Remote Sensing | Remote sensing | SFT | Image-text, Video-text, VQA | 2024.01 | EN | Integration of existing datasets | Semi-automated | N/A | Data review | N/A | 968K |
| [SkyScript ](https://github.com/wangzhecheng/SkyScript) | Remote Sensing | Remote sensing | Pre-training | Image-text | 2023.12 | EN | Academic and research resources, Scientific databases | Automated | N/A | N/A | CLIP, Logistic Regression model | 2.6M |
| [RSICap ](https://github.com/Lavender105/RSGPT) | Remote Sensing | Remote sensing | SFT | Image-text | 2023.07 | EN | Academic and research resources | Manual | 5 | Data generation, Data review | N/A | 2.5K |

</details>

<details>
<summary>

### 🔭 General Science

</summary>

 <a href="#-table-of-contents" style="float:right;">⬆ Back to Top</a>
  Dataset | Domain | Modality | Purpose | Type | Release | Language | Source | Annotation  Pipeline | Human   Annotators | Human Tasks | Auto-annotation  Tools | Size |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| [NaturalReasoning ](https://huggingface.co/datasets/facebook/natural_reasoning) | Multidisciplinary (incl. Physics) | Text | SFT | Text QA with CoT | 2025.02 | EN | Web and Internet content, Books and literary works, Academic and research resources | Semi-automated | N/A | Data review | LLaMA-70B | 2.8M |
  | [Nemotron-Science ](https://huggingface.co/datasets/nvidia/nemotron-science) | Multidisciplinary (incl. Physics) | Text with formulae and code | SFT, RLHF | Text QA with CoT | 2025.05 | EN | Social media and forums, Academic and research resources, Books and literary works | Semi-automated | N/A | Data review | DeepSeek-R1 | 2.7M |
  | [Galactica ](https://galactica.org/) | Multidisciplinary (incl. Chemistry) | Text (incl. formulas, code) | Pre-training | Raw text | 2022.11 | EN | Webpages | Fully-automated | N/A | Data generation and review | Custom crawlers, PDF parsers | 106B tokens |
  | [SciBERT ](https://github.com/allenai/scibert) | Multidisciplinary (incl. Physics) | Academic papers | Pre-training | Raw text | 2019.09 | EN | Academic and research resources | Automated | N/A | Data generation | Crawlers, text processing tools | 3.3B (tokens) |
  | [ArXivCap ](https://mm-arxiv.github.io/) | Physics, Biology, \etc | Paper figures | Pre-training | Image-text | 2024.05 | EN | Academic and research resources | Semi-automated | 7 | Data review | PDF parsers | 6.4M |
  | [SCP-116K ](https://github.com/AQA6666/SCP-116K-open) | Physics, Chemistry, Biology, \etc | Text with formulae | SFT | Text QA with CoT | 2025.01 | EN | Academic and research resources, Books and literary works | Semi-automated | N/A | Data review | PDF parsers, OCR, LaTeX rendering | 116.8K |
  | [MegaScience ](https://github.com/GAIR-NLP/MegaScience) | Medicine, Physics, Chemistry, Biology | Science textbooks | SFT | Text QA with CoT | 2024.08 | EN | Web and Internet content, Books and literary works, Integration of existing datasets | Semi-automated | N/A | Data review | Llama3.3-70B-Instruct, DeepSeek-V3, BGE-large-en-v1.5 | 651,840 |
</details>

## 📝 Scientific Evaluation Datasets

<details>
<summary>

### 🧬 Life Science

</summary>

 <a href="#-table-of-contents" style="float:right;">⬆ Back to Top</a>
| Dataset | Domain | Modality | Level | Type | Release | Language | Source | Annotation Pipeline | Human Annotators | Human Tasks | Auto-annotation Tools | Size | Evaluation Type | Metrics |
---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| [SeedBench ](https://arxiv.org/pdf/2505.13220) | Agriculture | Breeding literature | Expert | Text QA | 2025.05 | EN, ZH | Academic and research resources | Semi-automated | N/A | Data generation and review | GPT-4 | 2,264 | MCQ, Open-ended | Acc, F1, ROUGE |
| [AgEval ](https://arxiv.org/abs/2407.19617) | Agriculture | Plant stress phenotyping photos and annotations | Expert | VQA | 2025.01 | EN | Scientific databases | N/A | N/A | N/A | N/A | 1,200 | Classification, Regression | F1, NMAE |
| [AgXQA ](https://dl.acm.org/doi/10.1016/j.compag.2024.109349) | Agriculture | Agricultural extension records | Expert | Text QA | 2024.10 | EN | Academic and research resources | Semi-automated | N/A | N/A | N/A | 2,186 | Open-ended | EM, F1 |
| [Fundus-MMBench ](https://huggingface.co/datasets/MeteorElf/Fundus-MMBench) | Healthcare and Medical Sciences | CFP | Expert | VQA | 2025.07 | EN | Integration of existing datasets | Manual | N/A | Data review | N/A | 620 | MCQ | Acc |
| [ReXVQA ](https://huggingface.co/datasets/rajpurkarlab/ReXVQA) | Healthcare and Medical Sciences | X-ray | N/A | VQA | 2025.06 | EN | Integration of existing datasets | Semi-automated | 3 | Data review | GPT-4o, ClinicalBERT, MedEmbed | 40,557 | MCQ | Acc |
| [HealthBench ](https://openai.com/index/healthbench/) | Healthcare and Medical Sciences | Clinical dialogue, Medical task requests, Medical record summarization, \etc | Expert | Text QA | 2025.05 | EN | Comprehensive multi-source integration | Semi-automated | 262 | Data generation and review | GPT-o1, GPT-4.1 | 5,000 | Open-ended | Customized rubric criterion |
| [MedAlpaca ](https://arxiv.org/abs/2304.08247) | Healthcare and Medical Sciences | Biomedical knowledge base | Expert | Text QA | 2025.03 | EN | Web and Internet content | Semi-automated | N/A | Data review | GPT-3.5-Turbo | 374 | MCQ | Acc |
| [GEMeX-VQA ](https://huggingface.co/datasets/BoKelvin/GEMeX-VQA) | Healthcare and Medical Sciences | X-ray | N/A | VQA | 2025.03 | EN | Integration of existing datasets | Semi-automated | N/A | Data review | OpenBioLLM-70B, GPT-4o | 3,960 | MCQ, True/False, Open-ended | Acc |
| [MIMIC-Diff-VQA ](https://physionet.org/content/medical-diff-vqa/) | Healthcare and Medical Sciences | X-ray | Expert | VQA (multi-image) | 2025.02 | EN | Scientific databases | Semi-automated | 3 | Data generation and review | ScispaCy | 70,070 | MCQ, Open-ended | BLEU, METEOR, ROUGE-L, CIDEr |
| [MedAgentBench ](https://github.com/stanfordmlgroup/MedAgentBench) | Healthcare and Medical Sciences | EHR, Lab results, Diagnosis codes, Medication orders | Expert | Text QA | 2025.01 | EN | Academic and research resources | Manual | 2 | Data generation and review | N/A | 300 | Open-ended | Success rate |
| [MedXpertQA ](https://huggingface.co/datasets/TsinghuaC3I/MedXpertQA) | Healthcare and Medical Sciences | CT, ECG, Histopathology, MRI, US, X-ray, \etc | Expert | VQA, Text QA | 2025.01 | EN | Academic and research resources | Semi-automated | N/A | Data generation and review | GPT-4o, Claude | 4,460 | MCQ | Acc |
| [OpenMM-Medical ](https://huggingface.co/datasets/baichuan-inc/OpenMM_Medical) | Healthcare and Medical Sciences | CT, Dermatology, Endoscopy, CFP, MRI, Microscopy, X-ray, \etc | N/A | VQA | 2025.01 | EN, ZH | Comprehensive multi-source integration | Semi-automated | N/A | Data review | GPT-4o | 88,996 | MCQ | Acc |
| [Asclepius ](https://github.com/Asclepius-Med/Asclepius) | Healthcare and Medical Sciences | CT, Dermatology, CFP, Histopathology, MRI, Microscopy, OCT, X-ray, \etc | N/A | VQA, Image-text | 2024.11 | EN | Comprehensive multi-source integration | Semi-automated | 34 | Data generation and review | ChatGPT, GPT-4V, GPT-4o | 3,232 | MCQ | Acc |
| [ClinicalBench ](https://clinicalbench.github.io/) | Healthcare and Medical Sciences | EHR | N/A | Text QA | 2024.11 | EN | Integration of existing datasets | N/A | N/A | N/A | N/A | N/A | MCQ | F1, AUROC |
| [WorldMedQA-V ](https://huggingface.co/datasets/WorldMedQA/V) | Healthcare and Medical Sciences | Dermatology, Microscopy, X-ray, \etc | N/A | VQA | 2024.10 | EN, JA, ES, HE, PT | Academic and research resources | Semi-automated | N/A | Data review | GPT-4o, Gemini Flash1-5, Yi-VL-34B | 568 | MCQ | Acc |
| [CRAFT-BioQA ](https://huggingface.co/datasets/ingoziegler/CRAFT-BioQA) | Healthcare and Medical Sciences | Biomedical QA | N/A | Text QA | 2024.09 | EN | Academic and research resources | Automated | N/A | N/A | N/A | N/A | MCQ | Acc |
| [MedTrinity-25M ](https://huggingface.co/datasets/UCSC-VLAA/MedTrinity-25M) | Healthcare and Medical Sciences | CT, MRI, X-ray, Histopathology, \etc | Expert | Image-text, VQA | 2024.08 | EN | Integration of existing datasets, Scientific databases | Automated | N/A | N/A | N/A | 100,000 | Open-ended | Acc |
| [GMAI-MMBench ](https://huggingface.co/datasets/OpenGVLab/GMAI-MMBench) | Healthcare and Medical Sciences | CT, Dermatology, Endoscopy, CFP, Histopathology, MRI, Microscopy, OCT, PET, US, X-ray, \etc | N/A | VQA | 2024.08 | EN | Comprehensive multi-source integration | Semi-automated | N/A | Data review | GPT-4o | 26k | MCQ | Acc |
| [SlideBench ](https://uni-medical.github.io/SlideChat.github.io) | Healthcare and Medical Sciences | Histopathology | N/A | VQA | 2024.11 | EN | Scientific databases | Semi-automated | N/A | Data generation and review | GPT-4o | 16k | MCQ, Open-ended | Acc, BLEU |
| [Bio-ML ](https://zenodo.org/records/13119437) | Healthcare and Medical Sciences | Ontology data | Expert | Text QA | 2024.07 | EN | Encyclopedias and knowledge bases | Semi-automated | N/A | Data generation and review | N/A | 25,270 | Retrieval | F1 |
| [MedBench ](https://medbench.opencompass.org.cn) | Healthcare and Medical Sciences | Dianosis report, Clinical dialogue, EHR | Expert | Text QA | 2024.06 | ZH | Integration of existing datasets | Manual | N/A | Data generation | N/A | 300,901 | MCQ, Open-ended | BLEU, ROUGE-L, F1, Acc |
| [ClinicalLab ](https://github.com/WeixiangYAN/ClinicalLab) | Healthcare and Medical Sciences | Clinical notes | Expert | Text QA | 2024.06 | EN, ZH | Other sources | Manual | N/A | Data generation and review | GPT-4 | 1,500 | Open-ended | DWR, DIFR, CDR, Acceptability, Acc, BLEU, ROUGE, BERTScore |
| [AgentClinic-NEJM ](https://agentclinic.github.io/) | Healthcare and Medical Sciences | Clinical dialog, Diagnosis report, CT, Dermatology, Histopathology, \etc | Expert | VQA | 2024.05 | EN | Academic and research resources, Comprehensive multi-source integration | Automated | N/A | N/A | N/A | 120 | Open-ended | Acc, Patient compliance, Consultation ratings |
| [AgentClinic-Lang ](https://agentclinic.github.io/) | Healthcare and Medical Sciences | Medical exams | Expert | Text QA | 2024.05 | EN, ES, FA, FR, HI, KO, ZH | Academic and research resources, Comprehensive multi-source integration | Semi-automated | N/A | Data review | GPT-4 | 749 | Open-ended | Acc, Patient compliance, Consultation ratings |
| [AgentClinic-MedQA ](https://agentclinic.github.io/) | Healthcare and Medical Sciences | Medical exams | Expert | Text QA | 2024.05 | EN | Academic and research resources, Comprehensive multi-source integration | Semi-automated | N/A | Data review | GPT-4 | 215 | Open-ended | Acc, Patient compliance, Consultation ratings |
| [AgentClinic-MIMIC-IV ](https://agentclinic.github.io/) | Healthcare and Medical Sciences | EHR | Expert | Text QA | 2024.05 | EN | Scientific databases | Semi-automated | N/A | Data review | GPT-4 | 200 | Open-ended | Acc, Patient compliance, Consultation ratings |
| [AgentClinic-Spec ](https://agentclinic.github.io/) | Healthcare and Medical Sciences | Medical exams | Expert | Text QA | 2024.05 | EN | Integration of existing datasets | Semi-automated | N/A | N/A | GPT-4 | 260 | Open-ended | Acc, Patient compliance, Consultation ratings |
| [M3D-Bench ](https://huggingface.co/datasets/GoodBaiBai88/M3D-Cap) | Healthcare and Medical Sciences | CT, Clinical reports | Expert | Image-text, Text QA, VQA | 2024.04 | EN | Scientific databases, Integration of existing datasets | Semi-automated | N/A | Data generation and review | GPT-4V | 1,235 | MCQ, Open-ended, Retrieval | Acc, BLEU, ROUGE |
| [AMOS-MM ](https://www.codabench.org/competitions/3137/) | Healthcare and Medical Sciences | CT | Expert | Image-text, VQA | 2024.04 | EN, ZH | Integration of existing datasets, Scientific databases | N/A | N/A | N/A | N/A | 2300 | Open-ended, MCQ | Acc |
| [CMtMedQA ](https://github.com/SupritYoung/Zhongjing) | Healthcare and Medical Sciences | Clinical dialogue | Expert | Text QA | 2024.03 | ZH | Books and literary works | Semi-automated | 6 | Data review | GPT-3.5, CMeKG, RLHF-Label-Tool | 70k | Open-ended | GPT-4 score |
| [Medbullets ](https://github.com/HanjieChen/ChallengeClinicalQA/tree/main) | Healthcare and Medical Sciences | Medical exams | N/A | Text QA | 2024.02 | EN | Social media and forums | Automated | N/A | Data review | N/A | 618 | MCQ | ROUGE-L, BERTScore, CTC, G-Eval, BARTScore+ |
| [RareBench ](https://huggingface.co/datasets/chenxz/RareBench) | Healthcare and Medical Sciences | EHR, Medical history, Lab tests | Expert | Text QA | 2024.02 | EN, ZH | Scientific databases, Academic and research resources, Other sources | Manual | N/A | Data generation and review | N/A | 2,185 | Open-ended | Precision, Recall, F1, Median Rank, \etc |
| [OmniMedVQA ](https://huggingface.co/datasets/foreverbeliever/OmniMedVQA) | Healthcare and Medical Sciences | CT, Dermatology, Endoscopy, CFP, Histopathology, MRI, Microscopy, OCT, PET, US, X-ray, \etc | N/A | VQA | 2024.02 | EN | Comprehensive multi-source integration | Semi-automated | N/A | Data review | GPT-4 | 127,995 | MCQ | Acc |
| [MultiMedEval ](https://github.com/corentin-ryr/MultiMedEval) | Healthcare and Medical Sciences | CT, Dermatology, CFP, Histopathology, MRI, Microscopy, OCT, US, X-ray, \etc | N/A | VQA | 2024.02 | EN | Integration of existing datasets | Semi-automated | N/A | Data review | CheXbert, GPT, RadGraph | 60k | MCQ | Acc |
| [Fhirfly Medical Questions ](https://huggingface.co/datasets/fhirfly/medicalquestions) | Healthcare and Medical Sciences | Biomedical QA | N/A | Text QA | 2024.01 | EN | Academic and research resources | Semi-automated | N/A | Data review | N/A | 25,102 | True/False | Acc |
| [RP3D-DiagDS ](https://huggingface.co/datasets/QiaoyuZheng/RP3D-DiagDS) | Healthcare and Medical Sciences | CT, MRI, X-ray, US, Fluoroscopy, \etc | Expert | Classification | 2023.12 | EN | Scientific databases | Semi-automated | N/A | Data generation and review | Custom crawlers, GPT-4 | 40,936 | True/False | AUROC, AP |
| [NEJM-AI Benchmarking ](https://huggingface.co/datasets/SeanWu25/NEJM-AI_Benchmarking_Medical_Language_Models) | Healthcare and Medical Sciences | Medical exams | Expert | Text QA | 2023.11 | EN | Academic and research resources | Automated | N/A | N/A | NLTK, Regex | 858 | MCQ | Acc, BLEU, WER, Cosine |
| [MORFITT ](https://huggingface.co/datasets/qanastek/MORFITT) | Healthcare and Medical Sciences | Clinical papers | Expert | Classification | 2023.11 | FR | Academic and research resources | Manual | N/A | Data review | N/A | 1,560 | Classification | Precision, Rappel, F1 |
| [SourceData ](https://huggingface.co/datasets/bigbio/sourcedata_nlp) | Healthcare and Medical Sciences | Gene/protein entities | Expert | Raw text | 2023.10 | EN | Academic and research resources | Manual | N/A | Data generation and review | N/A | 620,000 | NER | Precision, Recall, F1 |
| [SDOH-NLI ](https://huggingface.co/datasets/davanstrien/SDOH-NLI) | Healthcare and Medical Sciences | Clinical notes | Expert | Classification | 2023.10 | EN | Integration of existing datasets | Manual | N/A | Data generation | N/A | 4.21k | Classification | Precision, Recall, F1 |
| [HealthsearchQA ](https://huggingface.co/datasets/katielink/healthsearchqa) | Healthcare and Medical Sciences | Consumer health QA | Expert | Text QA | 2023.08 | EN | Web and Internet content | Semi-automated | N/A | Data review | N/A | 3,173 | Open-ended | Factuality, Comprehension, Reasoning, Possible harm and bias |
| [CMB-Exam ](https://huggingface.co/datasets/FreedomIntelligence/CMB) | Healthcare and Medical Sciences | Medical exams | Expert | Text QA | 2023.08 | ZH | Web and Internet content | Semi-automated | N/A | Data review | N/A | 280,839 | MCQ | Acc |
| [CMB-Clin ](https://huggingface.co/datasets/FreedomIntelligence/CMB) | Healthcare and Medical Sciences | Medical exams | Expert | Text QA | 2023.08 | ZH | Books and literary works | Semi-automated | N/A | Data review | N/A | 208 | Open-ended | Fluency, Relevance, Completeness, Proficiency |
| [MultiMedBench ](https://huggingface.co/datasets/liuhaotian/MultiMedBench) | Healthcare and Medical Sciences | CT, Dermatology, Histopathology, Microscopy, MRI, X-ray, \etc | N/A | Text QA, VQA | 2023.07 | Mixed | Integration of existing datasets | N/A | N/A | N/A | N/A | 1M | N/A | Acc, ROUGE-L, BLEU, F1-RadGraph, F1 |
| [GPT-4 BiasBenchmark ](https://github.com/elehman16/gpt4_bias) | Healthcare and Medical Sciences | Clinical trials | Expert | Text QA | 2023.07 | EN | Academic and research resources | Semi-automated | N/A | Data generation and review | GPT-4 | 213 | Open-ended | Acc |
| [Lavita Medical QA ](https://huggingface.co/datasets/lavita/medical-qa-shared-task-v1-all) | Healthcare and Medical Sciences | Clinical guidelines | N/A | Text QA | 2023.07 | EN | Academic and research resources | Automated | N/A | N/A | N/A | 11,500 | MCQ | Acc |
| [BioASQ10b-factoid ](https://huggingface.co/datasets/legacy107/bioasq10b-factoid) | Healthcare and Medical Sciences | Clinical dialogue, PubMed snippets | Expert | Text QA | 2023.07 | EN | Scientific databases, Academic and research resources | Manual | N/A | Data generation and review | N/A | 166 | Open-ended | Acc, MRR |
| [MedNERF ](https://huggingface.co/datasets/Posos/MedNERF) | Healthcare and Medical Sciences | Drug Prescription | Expert | Classification | 2023.06 | FR | Other sources | Manual | N/A | Data generation and review | N/A | 100 | NER | F1 |
| [WikiMedQA ](https://huggingface.co/datasets/sileod/wikimedqa) | Healthcare and Medical Sciences | Clinical reports | Expert | Text QA | 2023.03 | EN | Web and Internet content | Semi-automated | N/A | N/A | SentenceBERT, BioLinkBERT | 5,893 | MCQ | Acc |
| [BioASQ ](https://zenodo.org/records/7655130) | Healthcare and Medical Sciences | Biomedical Documents | Expert | Text QA | 2022.12 | EN | Academic and research resources | Manual | 21 | Data generation and review | N/A | 4,721 | Open-ended | Acc |
| [BioRED ](https://ftp.ncbi.nlm.nih.gov/pub/lu/BioRED/) | Healthcare and Medical Sciences | Biomedical papers | N/A | Classification | 2022.09 | EN | Scientific databases | Semi-automated | 6 | Data generation and review | PubTator | 100 | NER | Precision, Recall, F1 |
| [BioLeaflets ](https://huggingface.co/datasets/ruslan/bioleaflets-biomedical-ner) | Healthcare and Medical Sciences | Package leaflets | Expert | Raw text | 2021.09 | EN | Web and Internet content | Semi-automated | N/A | Data generation | Stanza, Amazon Comprehend Medical | 134 | Generation | SacreBLEU, ROUGE-L, BERTScore, BLEURT, MoverScore-21 |
| [CBLUE ](https://github.com/CBLUEbenchmark/CBLUE) | Healthcare and Medical Sciences | Clinical trials, EHR, Medical forum, Medical textbooks | N/A | Classification, Text QA | 2021.06 | ZH | Comprehensive multi-source integration | Manual | 3 | Data generation and review | N/A | 46,729 | NER, Open-ended, Retrieval | Acc, F1 |
| [SLAKE ](https://huggingface.co/datasets/BoKelvin/SLAKE) | Healthcare and Medical Sciences | CT, MRI, X-ray | N/A | VQA | 2021.02 | EN, ZH | Academic and research resources | Automated | N/A | N/A | N/A | 2,070 | MCQ, Open-ended | Acc |
| [MEDIQA-AnS ](https://doi.org/10.17605/OSF.IO/FYG46) | Healthcare and Medical Sciences | Consumer health QA | Undergraduate | Text QA | 2020.09 | EN | Web and Internet content | Manual | 2 | Data generation | N/A | 708 | Open-ended | ROUGE, BLEU |
| [RadVisDial (G) ](https://aclanthology.org/2020.bionlp-1.6.pdf) | Healthcare and Medical Sciences | X-ray | N/A | VQA | 2020.07 | EN | Integration of existing datasets | Semi-automated | 2 | Data generation | NegBio, CheXpert | 91k | MCQ | Acc |
| [CORD-19 ](https://github.com/allenai/cord19) | Healthcare and Medical Sciences | Academic papers | N/A | Text QA | 2020.03 | EN | Academic and research resources | N/A | N/A | N/A | N/A | 280K | Retrieval, QA | MRR, Acc |
| [PathVQA ](https://huggingface.co/datasets/flaviagiammarino/path-vqa) | Healthcare and Medical Sciences | Histopathology | Expert | VQA | 2020.03 | EN | Academic and research resources | Automated | N/A | N/A | CoreNLP | 6,012 | MCQ, Open-ended | BLEU, Exact-match, F1 |
| [MedQuAD ](https://github.com/abachaa/MedQuAD) | Healthcare and Medical Sciences | Patient educational materials | Undergraduate | Text QA | 2019.11 | EN | Web and Internet content | Semi-automated | 2 | Data generation | MetaMap Lite, UMLS lookup | 47,457 | Open-ended | Acc, F1, MRR |
| [Pubmed Causal ](https://huggingface.co/datasets/medalpaca/medical_meadow_pubmed_causal) | Healthcare and Medical Sciences | Biomedical papers | N/A | Classification | 2019.11 | EN | Scientific databases | Manual | N/A | Data generation | N/A | 2,446 | Classification | Acc, F1 |
| [PubMedQA instruction ](https://huggingface.co/datasets/fedml/PubMedQA_instruction) | Healthcare and Medical Sciences | Clinical dialogue | Expert | Text QA | 2019.09 | EN | Academic and research resources | Manual | N/A | Data generation | N/A | 273k | Classification | Acc |
| [VQA-RAD ](https://huggingface.co/datasets/flaviagiammarino/vqa-rad) | Healthcare and Medical Sciences | CT, MRI, PET, US, X-ray | N/A | VQA | 2018.11 | EN | Academic and research resources | Manual | N/A | Data generation | N/A | 451 | MCQ, Open-ended | Acc, BLEU |
| [Pima ](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database) | Healthcare and Medical Sciences | EHR | Expert | Classification | 1988.11 | EN | Scientific databases | Manual | N/A | N/A | N/A | 77 | Classification | AUROC |
| [TOMG-Bench ](https://huggingface.co/datasets/Duke-de-Artois/TOMG-Bench) | Molecular and Cellular Biology | Molecule | Expert | Text QA | 2024.12 | EN | Scientific databases | Automated | N/A | N/A | N/A | 45,000 | Open-ended | Success Rate, Similarity, Novelty, Validity |
| [MoleculeQA ](https://huggingface.co/datasets/hcaoaf/MoleculeQA) | Molecular and Cellular Biology | Molecule | Expert | Text QA | 2024.11 | EN | Scientific databases | Manual | 2 | Data generation and review | N/A | 62,000 | MCQ | Acc |
| [BEACON ](https://github.com/terry-r123/RNABenchmark) | Molecular and Cellular Biology | RNA sequence | N/A | Raw text | 2024.06 | EN | Comprehensive multi-source integration | Semi-automated | N/A | Data generation and review | N/A | 96,283 | Classification, Regression | F1, AUROC, Precision, R\textsuperscript{2}, MSE, PCC |
| [GeneHop ](https://huggingface.co/datasets/casey-martin/GeneGPT) | Molecular and Cellular Biology | Multi-hop genomic QA | N/A | Text QA | 2023.04 | EN | Academic and research resources | Manual | N/A | Data generation and review | N/A | 150 | Open-ended | Acc |
| [PCdes ](https://github.com/thunlp/KV-PLM) | Molecular and Cellular Biology | SMILES | N/A | Text QA | 2022.12 | EN | Academic and research resources | Automated | N/A | N/A | Custom crawlers | 3,000 | Retrieval | Acc, Recall |
| [PEER ](https://github.com/DeepGraphLearning/PEER_Benchmark) | Molecular and Cellular Biology | Protein sequence | Expert | Classification, Regression | 2022.10 | EN | Comprehensive multi-source integration | Semi-automated | N/A | Data generation and review | N/A | 115,281 | Classification, Regression | Acc, RMSE, Precision, PCC |
| [BioPreDyn-bench ](https://sites.google.com/site/biopredynbenchmarks/) | Molecular and Cellular Biology | Time-series (simulation data) | Expert | Regression | 2015.02 | EN | Academic and research resources | N/A | N/A | N/A | 6 | 6 | Open-ended | NRMSE |
| [MicroVQA ](https://jmhb0.github.io/microvqa/) | Molecular and Cellular Biology, Healthcare and Medical Sciences | Microscopy | Expert | VQA | 2025.03 | EN | Academic and research resources | Semi-automated | 12 | Data generation and review | GPT-4o | 1042 | MCQ | Acc |
| [DISEASES ](https://diseases.jensenlab.org/Downloads) | Molecular and Cellular Biology, Healthcare and Medical Sciences, Multi-omics | Disease-gene associations | Expert | Classification | 2015.01 | EN | Academic and research resources, Integration of existing datasets, Scientific databases | Semi-automated | N/A | Data generation and review | NER tagger | 8,336,442 | Open-ended, True/False, Retrieval | Precision, Recall, F1, AUROC, AUPRC |
| [LAB-Bench ](https://huggingface.co/datasets/futurehouse/lab-bench) | Molecular and Cellular Biology, Multi-omics, Neuroscience | Research problems | N/A | Text QA | 2024.07 | EN | Academic and research resources | N/A | N/A | N/A | N/A | 2,457 | MCQ | Acc |
| [BioProBench ](https://github.com/YuyangSunshine/bioprotocolbench) | Molecular and Cellular Biology, Multi-omics, Pharmacy, Neuroscience, \etc | Protocol | N/A | Text QA | 2025.05 | EN | Academic and research resources | Semi-automated | N/A | Data review | N/A | 556,171 | Open-ended | Acc, F1, EM, BLEU |
| [Genome-Bench ](https://huggingface.co/datasets/Mingyin0312/Genome-Bench) | Multi-omics | Research problems | N/A | Text QA | 2025.06 | EN | Academic and research resources | N/A | N/A | Data generation and review | GPT-4 Turbo, GPT-4o | 3,332 | MCQ | Acc |
| [GeneChat-test ](https://drive.google.com/drive/folders/1CM4jSkQkEUhyaofDR1KKDRD2vOPsWLG5) | Multi-omics | Nucleotide sequence | N/A | Text QA | 2025.06 | EN | Scientific databases | N/A | N/A | Data generation | N/A | N/A | Open-ended | BLUE, METEOR |
| [GeneChat ](https://drive.google.com/drive/folders/1CM4jSkQkEUhyaofDR1KKDRD2vOPsWLG5) | Multi-omics | Nucleotide sequence | N/A | Text QA | 2025.06 | EN | Scientific databases | N/A | N/A | Data generation | N/A | 2,973 | Open-ended | BLEU, METEOR |
| [Genomics instructions ](https://huggingface.co/InstaDeepAI/ChatNT) | Multi-omics | Nucleotide sequence | N/A | Text QA | 2025.04 | EN | Academic and research resources | N/A | N/A | Data generation | N/A | 403,814 | Classification, Regression | F1, MCC, AUROC, PCC |
| [BixBench ](https://huggingface.co/datasets/futurehouse/BixBench) | Multi-omics | Genomics transcriptomics text | Expert | Text QA | 2025.03 | EN | Academic and research resources | Semi-automated | Data generation and review | 53 | Claude 3.5 Sonnet | 296 | Open-ended, MCQ | Acc |
| [Seq2Func ](https://github.com/ML-Bioinfo-CEITEC/genomic_benchmarks) | Multi-omics | Nucleotide sequence | N/A | Text QA | 2025.02 | EN | Scientific databases | Automated | N/A | Data generation | N/A | 33,000 | MCQ | MCC, F1 |
| [DNA2Image ](https://github.com/ML-Bioinfo-CEITEC/genomic_benchmarks) | Multi-omics | Nucleotide sequence | N/A | Generation | 2025.02 | EN | Scientific databases | Automated | N/A | Data generation | N/A | 4,800 | Generation | Invalid percentage, F1 |
| [DNA Long Bench ](https://github.com/wenduocheng/DNALongBench) | Multi-omics | DNA sequence | N/A | Classification, Regression | 2025.01 | EN | Scientific databases; Academic and research resources | Automated | N/A | N/A | N/A | 213,416 | Classification, Regression | SCC, PCC, AUROC |
| [LLaMA-Gene (protein) ](https://huggingface.co/dnagpt/llama-gene-train-data) | Multi-omics | Protein sequence | N/A | Text QA | 2024.12 | EN | Scientific databases | N/A | N/A | Data generation | N/A | 6,991 | Open-ended | Acc |
| [LLaMA-Gene (DNA) ](https://huggingface.co/dnagpt/llama-gene-train-data) | Multi-omics | DNA sequence | N/A | Text QA | 2024.12 | EN | Scientific databases | N/A | N/A | Data generation | N/A | 19,839 | Open-ended | Acc |
| [NT Benchmark ](https://github.com/chamwen/NT-Benchmark) | Multi-omics | Nucleotide sequence | N/A | Classification | 2024.10 | EN | Academic and research resources | N/A | N/A | N/A | N/A | 38,822 | MCQ | MCC |
| [BioinformaticsBench ](https://openreview.net/forum?id=eKw7delVSM) | Multi-omics | Textbook | Undergraduate | Text QA | 2024.06 | EN | Books and literary works, Academic and research resources | Semi-automated | 4 | N/A | GPT-3.5, GPT-4, GPT-4 Turbo | 602 | MCQ, True/False, Open-ended | Acc |
| [genomics-long-range-benchmark ](https://huggingface.co/datasets/InstaDeepAI/genomics-long-range-benchmark) | Multi-omics | Nucleotide sequence | N/A | Classification, Regression | 2024.05 | EN | Academic and research resources | N/A | N/A | N/A | N/A | N/A | Classification, Regression | MCC |
| [RNA-QA ](https://rna-gpt.github.io/) | Multi-omics | RNA sequence | N/A | Text QA | 2024.05 | EN | Academic and research resources | Automated | N/A | N/A | N/A | 121 K | Open-ended | Precision, Recall, F1, ROUGE |
| [BioinfoBench ](https://github.com/cinnnna/bioinfo-bench) | Multi-omics | RNA sequence | Undergraduate | Text QA | 2023.10 | EN | Other sources | Semi-automated | N/A | Data review | ChatGPT | 200 | MCQ | Acc, Perplexity, Next-token likelihood |
| [BioCoder ](https://academic.oup.com/bioinformatics/article/40/Supplement_1/i266/7700865) | Multi-omics | Codes | Undergraduate | Text QA | 2023.08 | EN | Integration of existing datasets, Academic and research resources | Automated | N/A | N/A | N/A | 2522 | Open-ended | Acc |
| [SpeciesClassification ](https://github.com/HazyResearch/hyena-dna) | Multi-omics | Nucleotide sequence | N/A | Classification | 2023.06 | EN | Academic and research resources | N/A | N/A | N/A | N/A | 5 species genomes | MCQ | Acc |
| [GUE Benchmark ](https://github.com/MAGICS-LAB/DNABERT_2) | Multi-omics | Nucleotide sequence | N/A | Classification | 2023.06 | EN | Academic and research resources | N/A | N/A | N/A | N/A | 80,648 | MCQ | MCC, F1 |
| [Genomic Benchmark ](https://github.com/ML-Bioinfo-CEITEC/genomic_benchmarks) | Multi-omics | Nucleotide sequence | N/A | Classification | 2023.05 | EN | Academic and research resources | N/A | N/A | N/A | N/A | 191,589 | MCQ | Acc, F1 |
| [GeneTuring ](https://huggingface.co/datasets/vladimire/geneturing) | Multi-omics | Biomedical knowledge base | N/A | Text QA | 2023.03 | EN | Academic and research resources | N/A | N/A | Data generation | GPT-2, BioGPT, BioMedLM, GPT-3, ChatGPT, New Bing | 600 | MCQ | Acc |
| [Human Pancreas ](https://github.com/JackieHanLab/TOSICA) | Multi-omics | scRNA-seq | N/A | Classification | 2023.01 | EN | Academic and research resources | N/A | N/A | N/A | N/A | 4,218 | Classification | Acc, Precision, Recall, F1 |
| [Myeloid ](http://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE154763) | Multi-omics | scRNA-seq | N/A | Classification | 2021.02 | EN | Academic and research resources | N/A | N/A | N/A | N/A | 3,430 | Classification | Acc, Precision, Recall, F1 |
| [Human Cell Atlas Dataset ](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE159929) | Multi-omics | scRNA-seq | N/A | Classification | 2021.02 | EN | Academic and research resources | N/A | N/A | N/A | N/A | 84,363 | Classification | Acc, F1 |
| [Human enhancers Ensembl ](https://github.com/ML-Bioinfo-CEITEC/genomic_benchmarks/tree/main/datasets) | Multi-omics | Nucleotide sequence | N/A | Classification | 2021.01 | EN | Academic and research resources | N/A | N/A | N/A | N/A | 154,842 | MCQ | MCC |
| [Human regulatory Ensembl ](https://github.com/ML-Bioinfo-CEITEC/genomic_benchmarks/tree/main/datasets) | Multi-omics | Nucleotide sequence | N/A | Classification | 2021.01 | EN | Academic and research resources | N/A | N/A | N/A | N/A | 289,061 | MCQ | MCC |
| [Human ocr Ensembl ](https://github.com/ML-Bioinfo-CEITEC/genomic_benchmarks/tree/main/datasets) | Multi-omics | Nucleotide sequence | N/A | Classification | 2021.01 | EN | Academic and research resources | N/A | N/A | N/A | N/A | 174,756 | MCQ | MCC |
| [Multiple Sclerosis ](https://www.ebi.ac.uk/gxa/sc/experiments/E-HCAD-35) | Multi-omics | scRNA-seq | N/A | Classification | 2019.07 | EN | Academic and research resources | N/A | N/A | N/A | N/A | 13,468 | Classification | Acc, Precision, Recall, F1 |
| [APARENT ](https://github.com/johli/aparentAPARENT) | Multi-omics | Nucleotide sequence | N/A | Regression | 2019.06 | EN | Academic and research resources | N/A | N/A | N/A | N/A | 8,000 | Regression | R\textsuperscript{2} |
| [Human enhancers Cohn ](https://github.com/ML-Bioinfo-CEITEC/genomic_benchmarks/tree/main/datasets) | Multi-omics | Nucleotide sequence | N/A | Classification | 2018.02 | EN | Academic and research resources | N/A | N/A | N/A | N/A | 27,791 | MCQ | MCC |
| [Human non-TATA promoters ](https://github.com/ML-Bioinfo-CEITEC/genomic_benchmarks/tree/main/datasets) | Multi-omics | Nucleotide sequence | N/A | Classification | 2017.02 | EN | Academic and research resources | N/A | N/A | N/A | N/A | 36,131 | MCQ | MCC |
| [Zheng68k ](https://support.10xgenomics.com/single-cell-gene-expression/datasets) | Multi-omics | scRNA-seq | N/A | Classification | 2016.07 | EN | Academic and research resources | N/A | N/A | N/A | N/A | 68,450 | Classification | Acc, F1 |
| [Drosophila enhancers Stark ](https://github.com/ML-Bioinfo-CEITEC/genomic_benchmarks/tree/main/datasets) | Multi-omics | Nucleotide sequence | N/A | Classification | 2014.06 | EN | Academic and research resources | N/A | N/A | N/A | N/A | 6,914 | MCQ | MCC |
| [COMET ](https://arxiv.org/abs/2412.10347) | Multi-omics | DNA, RBA, Protein Sequence/Residue | N/A | Classification, Regression | 2024.12 | EN | Academic and research resources | N/A | N/A | N/A | N/A | 1.22M | Classification, Regression | R\textsuperscript{2}, PCC, F1, SCC |
| [AdaBrain-Bench ](https://github.com/Jamine-W/AdaBrain-Bench) | Neuroscience | EEG | N/A | Classification | 2025.07 | EN | Integration of existing datasets | N/A | N/A | N/A | N/A | N/A | Open-ended | Acc, AUROC, AUPRC, F1, PCC, R\textsuperscript{2} |
| [FDA Pharmaceuticals FAQ ](https://huggingface.co/datasets/Jaymax/FDA_Pharmaceuticals_FAQ) | Pharmacy | FAQ-style text | Expert | Text QA | 2023.03 | EN | Web and Internet content | Automated | N/A | N/A | N/A | 1,681 | MCQ | Acc |
| [repoDB ](https://unmtid-shinyapps.net/shiny/repodb/) | Pharmacy, Healthcare and Medical Sciences | Drug-disease relationships, Clinical trial outcomes | Expert | Classification, Text QA | 2017.03 | EN | Scientific databases | Automated | N/A | N/A | scripts | 15,648 | MCQ, Retrieval | AUROC, AUPRC, Acc |
| [MedMax Eval ](https://huggingface.co/datasets/mint-medmax/medmax_eval_data) | Standardization of several biomedical evaluation sets | Radiology, Histopathology | Expert | VQA, Visual Chat, Interleaved Vision-Language Data, Image Generation, and Captioning | 2024.12 | EN | Academic and research resources | Automated | N/A | N/A | GPT-4, BioMedCLIP, Rule-based | 9,500 | Open-Ended, Close-Ended | Acc, CLIPScore |

</details>

<details>
<summary>

### ⚗️ Chemistry

</summary>

 <a href="#-table-of-contents" style="float:right;">⬆ Back to Top</a>
| Dataset | Domain | Modality | Level | Type | Release | Language | Source | Annotation Pipeline | Human Annotators | Human Tasks | Auto-annotation Tools | Size | Evaluation Type | Metrics |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| [OmniGenBench ](https://github.com/yangheng95/OmniGenBench) | Biochemistry, Multi-omics | DNA sequence, RNA sequence, TF binding, \etc | N/A | Classification | 2025.05 | N/A | Integration of existing datasets, Academic and research resources | N/A | N/A | N/A | N/A | N/A | N/A | AUROC, F1, RMSE, R\textsuperscript{2} |
| [MOSES ](https://tdcommons.ai/generation_tasks/molgen/) | Biochemistry | SMILES | Expert | Raw text | 2020.07 | EN | Academic and research resources | Manual | N/A | Data review | N/A | 1,936,962 | Generation | Chemical validity, Drug-likeness |
| [ChEMBL ](https://www.ebi.ac.uk/chembl/) | Biochemistry | SMILES | Expert | Raw text | 2012.01 | EN | Academic and research resources | Manual | N/A | Data generation and review | N/A | 1.96M | Generation | Chemical validity, Drug-likeness |
| [ChemRxivQuest ](https://arxiv.org/pdf/2505.05232) | General Chemistry | Academic papers | Expert | Text QA | 2025.05 | EN | Academic and research resources | Manual | N/A | Data generation and review | NA | 970 | Open-ended | Acc |
| [ScholarChemQA ](https://github.com/iriscxy/chemmatch) | General Chemistry | Academic papers | Expert | Text QA | 2025.02 | EN | Academic and research resources | Manual | N/A | Data generation and review | N/A | 40K | MCQ | Acc |
| ChemSafetyBench | General Chemistry | Text | Expert | Raw text | 2024.11 | EN | Academic and research resources | Automated | N/A | Data generation and review | NA | 30K+ | Open-ended | Acc, Recall, Precision, F1, safety/quality score, \etc |
| ChemEval | General Chemistry | Text | Expert | Raw text | 2024.09 | EN | Academic and research resources | Automated | N/A | Data generation and review | NA | unknown (42 tasks) | Open-ended | Acc, BLEU-2, F1, \etc |
| [ChemNLP ](https://huggingface.co/datasets/lavita/medical-qa-shared-task-v1-all) | General Chemistry | Text | Secondary school | Text QA | 2023.01 | EN | Academic and research resources | Manual | N/A | Data generation and review | N/A | 27.6K | Classification, NER, Generation | Acc, ROUGE |
| [ZINC ](https://zinc.docking.org/) | General Chemistry | SMILES | Expert | Raw text | 2012.10 | EN | Academic and research resources | Manual | N/A | Data review | N/A | 250K | Generation | Chemical validity, Drug-likeness |
| [PMO ](https://github.com/wenhao-gao/mol_opt) | General Chemistry | SMILES | Expert | Raw text | 2022.05 | EN | Academic and research resources | Automated | N/A | Data generation and review | N/A | 10K | Open-ended | target property, Chemical validity, Drug-likeness |
| [DeepProtein ](https://github.com/jiaqingxie/DeepProtein) | Pharmacy | Protein sequence, SMILES | Expert | Raw text | 2025.05 | EN | Academic and research resources | Automated | N/A | Data generation and review | N/A | 78K | Classification, Regression | Acc, MAE, F1, AUPRC, AUROC, R\textsuperscript{2}, \etc |
| [TrialBench ](https://huyjj.github.io/Trialbench/) | Pharmacy | SMILES, Disease code | Expert | Raw text | 2024.09 | EN | Academic and research resources | Automated | N/A | Data generation and review | N/A | 470K | Open-ended | F1, Recall, Precision, MSE, \etc |
| [TDC2 ](https://tdcommons.ai/) | Pharmacy | SMILES, Protein sequence, Genome sequence | Expert | Raw text | 2024.09 | EN | Academic and research resources | Manual | N/A | Data generation and review | NA | 3.4B tokens | Open-ended | F1, Recall, Precision, MSE, \etc |
| [PCQM4Mv2 ](https://ogb.stanford.edu/docs/lsc/pcqm4mv2/#dataset) | Pharmacy | Molecular graph | N/A | Regression | 2022.11 | EN | Academic and research resources | Automated | N/A | N/A | N/A | 3,746,619 | Regression | MAE |
| [SBDDBench ](https://github.com/futianfan/reinforced-genetic-algorithm) | Pharmacy | Protein sequence, SMILES | Expert | Protein-ligand | 2022.06 | EN | Academic and research resources | Automated | N/A | Data generation and review | N/A | 5K | Open-ended | binding affinity, Chemical validity, Drug-likeness |
| [GEOM ](https://github.com/learningmatter-mit/geom) | Pharmacy | 3D conformation | N/A | Regression | 2022.04 | EN | Academic and research resources | Automated | N/A | N/A | CREST (GFN2-xTB) | 37M conformations | Regression | MAE, RMSD |
| [TOP ](https://github.com/futianfan/HINT) | Pharmacy | SMILES | Expert | Raw text | 2022.02 | EN | Academic and research resources | Automated | N/A | Data generation and review | N/A | 12K | Open-ended | F1, Recall, AUPRC, \etc |
| [TDC ](https://tdcommons.ai/) | Pharmacy | SMILES, Protein sequence, Genome sequence | Expert | Raw text | 2021.06 | EN | Academic and research resources | Manual | N/A | Data generation and review | NA | 0.2B tokens | Open-ended | F1, Recall, Precision, MSE, \etc |
| [DeepPurpose ](https://github.com/kexinhuang12345/DeepPurpose) | Pharmacy | Protein sequence, SMILES | Expert | Raw text | 2020.12 | EN | Academic and research resources | Automated | N/A | Data generation and review | N/A | 5,074 | Classification, Regression | MSE, PCC, F1, AUROC, AUPRC, \etc |
| [DrugBank ](https://go.drugbank.com/) | Pharmacy | SMILES | Expert | Raw text | 2018.01 | EN | Academic and research resources | Manual | N/A | Data generation and review | N/A | 17.47K | Open-ended | Acc |
| USPTO | Synthetic Chemistry | SMILES | Expert | Raw text | 2015.07 | EN | Patent databases | Manual | N/A | Data generation and review | NA | 1,939,253 | Open-ended | Acc, F1, MSE, \etc |

</details>

<details>
<summary>

### ⚛️ Physics

</summary>

 <a href="#-table-of-contents" style="float:right;">⬆ Back to Top</a>
| Dataset | Domain | Modality | Level | Type | Release | Language | Source | Annotation Pipeline | Human Annotators | Human Tasks | Auto-annotation Tools | Size | Evaluation Type | Metrics |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| [FSReD ](https://github.com/SJ001/AI-Feynman) | General Physics | Text | Expert | Text QA | 2019.05 | EN | Comprehensive multi-source integration | Automated | N/A | Data review | N/A | 120 | Regression | MSE, Exact Match |
| [PIQA ](https://yonatanbisk.com/piqa/) | General Physics | Text | Primary school | Text QA | 2020.01 | EN | Other sources | Semi-automated | N/A | Data generation and review | N/A | 2,000 | MCQ | Acc |
| [SRBench ](https://github.com/cavalab/srbench) | General Physics | Text | N/A | Text QA | 2021.07 | EN | Comprehensive multi-source integration | Semi-automated | N/A | Data generation and review | N/A | 252 | Open-ended | Acc, Simplicity, Exact Match |
| [PROST ](https://huggingface.co/datasets/corypaik/prost) | General Physics | Text | N/A | Text QA | 2021.08 | EN | Other sources | Semi-automated | 4 | Data generation | N/A | 18,736 | MCQ | Acc |
| [MM-PhyQA ](https://arxiv.org/pdf/2404.08704) | Kinematics, Mechanics, Electrostatics and Current Electricity, Thermodynamics, Optics, Magnetism, \etc | Text | High school | VQA with CoT | 2024.04 | EN | Comprehensive multi-source integration | Semi-automated | 8+ | Data generation and review | ChatGPT | 675 | MCQ | Acc, ROUGE |
| [MVBench ](https://huggingface.co/datasets/OpenGVLab/MVBench) | General Physics | Video | N/A | Video QA | 2024.05 | EN | Comprehensive multi-source integration | Automated | 0 | Data review | N/A | 4,000 | MCQ | Acc |
| [UGPhysics ](https://github.com/YangLabHKUST/UGPhysics) | Mechanics, Thermodynamics, Electromagnetism, Modern Physics | Text (problem statements, equations, reasoning) | Undergraduate | Text QA | 2025.01 | EN, ZH | Academic and research resources | Semi-automated | N/A | Data generation and review | GPT-4o | 11,040 | MCQ, Open-ended, True/False, Retrieval | Acc |
| [PhysReason ](https://huggingface.co/datasets/zhibei1204/PhysReason) | Mechanics, Electromagnetism, Thermodynamics, \etc | Text (problem statements, equations), Diagrams (physics illustrations) | Undergraduate, Graduate, Expert | Text QA, VQA | 2025.02 | EN | Comprehensive multi-source integration | Semi-automated | 4 | Data generation and review | GPT-4 | 1,200 | MCQ | Acc |
| [TPBench ](https://tpbench.org/) | Cosmology, High Energy Theory, General Relativity, Astrophysics, Electromagnetism, Quantum Mechanics, Mechanics, \etc | Text | N/A | Text QA | 2025.02 | N/A | Other sources | Manual | N/A | Data generation and review | N/A | 57 | Open-ended | Acc, AI-based Holistic Grading |
| [PHYSICS ](https://github.com/yale-nlp/Physics) | Mechanics, Electromagnetism, Thermodynamics, Optics, \etc | Text (problem statements, equations, reasoning), Diagrams (illustrations, charts, experimental setups) | Undergraduate | Text QA, VQA | 2025.03 | EN | Comprehensive multi-source integration | Manual | N/A | Data generation and review | N/A | 1,297 | Open-ended | Acc |
| [PhysicsArena ](https://arxiv.org/pdf/2505.15472) | Mechanics, Electromagnetism, Thermodynamics, \etc | Text (problem statements, equations, reasoning), Diagrams (illustrations, charts, experimental setups) | Expert | Text QA, VQA | 2025.05 | EN | Comprehensive multi-source integration | Semi-automated | N/A | Data generation and review | N/A | 5,100 | Open-ended | Acc |
| [PHYBench ](https://phybench-official.github.io/phybench-demo/) | Mechanics, Electricity, Thermodynamics, Optics, Modern Physics, \etc | Research problems | Undergraduate | Text QA | 2025.05 | EN | Comprehensive multi-source integration | Semi-automated | 178 | Data generation and review | o1, DeepSeek-R1 | 500 | Open-ended | EED |
| [PhyX ](https://phyx-bench.github.io/) | Mechanics, Quantum Mechanics, Thermodynamics, Electromagnetism, Atomic Physics, \etc | Text (problem statements, equations, reasoning), Diagrams (illustrations, charts, experimental setups) | Undergraduate | Text QA, VQA | 2025.05 | EN | Comprehensive multi-source integration | Semi-automated | N/A | Data generation and review | GPT-4o | 3,000 | MCQ, Open-ended | Acc |
| [PhysUniBench ](https://prismax-team.github.io/PhysUniBenchmark/) | Mechanics, Electromagnetism, Optics, Atomic Physics, \etc | Text (problem statements, equations), Diagrams (physics illustrations) | Undergraduate | VQA | 2025.06 | EN, ZH | Comprehensive multi-source integration | Manual | N/A | Data generation and review | N/A | 3,304 | Open-ended, MCQ | Acc |
| [IntPhys 2 ](https://github.com/facebookresearch/IntPhys2) | General Physics | Video, Text (scene parameters, object categories, trajectories, physical attributes) | N/A | Video QA | 2025.06 | N/A | Other sources | Semi-automated | N/A | Data generation and review | N/A | 1,400 | Open-ended | Acc |
| [MVP-Bench ](https://huggingface.co/datasets/GZClarence/MVP-Bench) | General Physics | Video | N/A | Video QA | 2025.06 | EN | Encyclopedias and knowledge bases | Semi-automated | N/A | Data generation and review | OpenAI CLIP (ViT-L/14) | 55,000 | Open-ended | Acc |
| [SeePhys ](https://github.com/AI4Phys/SeePhys) | Mechanics, Electromagnetism, Particle Physics, Optics=, Astrophysics, Thermodynamics, Quantum Mechanics, \etc | Text (problem statements, equations), Diagrams (physics illustrations) | Secondary school, Undergraduate, Graduate | VQA | 2025.07 | EN,ZH | Comprehensive multi-source integration | Semi-automated | N/A | Data generation and review | GPT-4o | 2,000 | Open-ended | Acc |

</details>

<details>
<summary>

### 🌌 Astronomy

</summary>

 <a href="#-table-of-contents" style="float:right;">⬆ Back to Top</a>
| Dataset | Domain | Modality | Level | Type | Release | Language | Source | Annotation Pipeline | Human Annotators | Human Tasks | Auto-annotation Tools | Size | Evaluation Type | Metrics |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| [Astro-QA ](https://github.com/ACMISLab/Astro-QA) | Astronomy | Astronomy Olympiad competitions, Astronomy exams, Online encyclopedias | Undergraduate | Text QA | 2025.06 | Mixed | Comprehensive multi-source integration | Manual | 30+ | Data generation and review | N/A | 3,082 | Open-ended | DGscore, BLEU, ROUGE, chrF |
| [Astrovisbench ](https://github.com/UniverseTBD/AstroLLaVA) | Astronomy | Galaxy images | Expert | VQA | 2025.06 | EN | Comprehensive multi-source integration | Semi-automated | 6 | Data review | GPT-4o, Claude 3.5 Sonnet | 432 | Open-ended | VIscore, Image error level, Expert evaluation |
| [AstroMLab 1 ](https://huggingface.co/datasets/AstroMLab/Astrobench_MCQ_v1_Public) | Astronomy | Academic papers | Expert | Text QA | 2024.11 | EN | Academic and research resources | Automated | N/A | Data review | Gemini-1.5-Pro | 4,425 | MCQ | Acc |
| [AstroPT ](https://www.github.com/Smith42/astroPT) | Astronomy | Astronomical images | Expert | Image-text | 2024.05 | EN | Web and Internet content, Scientific databases | Automated | N/A | Data review | DESI Legacy Survey API | 8.6 M | Classification | PCC, Acc |
| [Astro-NER ](https://arxiv.org/pdf/2405.02602?) | Astronomy | Academic papers | Expert | Text QA | 2024.05 | EN | Academic and research resources | Semi-automated | 4 | Data generation and review | GPT-3.5 | 5,000 | Open-ended | Precision, Recall, F1 |
| [AstroLLaMA ](https://huggingface.co/UniverseTBD/astrollama) | Astronomy | Academic papers | Expert | Text QA | 2023.09 | EN | Academic and research resources,Web and Internet content | Manual | N/A | Data review | N/A | 9.5 M | Open-ended | Perplexity, Cosine similarity |
| [ATel ](https://github.com/JetBrains/lm-astronomy) | Astronomy | Academic papers | Expert | Text QA | 2023.05 | EN | Academic and research resources | Manual | N/A | Data review | N/A | 234 | Open-ended | Acc |
| [PhyE2Es ](https://github.com/Jie0618/PhysicsRegression) | Astrophysics | Text with formulae | Expert | Raw text | 2025.03 | EN | Scientific databases | Automated | N/A | Data generation and review | OpenLLAMA-2-3B | 8,000 | Regression | Acc, Numerical precision, Formula complexity, Formula depth |
| [Pathfinder Dataset ](https://www.github.com/smsharma/PAPERCLIP-Hubble) | Astrophysics | Academic papers, ADS | Expert | Text QA with CoT | 2024.11 | EN | Web and Internet content, Academic and research resources | Automated | 36+ | Data generation and review | text-embedding-3-small | 385,166 | Open-ended | Acc, MRR, Recall, NDCG, relevance score |
| [Starwhisper-pilsar ](https://github.com/ACMISLab/StarWhisper-Pulsar) | Astrophysics | Pulsar diagnostic plots, Pulsars signals | Expert | VQA | 2024.04 | EN | Integration of existing datasets | Manual | N/A | Data generation and review | DeepSeek-VL-7B, InternVL2-40B | 106,674 | Open-ended | Acc, Recall, Precision, F1, \etc |
| [PAPERCLIP ](https://www.github.com/smsharma/PAPERCLIP-Hubble) | Astrophysics | Synthetic conversation, Astronomical images | Expert | Text QA | 2024.03 | EN | Academic and research resources,Scientific databases | Automated | N/A | Data generation and review | Mixtral-8x7B-Instruct | 31,859 | Open-ended | Acc |

</details>

<details>
<summary>

### 🪨 Materials Science

</summary>

 <a href="#-table-of-contents" style="float:right;">⬆ Back to Top</a>
| Dataset | Domain | Modality | Level | Type | Release | Language | Source | Annotation Pipeline | Human Annotators | Human Tasks | Auto-annotation Tools | Size | Evaluation Type | Metrics |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| [CheMatAgent ](https://github.com/AI4Chem/ChemistryAgent) | Materials Science | Scientific instruction | Expert | Text QA | 2025.06 | EN | Other sources | Manual | N/A | Data generation and review | N/A | 137 | Open-ended | Acc |
| [ChEBI-20-MM ](https://huggingface.co/datasets/liupf/ChEBI-20-MM) | Materials Science | InChI, IUPAC, SELFIES, Science QA, Molecular Image | Expert | Text QA | 2025.01 | EN | Integration of existing datasets | Manual | N/A | Data generation and review | N/A | 3,300 | Open-ended | BLEU, ROUGE, METEOR, CIDEr |
| [LLM4MatBench ](https://github.com/vertaix/LLM4Mat-Bench) | Materials Science | CIF, Chemical composition, Numerical property | Expert | Text QA | 2024.10 | EN | Scientific databases | Manual | N/A | Data generation and review | N/A | 1.9M | Open-ended | Acc |
| [MatText ](https://github.com/lamalab-org/MatText) | Materials Science | Chemical composition, Numerical property | Expert | Text QA | 2024.08 | EN | Scientific databases | Manual | N/A | Data generation and review | N/A | 2,000,000 | Open-ended | MAE, AUROC |
| [MatBookQA ](https://openreview.net/forum?id=ZUkmRy6SqS) | Materials Science | Science QA | Expert | Text QA | 2024.05 | EN | Academic and research resources | Manual | N/A | Data generation and review | N/A | 650 | Open-ended | Acc |
| [MaSCQA ](https://github.com/M3RG-IITD/MaScQA) | Materials Science | Science QA | Expert | Text QA | 2023.08 | EN | Academic and research resources | Manual | N/A | Data generation and review | N/A | 650 | Open-ended | Acc |
| [MatSci-NLP ](https://github.com/BangLab-UdeM-Mila/NLP4MatSci-ACL23) | Materials Science | Chemical composition, Numerical property | Expert | Text QA | 2023.05 | EN | Academic and research resources | Manual | N/A | Data generation and review | N/A | 169,197 | Open-ended | Acc, F1 |
| [ChEBI-20 ](https://github.com/cnedwards/text2mol) | Materials Science | Scientific instruction | Expert | Text QA | 2021.11 | EN | Integration of existing datasets | Manual | N/A | Data generation and review | N/A | 3,301 | Open-ended | BLEU, ROUGE, METEOR, CIDEr |
| [MOSES ](https://github.com/molecularsets/moses) | Materials Science | SMILES | Expert | Text QA | 2020.11 | EN | Integration of existing datasets | Manual | N/A | Data generation and review | N/A | 176,000 | Open-ended | Uniqueness, Validity, Frag, Scaff, SNN |
| [MatBench ](https://matbench.materialsproject.org/) | Materials Science | CIF, Numerical property, Chemical composition | Expert | Text QA | 2020.09 | EN | Scientific databases | Manual | N/A | Data generation and review | N/A | 408,062 | Open-ended | MAE, AUROC |
| [GuacaMol ](https://github.com/BenevolentAI/guacamol) | Materials Science | SMILES | Expert | Text QA | 2019.03 | EN | Integration of existing datasets | Manual | N/A | Data generation and review | N/A | 2M | Open-ended | Validity, Uniqueness, Novelty |
| [MoleculeNet ](https://moleculenet.org/) | Materials Science | SMILES | Expert | Text QA | 2017.03 | EN | Integration of existing datasets | Manual | N/A | Data generation and review | N/A | 700,000 | Open-ended | AUROC, AUPRC, RMSE, MAE |
| [MaCBench ](https://huggingface.co/datasets/jablonkagroup/MaCBench) | Materials Science, Chemistry | Science QA, AFM Image | Expert | VQA | 2024.11 | EN | Academic and research resources | Manual | N/A | Data generation and review | N/A | 628 | Open-ended | Acc |
| [MMSci ](https://mmsci.s3.amazonaws.com/benchmark.zip) | Materials Science, Chemistry | Science QA | Graduate | VQA | 2024.05 | EN | Academic and research resources | Manual | N/A | Data generation and review | N/A | 742,273 | Open-ended | Acc |

</details>

<details>
<summary>

### 🌍 Earth Science

</summary>

 <a href="#-table-of-contents" style="float:right;">⬆ Back to Top</a>
| Dataset | Domain | Modality | Level | Type | Release | Language | Source | Annotation Pipeline | Human Annotators | Human Tasks | Auto-annotation Tools | Size | Evaluation Type | Metrics |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| [ClimaQA ](https://huggingface.co/datasets/UCSD-GENIE/ClimaQA) | Atmosphere | Textbooks | Expert | Text QA | 2025.03 | EN | Books and literary works | Semi-automated |  | Data review | GPT-4o | 3,633 | MCQ, Open-ended | Acc, BLEU, \etc |
| [WeatherQA ](https://huggingface.co/datasets/ZhanxiangHua/WeatherQA_SFT) | Atmosphere | Remote sensing, Science QA | Expert | VQA (multi-image) | 2024.06 | EN | Scientific databases | Semi-automated | 4 | Data review |  | 600 | MCQ, Open-ended | Acc, F1, BLEU, \etc |
| [ClimateBERT ](https://huggingface.co/datasets/climatebert/climate_sentiment) | Atmosphere | Corporate annual reports, Sustainability reports | Secondary school | Text QA | 2022.12 | EN | Web and Internet content | Manual | 4+ | Data review | Prodigy | 320 | MCQ | Acc |
| [OceanBench ](https://huggingface.co/datasets/zjunlp/OceanBench) | Hydrosphere | Academic papers | Expert | Text QA | 2024.09 | EN | Academic and research resources | Automated | 10+ | Data review | GPT-4, GPT-3.5 | 13,000 | Open-ended | Win Rate |
| [OmniEarth-Bench ](https://huggingface.co/datasets/initiacms/OmniEarth-Bench) | Hydrosphere, Biosphere, Lithosphere, Atmosphere, Cryosphere | Remote sensing, Science QA | Expert | VQA with CoT (multi-image) | 2025.05 | EN | Integration of existing datasets | Manual | 40+ | Data generation and review |  | 29,779 | MCQ | Acc, Precision, Recall, F1 |
| [MSEarth ](https://huggingface.co/MSEarth) | Hydrosphere, Biosphere, Lithosphere, Atmosphere, Cryosphere | Academic papers | Expert | VQA with CoT | 2025.05 | EN | Academic and research resources | Semi-automated | 20+ | Data review | GPT-4o | 11,500 | MCQ, Open-ended | BLEU, BERTScore, Acc |
| [EarthSE ](https://huggingface.co/ai-earth) | Hydrosphere, Biosphere, Lithosphere, Atmosphere, Cryosphere | Academic papers | Expert | Text QA with CoT | 2025.05 | EN | Academic and research resources | Semi-automated | 20+ | Data review | GPT-4o | 10,000 | Open-ended | Acc |
| [GeoBench ](https://huggingface.co/datasets/daven3/geobench) | Lithosphere | Science QA | Expert | Text QA | 2023.06 | EN | Web and Internet content, Academic and research resources | Semi-automated | 10+ | Data review |  | 2,516 | MCQ, Open-ended | Acc, GPTScore |
| [XLRS-Bench ](https://github.com/AI9Stars/XLRS-Bench) | Remote Sensing | Remote sensing | N/A | Image-text, VQA | 2025.03 | EN, ZH | Academic and research resources | Semi-automated | 55 | Data generation and review | GPT-4o | 32,389 | MCQ, Open-ended | Acc, IoU, BLEU, \etc |
| [LRS-VQA ](https://github.com/VisionXLab/LRS-VQA) | Remote Sensing | Remote sensing | N/A | Image-text, VQA | 2025.03 | EN | Academic and research resources | Automated | N/A | N/A | Qwen2-VL, GPT-4V | 7,333 | Open-ended | Acc |
| [MME-RealWorld-RS ](https://github.com/MME-Benchmarks/MME-RealWorld) | Remote Sensing | Remote sensing | N/A | Image-text, VQA | 2024.08 | EN, ZH | Academic and research resources | Manual | N/A | Data generation and review | N/A | 3,738 | MCQ | Acc |
| [VRSBench ](https://github.com/lx709/VRSBench) | Remote Sensing | Remote sensing | N/A | Image-text, VQA | 2024.06 | EN | Academic and research resources | Semi-automated | N/A | Data review | GPT-4V | 62,917 | Open-ended | Acc, IoU, BLEU, \etc |
| [GeoChat ](https://github.com/mbzuai-oryx/GeoChat) | Remote Sensing | Remote sensing | N/A | Image-text, VQA | 2023.11 | EN | Academic and research resources, Integration of existing datasets | Automated | N/A | N/A | Vicuna | 10K | Open-ended | Acc, IoU, METEOR |
| [RSIEval ](https://github.com/Lavender105/RSGPT) | Remote Sensing | Remote sensing | N/A | Image-text, VQA | 2023.07 | EN | Academic and research resources | Manual | 5 | Data generation and review | N/A | 1,036 | Open-ended | Acc, BLEU, ROUGE, \etc |
| [DIOR-RSVG ](https://github.com/ZhanYang-nwpu/RSVG-pytorch) | Remote Sensing | Remote sensing | N/A | Image-text | 2022.10 | EN | Academic and research resources | Semi-automated | N/A | Data review | N/A | 17,402 | Open-ended | IoU |
| [NWPU-Captions ](https://github.com/HaiyanHuang98/NWPU-Captions) | Remote Sensing | Remote sensing | N/A | Image-text | 2022.08 | EN | Academic and research resources | Manual | N/A | Data generation | N/A | 31,500 | Open-ended | BLEU, METEOR, \etc |
| [RSVQA-HRBEN ](https://rsvqa.sylvainlobry.com/) | Remote Sensing | Remote sensing | N/A | Image-text, VQA | 2020.05 | EN | Scientific databases | Automated | N/A | N/A | N/A | 77,232 | Open-ended | Acc |
| [RSVQA-LRBEN ](https://rsvqa.sylvainlobry.com/) | Remote Sensing | Remote sensing | N/A | Image-text, VQA | 2020.05 | EN | Scientific databases | Automated | N/A | N/A | N/A | 1,066,316 | Open-ended | Acc |
| [RSICD ](https://github.com/201528014227051/RSICD_optimal) | Remote Sensing | Remote sensing | N/A | Image-text | 2017.12 | EN | Academic and research resources | Manual | N/A | Data generation | N/A | 10,921 | Open-ended | BLEU, METEOR, CIDEr |
| [UCM-Captions ](https://github.com/201528014227051/RSICD_optimal) | Remote Sensing | Remote sensing | N/A | Image-text | 2016.07 | EN | Academic and research resources | Manual | N/A | Data generation | N/A | 2,100 | Open-ended | BLEU, METEOR, CIDEr |
| [Sydney-Captions ](https://github.com/201528014227051/RSICD_optimal) | Remote Sensing | Remote sensing | N/A | Image-text | 2016.07 | EN | Academic and research resources | Manual | N/A | Data generation | N/A | 613 | Open-ended | BLEU, METEOR, CIDEr |

</details>

<details>
<summary>

### 🔭 General Science 

</summary>

 <a href="#-table-of-contents" style="float:right;">⬆ Back to Top</a>
| Dataset | cScientific Domain | Modality | Type | Release | Language | Source | Annotation Pipeline | Human Annotators | Human Tasks | Auto-annotation Tools | Size | Level | Evaluation Type | Metrics |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| [MMMU ](https://huggingface.co/datasets/MMMU/MMMU) | Science (Biology, Chemistry, Geography, Math, Physics), Health & Medicine (Basic Medical Science, Clinical Medicine, Diagnostics, Pharmacy, Public Health), Tech & Engineering (Materials, \etc) | Scientific VQA, MRI, CT, X-ray, \etc | VQA | 2023.11 | EN | Comprehensive multi-source inte- gration | Semi-automatic | 50 | Data review | Claude, GPT-4, GPT-4V | 11,550 | Expert | MCQ | Acc |
| [MMMU Pro ](https://huggingface.co/datasets/MMMU/MMMU_Pro) | Science (Biology, Chemistry, Geography, Math, Physics), Health & Medicine (Basic Medical Science, Clinical Medicine, Diagnostics, Pharmacy, Public Health), Tech & Engineering (Materials, \etc) | Scientific VQA, MRI, CT, X-ray, \etc | VQA | 2023.11 | EN | Comprehensive multi-source integration | Semi-automatic | N/A | Data review | Claude, GPT-4, GPT-4V | 5,190 | Expert | MCQ | Acc |
| [ScienceQA ](https://github.com/lupantech/ScienceQA) | Biology, Earth Science, Physics, Chemistry, Geography | Scientific query, Scientific instruction, Science textbooks and literature | VQA | 2022.01 | EN | Books and literary works | Manual | 9+ | Data generation and review | ViT, GPT-2 | 21.2k | Primary school, Secondary school | MCQ | Acc |
| [SciQA ](https://huggingface.co/datasets/orkg/SciQA) | Material Science, Chemistry, Life sciences | Scientific query | Text QA | 2023.05 | EN | Academic and research resources | Manual | N/A | Data generation and review | N/A | 2,565 | Expert | Open-ended | Acc |
| [Scicode ](https://github.com/scicode-bench/SciCode) | Material Science, Biology, Chemistry, Physics, Mathematics | Scientific Instruction | Text QA | 2024.08 | EN | Academic and research resources | Manual | N/A | Data generation and review | N/A | 338 | Expert | Open-ended | pass@1 |
| [CURIE ](https://huggingface.co/datasets/nhop/curie) | Materials Science, Life Sciences, Physics, Earth Science | Scientific query | VQA | 2025.04 | EN | Integration of existing datasets | Manual | N/A | Data generation and review | N/A | 580 | Expert | Open-ended | Acc |
| [TheoremQA ](https://github.com/wenhuchen/TheoremQA) | Physics, Mathematics | Theorems | Text QA | 2023.12 | EN | Books and literary works, Encyclopedias and knowledge bases | Manual | N/A | Data generation and review | N/A | 800 | Undergraduate, Expert | Open-ended | Acc |
| [SciBench ](https://github.com/mandyyyyii/scibench) | Physics, Chemistry | Science QA | Text QA | 2023.09 | EN | Books and literary works | Manual | 7 | Data review | N/A | 695 | Undergraduate | Open-ended | Acc |
| [JEEBench ](https://github.com/dair-iitd/jeebench) | Physics, Chemistry | Science Exams | Text QA | 2023.12 | EN | Other sources | Semi-automated | N/A | Data generation and review | N/A | 515 | Expert | MCQ | Acc |
| [MMLU ](https://huggingface.co/datasets/cais/mmlu) | Physics (College Physics, Conceptual Physics, High School Physics), Chemistry (College Chemistry, High School Chemistry), Biology (College Biology, High School Biology) | Science QA | Text QA | 2020.09 | EN | Books and literary works | Manual | 7 | Data generation and review | N/A | 15.9k | Secondary School, Undergraduate, Expert | MCQ | Acc |
| [C-Eval ](https://github.com/hkust-nlp/ceval) | Chemistry (College Chemistry, High School Chemistry, Middle School Chemistry), Physics (College Physics, High School Physics, Middle School Physics), Biology (High School Biology, Middle School Biology), Medicine (Veterinary Medicine, Basic Medicine, Clinical Medicine, Physician), Earth Science (High School Geography, Middle School Geography) | Exam questions, Chinese educational assessments | Text QA | 2023.05 | ZH | Books and literary works | Manual | 12 | Data generation and review | N/A | 13.9k | Primary school, Secondary school, Undergraduate | MCQ | Acc |
| [GPQA ](https://github.com/idavidrein/gpqa) | Chemistry, Biology, Physics | Graduate-level scientific questions | Text QA | 2023.11 | EN | Other sources | Manual | 8 | Data generation and review | N/A | 448 | Expert | MCQ | Acc |
| [ArXivQA ](https://huggingface.co/datasets/MMInstruction/ArxivQA) | Physics (Accelerator Physics, High Energy Physics - Lattice, Mathematical Physics, \etc), Chemistry (Chemical Physics), Biology (Quantitative Biology), Material (Materials Theory) | scientific figure question-answer | Text QA | 2024.05 | EN, ZH | Other sources | Semi-automated | N/A | Data generation and review | GPT-4V | 249,587 | Expert | MCQ | Acc |
| [Xiezhi ](https://github.com/MikeGu721/XiezhiBenchmark) | Agronomy (Crop Science, Veterinary Medicine), Science (Chemistry, Physics), Medicine (Traditional Chinese Medicine) | Professional exams | Text QA | 2024.05 | EN | Comprehensive multi-source integration | Semi-automated | N/A | Data review | ChatGPT, Llama-7B | 250k | Expert | MCQ | Acc |
| [SuperGPQA ](https://huggingface.co/datasets/m-a-p/SuperGPQA) | Medicine, Science, Agriculture | Graduate Disciplines QA | Text QA | 2025.02 | EN | Other sources | Semi-automatic | 80+ | Data generation and review | N/A | 26.5k | Expert | MCQ | Acc |
| [BMMR ](https://bmmr.pages.dev/) | Health (Medicine, Pharmacy, \etc), Natural Sciences (Physics, Biology, \etc), Agriculture | Image, College-level visual question answering, OCR-based QA | VQA | 2025.07 | EN, ZH | Web and Internet content, Books and literary works, Integration of existing datasets | Semi-automated | N/A | Data generation and review | N/A | 109,449 | Primary school, Undergraduate, Secondary school | MCQ | Acc |
| [OlympiadBench ](https://github.com/OpenBMB/OlympiadBench) | Physics, Mathematics | QA from math and physics competitions, Image | Text QA, VQA | 2024.02 | ZH, EN | Other sources | Semi-automated | 14 | Data generation and review | N/A | 8.5k | Expert | Open-ended | Acc |
| [LLM-SRBench ](https://github.com/deep-symbolic-mathematics/llm-srbench) | LSR-Synth (Chemistry, Biology, Physics, Material Science), LSR-Transform | Structured Data | text | 2025.04 | EN | Comprehensive multi-source integration | Fully-automated | 0 | Data generation and review | N/A | 239 | Expert | Open-ended | Exact Match, MSE |
| [HLE ](https://lastexam.ai/) | Biology (Marine Biology, Molecular Biology, Computational Biology, Ecology, \etc), Chemistry (Chemical Engineering, Biochemistry, \etc), Physics (Biophysics), Materials Science | Organic reaction analysis, Molecular text, Chemical equations, Medical question answering, Textbook QA, \etc | Text QA | 2025.01 | EN | Academic and research resources | Manual | nearly 1000 | Data generation and review | GPT-4o | 2,500 | Expert | MCQ, Open-ended | Acc, Calibration Error |
| [SFE ](https://prismax.opencompass.org.cn/) | Astronomy, Chemistry, Life Science, Materials Science, Earth Science | Protein structure, RNA structure, Molecular structure, \etc | VQA | 2025.06 | EN, ZH | Scientific databases, Academic and research resources | Manual | N/A | Data generation and review | GPT-4o | 1,660 | Expert | MCQ, Open-ended | Exact Match, LLM-as-a-Judge score, BERTScore, IoU |
| [SciEval ](https://github.com/OpenDFM/SciEval) | Chemistry, Physics, Biology | Text (equations, molecules, chemical reactions, scientific QA, \etc) | Text QA | 2023.08 | EN | Comprehensive multi-source integration | Semi-automated | N/A | Data review | GPT-4 | 18,000 | Undergraduate, Graduate | MCQ, Open-ended, True/False | Acc, BLEU, MSE |
| [SciKnowEval ](https://huggingface.co/datasets/hicai-zju/SciKnowEval) | Chemistry, Physics, Biology, Materials Science | Textbook QA, Literature QA, SMILES, IUPAC, Equations, \etc | Text QA, Classification, Regression | 2024.06 | EN | Comprehensive multi-source integration, Academic and research resources, Scientific databases, Integration of existing datasets | Semi-automated | N/A | Data review | GPT-4o, GPT-3.5, Claude3, LLaMA, Qwen | 70,203 | Undergraduate, Graduate, Expert | MCQ, True/False, Open-ended | Acc, F1, BLEU, ROUGE, Smith-Waterman, Tanimoto |
| [AGIEval ](https://agi-eval.org/mvp/home) | Chemistry (GK-chemistry), Physics (GK-physics), Biology (GK-biology), Geography (GK-geography) | Textbook, Literature, SMILES, IUPAC, Equations, \etc | Text QA | 2023.09 | EN, ZH | Academic and research resources, Integration of existing datasets | Semi-automated | N/A | Data review | ChatGPT, GPT-4 | 8,062 | Secondary school, Undergraduate | MCQ, Open-ended | Acc, EM |
| [ScienceAgentBench ](https://osu-nlp-group.github.io/ScienceAgentBench/) | Bioinformatics, Computational chemistry, Geographical information science, Psychology & cognitive neuroscience | Microscopy images, SMILES strings, Geospatial data, EEG, ECG, IMU, \etc | VQA | 2024.10 | EN | Academic and research resources, Integration of existing datasets | Manual | 9 | Data generation and review | N/A | 102 tasks | Expert | Open-ended | VER, SR, CodeBERTScore, GPT-4o Judge |
| [MMVU](https://mmvu-benchmark.github.io/) | General Science, Healthcare, Engineering, Humanities and Social Science | Scientific Videos | Video QA | 2025.1 | EN | Academic and research resources | Manual | 67 | Data generation and review | N/A | 3,000 | Expert | MCQ, True/False | Acc, GPT-4o Judge |
| [SciArena](https://allenai.org/blog/sciarena) | General Science, Healthcare, Engineering, Humanities and Social Science | Scientific Literature | Text QA | 2025.7 | EN | Academic and research resources | Manual | N/A | Data generation | N/A | 13K+ | Expert | Open-ended | Human Preference |
</details>

## 🤖 Scientific Models

<details>
<summary>

### 🌐 General-purpose

</summary>

 <a href="#-table-of-contents" style="float:right;">⬆ Back to Top</a>
| Models | Domain | Parameters | Base LLM | Modality encoder | Release | Open-source |
|---|---|---|---|---|---|---|
| [Galactica ](https://github.com/paperswithcode/galai) | General Science | 120B | N/A | N/A | 2022.11 | ✅ |
| [DARWIN ](https://github.com/MasterAI-EAM/Darwin) | General Science | 7B | LLaMA-7B, Vicuna-7B | N/A | 2023.08 | ✅ |
| [FORGE ](https://github.com/at-aaims/forge) | General Science | 26B | GPT-NeoX | N/A | 2023.11 | ✅ |
| [SciGLM ](https://github.com/THUDM/SciGLM) | General Science | 6B / 32B | ChatGLM3 | N/A | 2024.01 | ✅ |
| [SciDFM ](https://huggingface.co/OpenDFM/SciDFM-MoE-A5.6B-v1.0) | General Science | 18.2B-A5.6B | N/A | N/A | 2024.09 | ✅ |
| [OmniScience ](https://github.com/google-deepmind/alphafold3?tab=readme-ov-file) | General Science | 70B | LLaMA-3.1 | N/A | 2025.03 | ❌ |
| [Intern-S1 ](https://github.com/InternLM/Intern-S1) | General Science | 241B-A28B/8B | Qwen3-235B-A22B, Qwen3-8B | InternViT-6B, InternViT-300M | 2025.08 | ✅ |

</details>

<details>
<summary>
 
 ### ⚛️ Physics
 
 </summary>
 
 <a href="#-table-of-contents" style="float:right;">⬆ Back to Top</a>

| Models | Domain | Parameters | Base LLM | Modality encoder | Release | Open-source |
|---|---|---|---|---|---|---|
| [MechGPT ](https://github.com/lamm-mit/MeLM) | Mechanics | 13B / 70B | LLaMA-2 | N/A | 2023.10 | ✅ |
| [Xiwu ](https://github.com/zhangzhengde0225/Xiwu) | High Energy Physics | 7B / 13B | LLaMA, Vicuna, ChatGLM, Grok-1 | N/A | 2024.04 | ✅ |
| [Poseidon ](https://github.com/camlab-ethz/poseidon) | Partial Differential Equations | 0.02B / 0.2B / 0.6B | scOT | N/A | 2024.05 | ✅ |
| [L3M ](https://arxiv.org/pdf/2506.14757) | Astrophysics | 0.5B | Qwen2.5-0.5B-Instruct | N/A | 2025.06 | ❌ |

</details>

<details>
<summary>

### ⚗️ Chemistry

</summary>

 <a href="#-table-of-contents" style="float:right;">⬆ Back to Top</a>
| Models | Domain | Parameters | Base LLM | Modality encoder | Release | Open-source |
|---|---|---|---|---|---|---|
| [ChemLLM ](https://github.com/keyhsw/chemllm) | Chemistry, Pharmacy | 7B | InternLM2 | N/A | 2024.06 | ✅ |
| LLM-RDF | Chemistry, chemical synthesis | N/A | GPT-4 | N/A | 2024.11 | ✅ |
| [InstructMol ](https://github.com/IDEA-XL/InstructMol) | Biochemistry, Chemistry, Pharmacy | 7B | LLaMA | molecular graph encoder | 2024.12 | ✅ |
| [ChemDFM ](https://huggingface.co/OpenDFM/ChemDFM-v1.0-13B) | Chemistry (molecular design), Chemistry | 13B | LLaMA-2 | N/A | 2025.07 | ✅ |
| [ChemMLLM ](https://huggingface.co/AI4Chem) | Chemistry (molecular design), Pharmacy | 34B | Lumina-mGPT-34B-512 | VQGAN | 2025.08 | ✅ |
| Chemma | Chemistry, Organic Chemistry | 7B | LLaMA-2 | N/A | 2025.07 | ✅ |
| Chem3DLLM | Chemistry (Molecular Design), Pharmacy | 7B | Qwen2-7B | ESM-Encoder | 2025.08 | ✅ |

</details>

<details>
<summary>
  
### 🪨 Materials Science

</summary>

 <a href="#-table-of-contents" style="float:right;">⬆ Back to Top</a>
| Models | Domain | Parameters | Base LLM | Modality encoder | Release | Open-source |
|---|---|---|---|---|---|---|
| [SMILES-BERT ](https://github.com/uta-smile/SMILES-BERT) | Materials Science | 30M | BERT-small | N/A | 2019.09 | ✅ |
| [MolGPT ](https://github.com/devalab/molgpt) | Materials Science | N/A | N/A | N/A | 2022.05 | ✅ |
| MOFormer | Materials Science | N/A | N/A | N/A | 2022.10 | ❌ |
| [MatBert-bandgap ](https://huggingface.co/korolewadim/matbert-bandgap) | Materials Science | 110M | MatBERT | N/A | 2023.03 | ✅ |
| [Regression Transformer ](https://github.com/IBM/regression-transformer) | Materials Science | N/A | N/A | N/A | 2023.04 | ✅ |
| [MolXPT ](https://huggingface.co/zequnl/molxp) | Materials Science | N/A | GPT-2 | N/A | 2023.05 | ✅ |
| [xyztransformer ](https://github.com/danielflamshep/xyztransformer) | Materials Science | N/A | N/A | N/A | 2023.05 | ✅ |
| [polyBERT ](https://github.com/Ramprasad-Group/polyBERT) | Materials Science | N/A | DeBERTa | N/A | 2023.07 | ✅ |
| GPT-MolBERTa | Materials Science | N/A | RoBERTa | N/A | 2023.10 | ❌ |
| ChemRLformer | Materials Science | N/A | N/A | N/A | 2023.10 | ❌ |
| [CrystaLLM ](https://github.com/facebookresearch/crystal-text-llm) | Materials Science | 70B | LLaMA-2 70B | N/A | 2024.02 | ✅ |
| [MatText ](https://github.com/lamalab-org/mattext) | Materials Science | N/A | BERT | N/A | 2024.06 | ✅ |
| [ChatMOF ](https://github.com/Yeonghun1675/ChatMOF) | Materials Science | N/A | GPT-4, GPT-3.5-turbo, and GPT-3.5-turbo-16k | N/A | 2024.06 | ✅ |
| LHS2RHS | Materials Science | N/A | N/A | N/A | 2024.10 | ❌ |
| RHS2LHS | Materials Science | N/A | N/A | N/A | 2024.10 | ❌ |
| TGT2CEQ | Materials Science | N/A | N/A | N/A | 2024.10 | ❌ |
| [CrystaLLM ](https://github.com/lantunes/CrystaLLM) | Materials Science | 200M | GPT-2 | N/A | 2024.12 | ✅ |
| [molT5-large ](https://github.com/Mantas-it/Chem_Procedure_Prediction) | Materials Science | 770M | T5-large | N/A | 2024.12 | ✅ |
| [Qwen2-KG ](https://github.com/MontageBai/KGFM) | Materials Science | 72B | Qwen2-72B | N/A | 2025.02 | ✅ |
| [LLM-Prop ](https://github.com/vertaix/LLM-Prop) | Materials Science | 37M | T5-small | N/A | 2025.06 | ✅ |
| [Crystal Synthesis LLM ](https://github.com/szl666/CSLLM) | Materials Science | 8B | LLaMA-3-8B | N/A | 2025.07 | ✅ |

</details>

<details>
<summary>
  
### 🧬 Life Sciences

</summary>

 <a href="#-table-of-contents" style="float:right;">⬆ Back to Top</a>
| Models | Domain | Parameters | Base LLM | Modality encoder | Release | Open-source |
|---|---|---|---|---|---|---|
| [ShizhenGPT ](https://github.com/FreedomIntelligence/ShizhenGPT) | Healthcare and Medical Sciences | 7B / 32B | Qwen2.5 | Qwen2.5-VL vision encoder, Whisper-large-v3 | 2025.08 | ✅ |
| [ProGen2 ](https://neurosnap.ai/service/ProGen2) | Proteomics | 6.4B / 2.7B / 764M / 151M | N/A | N/A | 2022.06 | ✅ |
| [BioGPT ](https://huggingface.co/microsoft/biogpt) | Healthcare and Medical Sciences, General Biology | 347M | GPT-2 | N/A | 2022.10 | ✅ |
| [ESM-2 ](https://github.com/facebookresearch/esm) | Proteomics | 15B / 3B / 650M /150M/ 35M / 8M | N/A | N/A | 2023.03 | ✅ |
| [OphGLM ](https://github.com/ML-AILab/OphGLM) | Healthcare and Medical Sciences | 6B | ChatGLM-6B | ConvNext | 2023.03 | ✅ |
| [MedAlpaca ](https://github.com/kbressem/medAlpaca) | Healthcare and Medical Sciences | 7B / 13B | LLaMA | N/A | 2023.04 | ✅ |
| [DoctorGLM ](https://xionghonglin.github.io/DoctorGLM/) | Healthcare and Medical Sciences | 6B | ChatGLM-6B | N/A | 2023.04 | ✅ |
| [PMC-LLaMA ](https://github.com/chaoyi-wu/PMC-LLaMA) | Healthcare and Medical Sciences | 13B | LLaMA | N/A | 2023.04 | ✅ |
| [scGPT ](https://github.com/bowang-lab/scGPT) | Multi-omics | 30k / 300k / 3M / 33M | N/A | N/A | 2023.04 | ✅ |
| [Med-PaLM ](https://sites.research.google/med-palm/) | Healthcare and Medical Sciences | N/A | PaLM | N/A | 2023.05 | ❌ |
| [Med-PaLM 2 ](https://sites.research.google/med-palm/) | Healthcare and Medical Sciences | N/A | PaLM 2 | N/A | 2023.05 | ❌ |
| [GatorTronS ](https://huggingface.co/UFNLP/gatortronS) | Healthcare and Medical Sciences | 345M / 3.9B / 8.9B | GPT-3 | N/A | 2023.05 | ✅ |
| [GatorTronGPT ](https://github.com/uf-hobi-informatics-lab/GatorTronGPT) | Healthcare and Medical Sciences | 5B / 20B | GPT-3 | N/A | 2023.05 | ✅ |
| [HuatuoGPT ](https://github.com/FreedomIntelligence/HuatuoGPT) | Healthcare and Medical Sciences | 7B / 13B | Baichuan-7B, Ziya-LLaMA-13B-Pretrain-v1 | N/A | 2023.05 | ✅ |
| [BiomedGPT ](https://github.com/taokz/BiomedGPT) | Healthcare and Medical Sciences | 33M / 93M / 182M | OFA | VQ-GAN | 2023.05 | ✅ |
| [ClinicalGPT ](https://huggingface.co/medicalai/ClinicalGPT-base-zh) | Healthcare and Medical Sciences | 7B | BLOOM-7B | N/A | 2023.06 | ✅ |
| [GENA-LM ](https://github.com/AIRI-Institute/GENA_LM) | Molecular and Cell Biology, Multi-omics | 110M / 336M | BERT | N/A | 2023.06 | ✅ |
| [NYUTron ](https://hslguides.med.nyu.edu/aihsl/nyutron) | Healthcare and Medical Sciences, Neuroscience, Pharmacy | 190M | BERT | N/A | 2023.06 | ✅ |
| [ChatDoctor ](https://github.com/Kent0n-Li/ChatDoctor) | Healthcare and Medical Sciences | 7B | LLaMA | N/A | 2023.06 | ✅ |
| [SoulChat ](https://github.com/scutcyr/SoulChat) | Neuroscience, Healthcare and Medical Sciences | 6B | ChatGLM-6B | N/A | 2023.07 | ✅ |
| [DNAGPT ](https://github.com/TencentAILabHealthcare/DNAGPT) | Molecular and Cell Biology, Multi-omics | 3B | GPT | N/A | 2023.07 | ✅ |
| [Med-Flamingo ](https://huggingface.co/med-flamingo/med-flamingo) | Healthcare and Medical Sciences | 9B | Openflamingo | Openflamingo | 2023.07 | ✅ |
| [DISC-MedLLM ](https://huggingface.co/Flmc/DISC-MedLLM) | Healthcare and Medical Sciences | 13B | Baichuan-13B | N/A | 2023.08 | ✅ |
| [IvyGPT ](https://github.com/WangRongsheng/IvyGPT) | Healthcare and Medical Sciences | 33B | LLaMA-33B | N/A | 2023.08 | ❌ |
| [Zhongjing ](https://github.com/SupritYoung/Zhongjing) | Healthcare and Medical Sciences | 13B | Ziya-LLaMA-13B-V1 | N/A | 2023.08 | ✅ |
| [Radiology-Llama2 ](https://huggingface.co/allen-eric/radiology-llama2) | Healthcare and Medical Sciences | 7B | LLaMA-2 | N/A | 2023.08 | ✅ |
| [RadFM ](https://github.com/chaoyi-wu/RadFM) | Healthcare and Medical Sciences | 9B | MedLLaMA-13B | 3D ViT | 2023.08 | ✅ |
| [CPLLM ](https://github.com/nadavlab/CPLLM) | Healthcare and Medical Sciences | 13B | Llama2-13B | N/A | 2023.09 | ✅ |
| [DRG-LLaMA ](https://github.com/hanyin88/DRG-LLaMA) | Healthcare and Medical Sciences | 7B | LLaMA-7B | N/A | 2023.09 | ✅ |
| [MindGPT ](https://github.com/JxuanC/MindGPT) | Neuroscience, Healthcare and Medical Sciences | 124M | GPT-2 | CLIP-ViT-B/32 | 2023.09 | ❌ |
| [BioinspiredLLM ](https://huggingface.co/lamm-mit/BioinspiredLLM) | General Biology, Molecular and Cell Biology, Proteomics | 13B | LLaMA-2 | N/A | 2023.09 | ✅ |
| [Qilin-Med ](https://github.com/williamliujl/Qilin-Med) | Healthcare and Medical Sciences | 7B | Baichuan-7B | N/A | 2023.10 | ❌ |
| [CXR-LLAVA ](https://github.com/ECOFRI/CXR_LLaVA) | Healthcare and Medical Sciences | 7B | LLaMA-2 | CLIP ViT-L/16 | 2023.10 | ✅ |
| InstructProtein | Proteomics | 1.3B | OPT-1.3B | N/A | 2023.10 | ❌ |
| [ChiMed-GPT ](https://huggingface.co/SYNLP/ChiMed-GPT-1.0) | Healthcare and Medical Sciences | 13B | Ziya-13B-v2 | N/A | 2023.11 | ✅ |
| [HuatuoGPT-II ](https://github.com/FreedomIntelligence/HuatuoGPT-II) | Healthcare and Medical Sciences | 7B/13B | Baichuan2-7B-Base, Baichuan2-13B-Base | N/A | 2023.11 | ✅ |
| [Taiyi-LLM ](https://github.com/DUTIR-BioNLP/Taiyi-LLM) | Healthcare and Medical Sciences | 7B | Qwen-7B-base | N/A | 2023.11 | ✅ |
| [Meditron ](https://github.com/epfLLM/meditron) | Healthcare and Medical Sciences | 7B / 70B | LLaMA-2 | N/A | 2023.11 | ✅ |
| [MAIRA-1 ](https://aka.ms/maira) | Healthcare and Medical Sciences | 7B | Vicuna-7B | RAD-DINO | 2023.11 | ✅ |
| [MAIRA-2 ](https://huggingface.co/microsoft/maira-2) | Healthcare and Medical Sciences | 7B | Vicuna-7B-v1.5 | RAD-DINO | 2023.11 | ✅ |
| [Neuro-GPT ](https://huggingface.co/wenhuic/Neuro-GPT) | Neuroscience, Healthcare and Medical Sciences | 124M | GPT-2 | EEG Encoder | 2023.11 | ✅ |
| [PLLaMa ](https://huggingface.co/Xianjun/PLLaMa-7b-instruct) | Molecular and Cell Biology, General Biology | 7B / 13B | LLaMA-2 | N/A | 2024.01 | ✅ |
| [EEG-GPT ](https://github.com/neurosity/EEG-GPT) | Neuroscience | N/A | GPT-3 | EEG Encoder | 2024.01 | ❌ |
| [BioMistral ](https://huggingface.co/BioMistral/BioMistral-7B) | Healthcare and Medical Sciences, Molecular and Cell Biology | 7B | Mistral-7B-Instruct-v0.1 | N/A | 2024.02 | ✅ |
| [MMed-LLaMA 3 ](https://huggingface.co/Henrychur/MMed-Llama-3-8B) | Healthcare and Medical Sciences | 8B | LLaMA 3 | N/A | 2024.02 | ✅ |
| [ProLLaMA ](https://github.com/PKU-YuanGroup/ProLLaMA) | Proteomics | 7B | LLaMA-2 | N/A | 2024.02 | ✅ |
| [ProtLLM ](https://protllm.github.io/project) | Proteomics | 7B | LLaMA-7B | ProtST (protein) | 2024.03 | ✅ |
| [BrainGPT ](https://huggingface.co/BrainGPT) | Neuroscience | 7B | Mistral-7B | N/A | 2024.03 | ✅ |
| [Apallo ](https://github.com/FreedomIntelligence/Apollo) | Healthcare and Medical Sciences | 0.5B / 1.8B / 2B / 6B / 7B | Qwen | N/A | 2024.03 | ✅ |
| [Med-Gemini ](https://github.com/Google-Health/med-gemini-medqa-relabelling) | Healthcare and Medical Sciences | N/A | Gemini 1.5 Pro | Custom encoders (multimodal) | 2024.04 | ❌ |
| [UMBRAE ](https://huggingface.co/datasets/weihaox/umbrae) | Neuroscience | 7B | Vicuna-7B | CLIP-ViT/L-14 (vision), Encoder (fMRI) | 2024.04 | ✅ |
| [SeedLLM ](https://seedllm.org.cn) | Agronomy | 7B | Qwen2.5 | N/A | 2024.04 | ❌ |
| [Alphafold3 ](https://github.com/google-deepmind/alphafold3) | Molecular and Cell Biology, Proteomics, Pharmacy, Neuroscience | N/A | N/A | Input Feature Embedder | 2024.05 | ❌ |
| [DrugLLM ](https://huggingface.co/efedemircan/drugllm) | Pharmacy | 7B | LLaMA 7B | N/A | 2024.05 | ❌ |
| [LLaVA-Med ](https://github.com/microsoft/LLaVA-Med) | Healthcare and Medical Sciences | N/A | Vicuna-7B | Clip ViT-L/14 | 2024.05 | ✅ |
| [CareGPT ](https://github.com/WangRongsheng/CareGPT) | Healthcare and Medical Sciences | 7B | LLaMA-2 | N/A | 2024.05 | ✅ |
| [ProtT3 ](https://github.com/acharkq/ProtT3) | Proteomics | N/A | Galactica 1.3B | ESM-2 (protein) | 2024.05 | ✅ |
| [MolecularGPT ](https://github.com/NYUSHCS/MolecularGPT) | Molecular and Cell Biology | N/A | LLaMA | N/A | 2024.06 | ✅ |
| [HuatuoGPT-Vision ](https://github.com/FreedomIntelligence/HuatuoGPT-Vision) | Healthcare and Medical Sciences | 7B / 34B | Qwen2-7B | Qwen Image Encoder (vision) | 2024.06 | ✅ |
| [NeuroLM ](https://huggingface.co/Weibang/NeuroLM) | Neuroscience | 254M/500M/1.7B | GPT-2 | Encoder (EEG) | 2024.08 | ✅ |
| [RNAGPT ](https://rna-gpt.github.io/) | Molecular and Cell Biology, Multi-omics | 8B | LLaMA-3 | RNA-FM sequence encoder (RNA) | 2024.10 | ❌ |
| [AgroGPT ](https://github.com/AI-agriculture/AgroGPT) | Agronomy | 3B / 7B | LLaVA-1.5, Mipha | CLIP-ViT-L/14 (vision), SigLIP | 2024.10 | ✅ |
| [LLaMA-Gene ](https://github.com/maris205/llama-gene) | Molecular and Cell Biology, Proteomics | 7B | LLaMA-7B | N/A | 2024.11 | ✅ |
| [GMAI-VL ](https://github.com/uni-medical/GMAI-VL) | Healthcare and Medical Sciences | 7B | InternLM | Image Encoder (vision) | 2024.11 | ✅ |
| [HuatuoGPT-o1 ](https://github.com/FreedomIntelligence/HuatuoGPT-o1) | Healthcare and Medical Sciences | 7B / 8B / 70B / 72B | LLaMA-3.1, Qwen2.5 | N/A | 2024.12 | ✅ |
| [Evolla ](https://github.com/westlake-repl/Evolla) | Proteomics | 10B / 80B | LLaMA-3 8B | Saprot (protein) | 2025.01 | ✅ |
| UniMind | Neuroscience | 7B | InternLM2.5 | Encoder (EEG) | 2025.01 | ❌ |
| [NatureLM ](https://naturelm.github.io/) | Pharmacy, Molecular and Cell Biology, Proteomics, Material | 46.7B | Mixtral 8x7B | N/A | 2025.02 | ❌ |
| [MindLLM ](https://huggingface.co/BoltzmachineQ/MindLLM) | Neuroscience, Healthcare and Medical Sciences | 7B | Vicuna-7B | Encoder (fMRI) | 2025.02 | ✅ |
| [MedVLM-R1 ](https://huggingface.co/JZPeterPan/MedVLM-R1) | Healthcare and Medical Sciences | 2B | Qwen2-VL | Qwen Image Encoder (vision) | 2025.02 | ✅ |
| [AlphaGenome ](https://github.com/google-deepmind/alphagenome) | Molecular and Cell Biology, Multi-omics | N/A | N/A | N/A | 2025.05 | ✅ |
| [ChatNT ](https://instadeep.com/2025/06/talking-biology-with-chatnt) | Molecular and Cell Biology, Proteomics, Multi-omics | 7B | Vicuna-7B | Nucleotide Transformer v2 (DNA) | 2025.06 | ✅ |
| [Lingshu ](https://huggingface.co/papers/2506.07044) | Healthcare and Medical Sciences | 7B / 32B | Qwen | N/A | 2025.06 | ✅ |
| [PodGPT ](https://github.com/vkola-lab/PodGPT) | Healthcare and Medical Sciences | N/A | Gemma, Mixtral, LLaMA | N/A | 2025.07 | ✅ |
| [MedGemma ](https://github.com/Google-Health/medgemma) | Healthcare and Medical Sciences | 4B / 27B | Gemma 3 | SigLip Image Encoder (vision) | 2025.07 | ✅ |
| [MedMax ](https://github.com/Hritikbansal/medmax) | Natively Multimodal Biomedical Tasks | 7B | Meta Chameleon| N/A| 2024.12 | ✅ |

</details>

<details>
<summary>
  
### 🌌 Astronomy

</summary>

 <a href="#-table-of-contents" style="float:right;">⬆ Back to Top</a>
| Models | Domain | Parameters | Base LLM | Modality encoder | Release | Open-source |
|---|---|---|---|---|---|---|
| [AstroLLaMA-2-7B ](https://huggingface.co/UniverseTBD/astrollama) | Astronomy | 7B | Llama-2 LLM | N/A | 2023.09 | ✅ |
| [AstroLLaMA-3-8B ](https://huggingface.co/AstroMLab/astrollama-2-70b-chat_aic) | Astronomy | 8B | LLaMA-2-7B LLM | N/A | 2024.09 | ✅ |
| [AstroLLaMA-2-70B ](https://huggingface.co/AstroMLab/astrollama-2-70b-chat_aic) | Astronomy | 70B | LLaMA-2-7B LLM | N/A | 2024.09 | ✅ |
| [AstroSage-LLaMA-3.1-8B ](https://huggingface.co/AstroMLab/AstroSage-8B) | Astronomy | 8B | Llama-3.1-8B LLM | N/A | 2025.04 | ✅ |
| [AstroLLaVa-7B ](https://huggingface.co/UniverseTBD/astrollama) | Astronomy | 7B | LLaVA 1.5 LLM | CLIP-ViT/L-14 (vision) | 2025.04 | ✅ |
| [AstroSage-LLaMA-3.1-70B ](https://w3id.org/UniverseTBD/AstroLLaVA) | Astronomy | 70B | Llama-3.1-70B LLM | N/A | 2025.05 | ✅ |

</details>

<details>
<summary>
  
### 🌍 Earth Science

</summary>

 <a href="#-table-of-contents" style="float:right;">⬆ Back to Top</a>
| Models | Domain | Parameters | Base LLM | Modality encoder | Release | Open-source |
|---|---|---|---|---|---|---|
| [OceanGPT ](https://huggingface.co/collections/zjunlp/oceangpt-664cc106358fdd9f09aa5157) | Hydrosphere, Biosphere, Lithosphere, Remote Sensing | 7B | LLama, Qwen | N/A | 2023.03 | ✅ |
| [K2 ](https://huggingface.co/daven3/k2) | Lithosphere, Remote Sensing | 7B | LLama | N/A | 2023.08 | ✅ |
| [GeoChat ](https://github.com/mbzuai-oryx/GeoChat) | Remote Sensing, Lithosphere | 7B | Vicuna-v1.5 | N/A | 2023.11 | ✅ |
| [SkyEyeGPT ](https://github.com/ZhanYang-nwpu/SkyEyeGPT) | Remote Sensing | 7B | N/A | N/A | 2024.01 | ✅ |
| [TeoChat ](https://github.com/ermongroup/TEOChat) | Remote Sensing, Lithosphere | 7B | Vdieo-LLaVA | N/A | 2024.10 | ✅ |
| [EarthMarker ](https://github.com/wivizhang/EarthMarker) | Remote Sensing | 13B | LLaMA-2 | N/A | 2024.11 | ✅ |
| [EarthDial ](https://github.com/hiyamdebary/EarthDial) | Remote Sensing | 4B | Phi-3-mini | N/A | 2024.12 | ✅ |
| [GeoPixel ](https://github.com/mbzuai-oryx/GeoPixel) | Remote Sensing, Lithosphere | 7B | IXC-2.5 | N/A | 2025.01 | ✅ |
| [EagleVision ](https://github.com/XiangTodayEatsWhat/EagleVision) | Remote Sensing | 1B/2B/4B/7B | Qwen2-VL-72B, GPT-4o | N/A | 2025.03 | ✅ |
| [ClimateChat ](https://huggingface.co/itpossible/ClimateChat) | Lithosphere, Climate | 7B | jiuZhou | N/A | 2025.03 | ✅ |
| [GeoGPT ](https://huggingface.co/GeoGPT-Research-Project/GeoGPT-R1-Preview) | Lithosphere, Remote Sensing | 70B | Llama3.1-70B, Qwen2.5-72B | N/A | 2025.04 | ✅ |
| [GeoLLaVA-8K ](https://github.com/MiliLab/GeoLLaVA-8K) | Remote Sensing, Lithosphere | 7B | LongVA | N/A | 2025.05 | ✅ |
</details>

## 📅 Star History  
 <a href="#-table-of-contents" style="float:right;">⬆ Back to Top</a>

[![Star History Chart](https://api.star-history.com/svg?repos=open-sciencelab/Awesome-Scientific-Datasets-and-LLMs&type=Date)](https://www.star-history.com/#open-sciencelab/Awesome-Scientific-Datasets-and-LLMs&Date)
