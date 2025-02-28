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

| Tool | Description |
|------|-------------|
| [Databricks Platform, Azure Databricks](https://azure.microsoft.com/ru-ru/products/databricks) | Datalake data management and implementation tool |
| [Hidden Layer AI Detection Response](https://hiddenlayer.com/aidr/) | Tool for detecting and responding to incidents |
| [Guardian](https://protectai.com/guardian) | Model protection in CI/CD |
| [Seldon](https://www.seldon.io) | Open-source platform for deploying and monitoring machine learning models with a focus on security and observability |
| [Fortinet AI Security](https://www.fortinet.com) | AI-powered security solutions for proactive threat detection and response |
| [Aqua Security](https://www.aquasec.com) | Cloud-native security platform to secure machine learning models in production |
| [Privitar](https://www.informatica.com/) | Data privacy platform with ML-specific security features for data protection |
| [RedHat OpenShift](https://www.openshift.com) | Kubernetes-based container platform with security tools for ML model deployment |
| [Palo Alto Networks Cortex XSOAR](https://www.paloaltonetworks.com/cortex/cortex-xsoar) | AI-powered security automation platform for securing machine learning models and applications |

### Books & Publications



### Community Resources





