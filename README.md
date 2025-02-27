# Awesome-MLSecOps

## Table of Contents
- [Industry](#Industry)
- [Open Source Tools](#Open-Source-Tools)
- [Commercial Resources](#Commercial-Resources)
- [Books](#Books)
- [Database](#Database)
- [Blogs and Publications](#Blogs)
- [Community Resources](#Community-Resources)
- [Academic Fields && Academic Resources](#Academic-Fields-&&-Academic-Resources)
- [Concern of Security and Privacy in Data Layer](#Concern-of-Security-and-Privacy-in-Data-Layer)
- [Concern of Security and Privacy in Model Layer](#Concern-of-Security-and-Privacy-in-Model-Layer)
- [Concern of Security and Privacy in APP Layer](#Concern-of-Security-and-Privacy-in-APP-Layer)

## Open Source Tools

| Tool | Description | Risk |
|------|-------------|------|
| [DeepSec](https://github.com/Malmo-Uppdrag/DeepSec) | A framework for evaluating the robustness of machine learning models against adversarial and other security threats. | R9-Security |
| [AIF360](https://github.com/IBM/AIF360) | A library developed by IBM for detecting and mitigating bias in AI models to improve fairness and privacy. | R4-Security |
| [PySyft](https://github.com/OpenMined/PySyft) | A flexible framework for building privacy-preserving machine learning models via federated learning, differential privacy, and encrypted computation. | R1-Privacy, R2-Security |
| [Fairness Indicators](https://github.com/tensorflow/fairness-indicators) | Tools for assessing fairness and biases in machine learning models, focusing on metrics to identify potential risks in data and predictions. | R4-Security |
| [FastGradientMethod](https://github.com/cleverhans-lab/cleverhans) | A part of CleverHans that implements the Fast Gradient Sign Method (FGSM) attack for evaluating and defending against adversarial attacks. | R9-Security |
| [PyAttack](https://github.com/CyberSecurity4ML/PyAttack) | A framework for adversarial machine learning with several attack models that can be applied to a variety of ML models. | R9-Security |
| [WhiteBoxML](https://github.com/ruohan2015/WhiteBoxML) | A framework to test the adversarial robustness of machine learning models through white-box attacks. | R9-Security |
| [FedML](https://github.com/FedML-AI/FedML) | An open-source library for federated learning and privacy-preserving ML models, helping to protect sensitive data across distributed environments. | R1-Privacy |
| [Wit.ai](https://github.com/wit-ai) | A toolkit for building conversational AI that can identify vulnerabilities such as privacy leakage in natural language processing systems. | R2-Privacy, R9-Security |
| [Art of Adversarial Attack](https://github.com/danielgatis/art-of-adversarial-attack) | A set of adversarial attacks and defenses to test model robustness against real-world attacks, including evasion and poisoning. | R9-Security |
| [SecML](https://github.com/UK-MAC/secml) | A machine learning library designed to support secure ML applications, focusing on adversarial training and security. | R9-Security |
| [SafeML](https://github.com/safeml/safeml) | A tool for secure and explainable machine learning that focuses on model transparency and integrity during deployment. | R10-Security |
| [Adversarial Robustness Toolkit](https://github.com/Trusted-AI/adversarial-robustness-toolbox) | A toolkit that provides a variety of attacks and defenses for evaluating adversarial robustness in ML models. | R9-Security, R10-Security |
| [Model Inversion Attack ToolBox](https://github.com/ibm/model-inversion-attack-toolbox) | A framework for implementing model inversion attacks to expose data that was used for model training. | R5-Privacy |
| [Snorkel](https://github.com/snorkel-team/snorkel) | A framework for semi-supervised learning and data augmentation, addressing the risk of data poisoning and mislabeling. | R1-Security, R4-Security |
| [TRIKE](https://github.com/cyberark/trike) | A framework that focuses on security for AI/ML systems by detecting vulnerabilities across ML pipelines. | R5-Security |
| [Adversarial Prompt Injection](https://github.com/fairlearn/adversarial-prompt-injection) | Framework for constructing adversarial prompts for large language models, focusing on prompt injection attacks. | R10-Security |
| [Practical-ML-Security](https://github.com/Practical-ML-Security) | A practical guide to securing machine learning systems with tools, case studies, and mitigation techniques. | R10-Security |
| [Robustness Gym](https://github.com/robustness-gym/robustness-gym) | A toolkit for evaluating the robustness of machine learning models, including performance under adversarial attacks. | R9-Security |
| [Guardrails](https://github.com/NeMo-Guardrails/Guardrails) | A framework for adding guardrails and safety measures in large language model applications. | R10-Security |
| [Shannon's Protector](https://github.com/ShannonProtect/ShannonProtector) | A tool focused on securing machine learning models from backdoor attacks and ensuring robustness during deployment. | R9-Security |
| [Ensemble ML Defense](https://github.com/ensembleml/ensemble-ml) | A tool for building ensemble models that enhance security by combining multiple defensive models against adversarial attacks. | R9-Security |
| [Privacy-Preserving Machine Learning](https://github.com/IBM/privacy-preserving-ml) | A framework for implementing privacy-preserving algorithms, such as federated learning and differential privacy. | R1-Privacy |



## Open Source Privacy Resources


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
