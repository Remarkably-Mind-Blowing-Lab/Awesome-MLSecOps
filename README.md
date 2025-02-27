# Awesome-MLSecOps

## Table of Contents
- [Introduction to MLSecOps](#Introduction-to-MLSecOps)
- [Security & Privacy Considerations in ML](#Security-&-Privacy-Considerations-in-ML)
- [MLSecOps Phases](#MLSecOps-Phases)
  - [Concern of Security and Privacy in Data Layer](#Concern-of-Security-and-Privacy-in-Data-Layer)
  - [Concern of Security and Privacy in Model Layer](#Concern-of-Security-and-Privacy-in-Model-Layer)
  - [Concern of Security and Privacy in Application Layer](#Concern-of-Security-and-Privacy-in-Application-Layer)
- [Security Tools & Resources](#Security-Tools-&-Resources)
  - [Open Source Tools](#Open-Source-Tools)
  - [Commercial Resources](#Commercial-Resources)
  - [Books](#Books)
  - [Database](#Database)
  - [Blogs and Publications](#Blogs-and-Publications)
  - [Community Resources](#Community-Resources)
- [MLOps Infrastructure & DevSecOps](#MLOps-Infrastructure-&-DevSecOps)
- [Community Contributions & Development](#Community-Contributions-&-Development)
- [Academic Fields & Academic Resources](#Academic-Fields-&-Academic-Resources)

## Security Tools & Resources

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








## Industry

| Company | Description |
|---------|-------------|
| [ProtectAI](https://protectai.com/) | Security for machine learning models and AI systems. | 
| [HiddenLayer](https://hiddenlayer.com/) | The ultimate security platform for AI. |
| [Robust Intelligence](https://www.robustintelligence.com/) | Ensuring AI security and safety to drive enterprise adoption. |
| [CalypsoAI](https://calypsoai.com) | AI security solutions to enable safe innovation. |
| [Lakera](https://www.lakera.ai/) | Real-time security for GenAI applications without performance trade-offs. |

## Concern of Security and Privacy in Data Layer

- **Data Collection (Dynamic Phase)**
  - **Description:** Data is gathered from various sources—APIs, sensors, web scraping, user input, etc.
  - **Risks:**
      - **Data Poisoning Attacks:** Attackers inject manipulated or biased data during collection. **(R1-Security)**
      - **Data Fetching Attacks:** Malicious code or hijacked data streams compromise the incoming data in real time. **(R2-Security)**
      - **Unauthorized PII Collection:** Collecting Personally Identifiable Information (PII) or sensitive data (e.g., financial, health records) without proper anonymization or consent can lead to privacy breaches. **(R1-Privacy)**
- **Data Preprocessing & Annotation (Dynamic Phase)**
  - **Description:** Raw data is cleaned, normalized, and labeled, possibly using both automated processes and human intervention.
  - **Risks:**
      - **Malicious Injection during Preprocessing:** Errors or deliberate manipulations (e.g., mislabeling) can occur as data is transformed. **(R3-Security)**
      - **Annotation Errors:** Intentional or unintentional misannotations can bias the training data. **(R4-Security)**
      - **PII Leakage:** During data cleaning, transformation, or labeling, sensitive details might inadvertently be exposed or improperly anonymized. **(R2-Privacy)**
      - **Unsecured Data Transfer Exposure:** During the transfer of data between systems or over networks, unencrypted channels may expose sensitive information. **(R3-Privacy)**
- **Data Storage (Static Phase)**
  - **Description:** The preprocessed and annotated data is stored in databases or data warehouses for later use.
  - **Risks:**
      - **Fake Data Attacks:**  The stored dataset might be replaced or corrupted with spurious data. **(R5-Security)**
      - **Incomplete Data Attacks:** Missing or tampered data remains in the repository. **(R6-Security)**
      - **Data Tampering Attacks:** Stored data may be altered after the fact, leading to a compromised dataset. **(R7-Security)**
      - **Sensitive Data Exposure:** Stored datasets that include sensitive information become attractive targets for unauthorized access or leakage. **(R4-Privacy)**
      
## Concern of Security and Privacy in Model Layer

- **Model Training & Development (Dynamic Phase)**  
  - **Description:** Machine learning models are trained using the preprocessed data. This phase involves iterative training, hyperparameter tuning, and validation.
  - **Risks:**
    - **Bias & Jailbreak Risks:** Training on biased data or adversarial inputs that cause the model to behave unexpectedly. **(R8-Security)**  
    - **Adversarial Attacks:** During training, adversarial examples might be introduced to degrade model performance. **(R9-Security)**  
    - **Backdoor Attacks:** Hidden triggers are embedded during training to activate malicious behavior during inference. **(R10-Security)**
    - **Unintentional Data Memorization:** Without incorporating privacy-preserving techniques (e.g., differential privacy), models may leak information via model inversion or membership inference attacks. **(R5-Privacy)**

- **Model Storage & Management (Static Phase)**  
  - **Description:** After training, the finalized model—including its weights and configurations—is saved as a static artifact (e.g., model files, container images).
  - **Risks:**
    - **Fake Model Attacks:** The saved model might be replaced with a malicious version. **(R11-Security)**  
    - **Incomplete Model Artifacts:** Missing parameters or weights can compromise the model’s integrity. **(R12-Security)**  
    - **Model Tampering:** Post-training modifications (e.g., unauthorized changes to model weights) that alter intended behavior. **(R13-Security)**

- **Model Deployment & Containerization (Static & Dynamic Phase)**  
  - **Description:** The model is deployed to production, often within a containerized environment. This includes setting up APIs, load balancers, and runtime environments.
  - **Risks:**
    - **Container Image Vulnerabilities:** Insecure container configurations or pre-built images that contain vulnerabilities. **(R14-Security)**  
    - **Static Configuration Errors:** Faulty configuration files or environment settings that are baked into the deployment. **(R15-Security)**  
    - **Container Runtime Attacks:** Active exploitation such as container escapes or runtime virus attacks. **(R16-Security)**  
    - **API Abuse & Injection:** Real-time attacks on the deployment endpoint, exploiting weaknesses in API security. **(R17-Security)**
    - **Sensitive Pattern Extraction:** Even if the model itself appears secure, it might reveal sensitive patterns or individual data points through carefully crafted queries. **(R6-Privacy)**  
    - **Unauthorized Model Extraction:** Improper access control to the model files could enable unauthorized extraction of underlying sensitive features. **(R7-Privacy)**  
    
## Concern of Security and Privacy in APP Layer

- **Model Optimization & Integration (Dynamic Phase)**  
  - **Description:** The deployed model is further optimized for performance (e.g., via quantization, pruning, or transfer learning) and integrated into the application.
  - **Risks:**
    - **Quantization Attacks:** Exploiting the optimization process (e.g., precision loss) to manipulate model behavior. **(R18-Security)**  
    - **Model Transfer Attacks:** During model migration or integration, attackers could extract or tamper with model parameters dynamically. **(R19-Security)**  
    - **Insecure Data Management:** Insecure APIs, unencrypted data storage in the application, or flawed session management can expose user data. **(R8-Privacy)**  

- **Application Development & Code Integration (Static Phase)**  
  - **Description:** The application code (front-end/back-end) that leverages the model is developed, reviewed, and deployed.
  - **Risks:**
    - **Code Vulnerability Attacks:** Pre-existing vulnerabilities in the application code (e.g., remote code execution, SQL injection, XSS) which become a fixed risk if not patched. **(R20-Security)**  
    - **Insecure API Integration:** Static misconfigurations in API usage or credentials that can be exploited. **(R21-Security)**  
    - **Sensitive Log Exposure:** If logs are not sanitized or securely stored, they can become a vector for privacy breaches. **(R9-Privacy)**  
- **Service Exposure & Runtime Monitoring (Dynamic Phase)**  
  - **Description:** The final application, which includes the optimized model and integrated code, is exposed to end-users. It is actively monitored in a live environment.
  - **Risks:**
    - **Runtime Exploitation:** Attacks during API calls, including DDoS or injection attacks that occur on-the-fly. **(R22-Security)**  
    - **Anomalous Behavior Detection:** Dynamic monitoring may reveal unusual patterns (e.g., sudden spikes in traffic, unexpected model outputs) indicative of ongoing attacks. **(R23-Security)**  
    - **Unvetted Data Collection:** Third-party components may collect or transmit user data without adequate consent or security measures. **(R10-Privacy)**  
    - **Side-Channel Data Leaks:** Inference through aggregate statistics or error messages could expose individual data details. **(R11-Privacy)**  
