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

| Tool                               | Description                                                                                                                                              |
|------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------|
| **AWS (Amazon Web Services)**      | Provides integrated services like **Amazon SageMaker** for model development and deployment with built-in security features such as IAM, VPC, and encryption. |
| **Amazon Macie**                   | Uses machine learning to discover, classify, and protect sensitive data in Amazon S3, ensuring data privacy.                                               |
| **AWS KMS (Key Management Service)**| Manages encryption keys to protect sensitive data and model files, ensuring secure data handling and storage.                                               |
| **Amazon GuardDuty**               | A threat detection service that continuously monitors for malicious activity or unauthorized behavior to protect AWS resources.                          |
| **Microsoft Azure**                | Offers tools like **Azure Machine Learning** for secure ML model deployment and **Azure Security Center** for unified security management and threat detection. |
| **Azure Machine Learning**         | Secure ML model development and deployment platform with integrated data encryption, access control, and compliance tools.                               |
| **Azure Sentinel**                 | A cloud-native SIEM (Security Information and Event Management) that provides security monitoring for cloud-based ML services.                            |
| **Google Cloud Platform (GCP)**    | Provides services like **Vertex AI** for model development with secure deployment options such as IAM and VPC service controls.                           |
| **Vertex AI**                      | Offers a unified platform for machine learning model development, deployment, and monitoring, with built-in security features like access control.        |
| **Cloud Security Command Center**  | Provides visibility and security monitoring of GCP resources and workloads to detect vulnerabilities and ensure security across machine learning models.    |
| **DataRobot**                      | An automated machine learning platform that integrates security features like model monitoring, bias detection, and adversarial protection for enterprises. |
| **Databricks**                     | A unified analytics platform that offers end-to-end ML workflows, providing security features like data access controls, encrypted storage, and monitoring. |
| **H2O.ai Driverless AI**           | Automated ML platform offering security against adversarial attacks and ensuring model transparency, explainability, and monitoring.                      |
| **IBM Watson OpenScale**           | Ensures model transparency and trust, offering tools for continuous monitoring of bias, model drift, and adversarial risks with compliance features.        |
| **Aqua Security**                  | Specializes in securing containerized and cloud-native environments, providing vulnerability scanning and runtime security for ML model containers.         |
| **Palo Alto Networks Prisma Cloud**| Provides container and Kubernetes security with vulnerability scanning, configuration auditing, and runtime protection, supporting ML model containers.     |
| **Snyk**                           | A DevSecOps tool that scans for vulnerabilities in code, dependencies, and container images, securing ML deployment pipelines.                              |
| **Immuta**                         | A data governance platform offering fine-grained access controls, dynamic data masking, and compliance features to ensure privacy and security in ML data. |
| **BigID**                          | Helps identify and classify sensitive data to ensure privacy and security compliance in machine learning data handling and usage.                           |
| **Tonic.ai**                       | Provides synthetic data generation tools, preserving data privacy and enabling secure ML model development and testing without using real sensitive data.  |
| **Fiddler AI**                     | A model monitoring and explainability platform that tracks performance, biases, and security risks in deployed machine learning models.                    |
| **Robust Intelligence**            | Focuses on adversarial protection, offering automated testing for vulnerabilities in ML models and securing them against adversarial inputs.                 |
| **Deloitte, PwC, EY (Consulting)** | Offers enterprise-level AI and ML security consulting, including risk assessments, compliance audits, and overall secure AI/ML framework development.        |
| **Accenture**                      | Provides end-to-end digital transformation consulting, integrating security measures into machine learning models and ensuring safe deployment.            |

