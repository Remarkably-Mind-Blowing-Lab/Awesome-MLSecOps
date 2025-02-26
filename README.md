# Awesome-MLSecOps

## Table of Contents
- [Industry](#Industry)
- [Concern of Security in Data Layer](#Concern-of-Security-in-Data-Layer)
- [Open Source Security Resources in Data Layer](#Open-Source-Security-Resources-in-Data-Layer)

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
    


