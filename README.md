# Awesome-MLSecOps

## Table of Contents
- [Industry](Industry)
- [Concern of Security in Data Layer](Concern-of-Security-in-Data-Layer)

## Industry

| Company | Description |
|---------|-------------|
| [ProtectAI](https://protectai.com/) | Security for machine learning models and AI systems. |
| [HiddenLayer](https://hiddenlayer.com/) | The ultimate security platform for AI. |
| [Robust Intelligence](https://www.robustintelligence.com/) | Ensuring AI security and safety to drive enterprise adoption. |
| [CalypsoAI](https://calypsoai.com) | AI security solutions to enable safe innovation. |
| [Lakera](https://www.lakera.ai/) | Real-time security for GenAI applications without performance trade-offs. |

## Concern of Security in Data Layer

- Data Collection (Dynamic Phase)
  - **Description:** Data is gathered from various sources—APIs, sensors, web scraping, user input, etc.
  - **Risks:**
      - **Data Poisoning Attacks:** Attackers inject manipulated or biased data during collection.
      - **Data Fetching Attacks:** Malicious code or hijacked data streams compromise the incoming data in real time.
- Data Preprocessing & Annotation (Dynamic Phase)
  - **Description:** Raw data is cleaned, normalized, and labeled, possibly using both automated processes and human intervention.
  - **Risks:**
      - **Malicious Injection during Preprocessing:** Errors or deliberate manipulations (e.g., mislabeling) can occur as data is transformed.
      - **Annotation Errors:** Intentional or unintentional misannotations can bias the training data.
- Data Storage (Static Phase)
  - **Description:** The preprocessed and annotated data is stored in databases or data warehouses for later use.
  - **Risks:**
      - **Fake Data Attacks:**  The stored dataset might be replaced or corrupted with spurious data.
      - **Incomplete Data Attacks:** Missing or tampered data remains in the repository.
      - **Data Tampering Attacks:** Stored data may be altered after the fact, leading to a compromised dataset.

+ Collection of Academic Papers :
  + 





