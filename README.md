# Awesome-MLSecOps

## Table of Contents

- [Introduction to MLSecOps](#Introduction-to-MLSecOps)
- [Security & Privacy Considerations in ML](#Security-&-Privacy-Considerations-in-ML)
- [MLSecOps Phases](#MLSecOps-Phases)
  - [Security & Privacy in the Data Layer](#Security-&-Privacy-in-the-Data-Layer)
  - [Security & Privacy in the Model Layer](#Security-&-Privacy-in-the-Model-Layer)
  - [Security & Privacy in the Application Layer](#Security-&-Privacy-in-the-Application-Layer)
- [Security Tools & Resources](#Security-Tools-&-Resources)
  - [Open Source Tools](#Open-Source-Tools)
  - [Commercial Tools & Solutions](#Commercial-Tools-&-Solutions)
  - [Books & Publications](#Books-&-Publications)
  - [Community Resources](#Community-Resources)
- [MLOps Infrastructure & DevSecOps](#MLOps-Infrastructure-&-DevSecOps)

## Introduction to MLSecOps

MLSecOps (Machine Learning Security Operations) is an emerging discipline that merges machine learning (ML), security, and operations (Ops) to create a holistic framework for addressing the unique security challenges posed by machine learning systems. With the growing use of machine learning models in critical applications—ranging from autonomous driving to medical diagnosis and financial services—the need to integrate security measures into the ML lifecycle has never been more pressing. MLSecOps builds on the principles of DevSecOps, which aims to ensure security is woven into every part of the software development lifecycle, and applies these principles to the realm of machine learning.

## Security Tools & Resources

### Open Source Tools

| Tool | Description | Risk |
|------|-------------|------|
| [DeepSec](https://github.com/ryderling/DEEPSEC) | A framework for evaluating the robustness of machine learning models against adversarial and other security threats. | R9-Security |
| [AIF360](https://github.com/IBM/AIF360) | A library developed by IBM for detecting and mitigating bias in AI models to improve fairness and privacy. | R4-Security |
| [Fairness Indicators](https://github.com/tensorflow/fairness-indicators) | Tools for assessing fairness and biases in machine learning models, focusing on metrics to identify potential risks in data and predictions. | R4-Security |
| [FastGradientMethod](https://github.com/cleverhans-lab/cleverhans) | A part of CleverHans that implements the Fast Gradient Sign Method (FGSM) attack for evaluating and defending against adversarial attacks. | R9-Security |
| [Adversarial Robustness Toolkit](https://github.com/Trusted-AI/adversarial-robustness-toolbox) | A toolkit that provides a variety of attacks and defenses for evaluating adversarial robustness in ML models. | R9-Security, R10-Security |
| [AIShield Watchtower](https://github.com/bosch-aisecurity-aishield/watchtower) | AIShield Watchtower: Dive Deep into AI's Secrets! Open-source tool by AIShield for AI model insights & vulnerability scans. Secure your AI supply chain today! | R16-Security |
| [SafeML](https://github.com/ISorokos/SafeML) | Exploring techniques for estimating safety of machine learning classifiers | R10-Security |
| [Garak](https://github.com/leondz/garak) | LLM vulnerability scanner that detects security flaws in large language models, focusing on prompt injection and adversarial vulnerabilities. | R17-Security, R10-Security, R9-Security |
| [ModelScan](https://github.com/protectai/modelscan) | Protection Against ML Model Serialization Attacks, preventing malicious modifications of stored model files. | R5-Security, R7-Security |
| [NB Defense](https://nbdefense.ai) | Secure Jupyter Notebooks, protecting against malicious code and data leakage. | R1-Security, R3-Security, R20-Security |
| [TensorFlow Privacy](https://github.com/tensorflow/privacy) | Library of privacy-preserving machine learning algorithms and tools, including differential privacy. | R1-Privacy, R2-Privacy, R5-Privacy |
| [Foolbox](https://github.com/bethgelab/foolbox) | Python toolbox for creating and evaluating adversarial attacks and defenses. | R9-Security, R10-Security |
| [Audit AI](https://github.com/pymetrics/audit-ai) | Bias testing for generalized machine learning applications, ensuring fairness in model predictions. | R4-Security |
| [Privacy Meter](https://github.com/privacytrustlab/ml_privacy_meter) | An open-source library to audit data privacy in statistical and machine learning algorithms. | R2-Privacy, R1-Privacy, R5-Privacy |
| [Agentic Security](https://github.com/msoedov/agentic_security) | Agentic LLM Vulnerability Scanner / AI red teaming kit | R17-Security, R10-Security |
| [TF-encrypted](https://tf-encrypted.io/) | Encryption for TensorFlow, providing privacy-preserving machine learning | R1-Privacy, R2-Security |
| [AnonLLM](https://github.com/fsndzomga/anonLLM) | Anonymize Personally Identifiable Information (PII) for Large Language Model APIs | R1-Privacy |
| [AI Goat](https://github.com/dhammon/ai-goat) | Vulnerable LLM CTF challenges, a playground for discovering LLM security flaws | R17-Security, R10-Security |
| [Pyrit](https://github.com/Azure/PyRIT) | The Python Risk Identification Tool for generative AI, helps identify risks in AI models | R9-Security, R8-Privacy |
| [Raze to the Ground: Query-Efficient Adversarial HTML Attacks on Machine-Learning Phishing Webpage Detectors](https://github.com/advmlphish/raze_to_the_ground_aisec23) | Source code for query-efficient adversarial attacks on machine-learning phishing webpage detectors | R9-Security |
| [Giskard](https://github.com/Giskard-AI/giskard) | Open-source testing tool for LLM applications to assess performance and security | R9-Security, R10-Security |
| [Safetensors](https://github.com/huggingface/safetensors) | Convert pickle to a safe serialization option, preventing security risks in model storage | R5-Security, R7-Security |
| [Citadel Lens](https://www.citadel.co.jp/en/products/lens/) | Quality testing of models according to industry standards, ensuring integrity and security | R10-Security |
| [Model-Inversion-Attack-ToolBox](https://github.com/ffhibnese/Model-Inversion-Attack-ToolBox) | A framework for implementing Model Inversion attacks, to extract sensitive data from models | R5-Privacy |
| [NeMo-Guardrails](https://github.com/NVIDIA/NeMo-Guardrails) | NeMo Guardrails help add programmable safety layers for LLM applications | R10-Security, R6-Privacy |
| [AugLy](https://github.com/facebookresearch/AugLy) | A tool for generating adversarial attacks to test robustness in models | R9-Security |
| [Knockoffnets](https://github.com/tribhuvanesh/knockoffnets) | PoC to implement BlackBox attacks to steal model data | R5-Security |
| [Robust Intelligence Continuous Validation](https://www.robustintelligence.com/platform/continuous-validation) | Tool for continuous model validation to ensure compliance with standards | R9-Security |
| [VGER](https://github.com/JosephTLucas/vger) | Jupyter Attack framework for testing vulnerabilities in Jupyter Notebooks | R20-Security |
| [AIShield Watchtower](https://github.com/bosch-aisecurity-aishield/watchtower) | Open-source tool from AIShield for studying AI models and scanning for vulnerabilities | R17-Security |
| [PS-fuzz](https://github.com/prompt-security/ps-fuzz) | Tool for scanning LLM vulnerabilities, focused on prompt injection and other attacks | R10-Security |
| [Mindgard-cli](https://github.com/Mindgard/cli/) | CLI tool for checking the security of AI models and ensuring they are robust | R9-Security |
| [PurpleLLama3](https://meta-llama.github.io/PurpleLlama/) | Check LLM security with Meta LLM Benchmark, focused on evaluating LLM vulnerabilities | R10-Security |
| [Model Transparency](https://github.com/sigstore/model-transparency) | Generates model signing to ensure integrity and transparency in AI models | R11-Security |
| [ARTkit](https://github.com/BCG-X-Official/artkit) | Automated prompt-based testing and evaluation for generative AI applications | R9-Security |
| [LangBiTe](https://github.com/SOM-Research/LangBiTe) | A bias testing framework specifically for LLMs, detecting and mitigating bias in LLMs | R4-Security |
| [OpenDP](https://github.com/opendp/opendp) | Core library for differential privacy algorithms powering the OpenDP Project | R1-Privacy, R2-Security |

### Commercial Tools & Solutions

| [Seldon](https://www.seldon.io) | Open-source platform for deploying and monitoring machine learning models with a focus on security and observability |
| [Fortinet AI Security](https://www.fortinet.com) | AI-powered security solutions for proactive threat detection and response |
| [DataRobot MLOps](https://www.datarobot.com/mlops/) | Enterprise MLOps platform for managing machine learning models' lifecycle securely |
| [Aqua Security](https://www.aquasec.com) | Cloud-native security platform to secure machine learning models in production |
| [Privitar](https://www.privitar.com) | Data privacy platform with ML-specific security features for data protection |
| [Talon Cyber Security](https://www.talonsec.com) | AI-driven endpoint protection for securing machine learning applications |
| [Anaconda Enterprise](https://www.anaconda.com/enterprise) | Secure data science platform for building and deploying machine learning models |
| [RedHat OpenShift](https://www.openshift.com) | Kubernetes-based container platform with security tools for ML model deployment |
| [HPE Ezmeral](https://www.hpe.com/us/en/ezmeral/ai-ops.html) | Enterprise AI and data analytics platform with integrated security for machine learning models |
| [Palo Alto Networks Cortex XSOAR](https://www.paloaltonetworks.com/cortex/cortex-xsoar) | AI-powered security automation platform for securing machine learning models and applications |

### Books & Publications

| Article | Description |
|------|-------------|
| | || Title | Description |
|-------|-------------|
| I Know What You Asked: Prompt Leakage via KV-Cache Sharing in Multi-Tenant LLM Serving | [Paper](https://arxiv.org/abs/2409.20002v2) |
| Prompt-to-SQL Injections in LLM-Integrated Web Applications: Risks and Defenses | [Paper](https://syssec.dpss.inesc-id.pt/papers/pedro_icse25.pdf) |
| My Model is Malware to You: Transforming AI Models into Malware by Abusing TensorFlow APIs | [Repo](https://github.com/ZJU-SEC/TensorAbuse) |
| Models Are Codes: Measuring Malicious Code Poisoning Attacks on Pre-trained Model Hubs | [Paper](https://arxiv.org/pdf/2409.09368) |
| Demystifying RCE Vulnerabilities in LLM-Integrated Apps | [Paper](https://arxiv.org/pdf/2309.02926) [Repo](https://github.com/LLMSmith/LLMSmith) |
| Cracks in The Stack: Hidden Vulnerabilities and Licensing Risks in LLM Pre-Training Datasets | [Paper](https://arxiv.org/pdf/2501.02628) |
| We Have a Package for You! A Comprehensive Analysis of Package Hallucinations by Code Generating LLMs | [Paper](https://arxiv.org/pdf/2406.10279) |
| An Empirical Study of Artifacts and Security Practices in the Pre-trained Model Supply Chain | [Paper](https://wenxin-jiang.github.io/files/publications/JiangSynovicSethiIndarapuHyattSchorlemmerThiruvathukalDavis-PTMSupplyChain-SCORED22.pdf) [Repo](https://github.com/PurdueDualityLab/SCORED22-PTMSupplyChain) |
| Naming Practices of Pre-Trained Models in Hugging Face | [Paper](https://arxiv.org/pdf/2310.01642) |
| Towards Semantic Versioning of Open Pre-trained Language Model Releases on Hugging Face | [Paper](https://arxiv.org/pdf/2409.10472) |
| A New Era in LLM Security: Exploring Security Concerns in Real-World LLM-based Systems | [Paper](https://arxiv.org/pdf/2402.18649) |
| Large Language Model Supply Chain: A Research Agenda | [Paper](https://arxiv.org/pdf/2404.12736) |
| Lifting the Veil on the Large Language Model Supply Chain: Composition, Risks, and Mitigations | [Paper](https://arxiv.org/pdf/2410.21218) |
| Large Language Model Supply Chain: Open Problems From the Security Perspective | [Paper](https://arxiv.org/pdf/2411.01604) |
| Practical LLM Security: Takeaways From a Year in the Trenches | [Link](https://www.blackhat.com/us-24/briefings/schedule/#practical-llm-security-takeaways-from-a-year-in-the-trenches-39468) [Slides](https://i.blackhat.com/BH-US-24/Presentations/US24-Harang-Practical-LLM-Security-Takeaways-From-Wednesday.pdf) |
| Isolation or Hallucination? Hacking AI Infrastructure Providers for Fun and Weights | [Link](https://www.blackhat.com/us-24/briefings/schedule/#isolation-or-hallucination-hacking-ai-infrastructure-providers-for-fun-and-weights-40569) |
| From MLOps to MLOops - Exposing the Attack Surface of Machine Learning Platforms | [Link](https://www.blackhat.com/us-24/briefings/schedule/#from-mlops-to-mloops---exposing-the-attack-surface-of-machine-learning-platforms-39309) [Slides](https://i.blackhat.com/BH-US-24/Presentations/US24-Menashe-From-MLOps-To-MLOops.pdf) |
| LLM4Shell: Discovering and Exploiting RCE Vulnerabilities in LLM-Integrated Frameworks and Apps | [Link](https://www.blackhat.com/asia-24/briefings/schedule/index.html#llmshell-discovering-and-exploiting-rce-vulnerabilities-in-real-world-llm-integrated-frameworks-and-apps-37215) [Slides](https://i.blackhat.com/Asia-24/Presentations/bh-asia-2024-llm4shell.pdf) |
| Confused Learning: Supply Chain Attacks through Machine Learning Models | [Link](https://www.blackhat.com/asia-24/briefings/schedule/index.html#confused-learning-supply-chain-attacks-through-machine-learning-models-37794) [Slides](https://i.blackhat.com/Asia-24/Presentations/Asia-24-Wood-Confused-Learning.pdf) |
| Hidden Layer: Autolabel Vulnerability Report | [Link](https://hiddenlayer.com/sai-security-advisory/2024-09-autolabel) |
| Hidden Layer: Guardrails Vulnerability Report | [Link](https://hiddenlayer.com/sai-security-advisory/2024-09-guardrails) |
| Hidden Layer: MindsDB Vulnerability Report | [Link](https://hiddenlayer.com/sai-security-advisory/2024-09-mindsdb) |
| Machine Learning Bug Bonanza – Exploiting ML Services | [Link](https://jfrog.com/blog/machine-learning-bug-bonanza-exploiting-ml-services/) |
| OWASP Top 10 for LLMs | [Link](https://owasp.org/www-project-top-10-for-large-language-model-applications/assets/PDF/OWASP-Top-10-for-LLMs-2023-v1_1.pdf) |
| Data Scientists Targeted by Malicious Hugging Face ML Models with Silent Backdoor | [Link](https://jfrog.com/blog/data-scientists-targeted-by-malicious-hugging-face-ml-models-with-silent-backdoor/) |
| More Models, More ProbLLMs | [Link](https://www.oligo.security/blog/more-models-more-probllms) |
| Shelltorch Explained: Multiple Vulnerabilities in Pytorch Model Server | [Link](https://www.oligo.security/blog/shelltorch-explained-multiple-vulnerabilities-in-pytorch-model-server) |
| Anatomy of an LLM RCE | [Link](https://www.cyberark.com/resources/threat-research-blog/anatomy-of-an-llm-rce) |
| 老树开新花：大模型时代的代码执行沙箱 | [Link](https://mp.weixin.qq.com/s/X54d0foyBS56lGFUPyOvTw) |
| 警惕Hugging Face开源组件风险被利用于大模型供应链攻击 | [Link](https://security.tencent.com/index.php/blog/msg/209) |


### Community Resources

| Community | Description |
|------|-------------|



