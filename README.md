🛡️ Threat Intelligence Knowledge Graphs (TiKG)
Entity & Relation Extraction for Cyber Threat Intelligence
<p align="center">
  <b>From Unstructured Threat Reports ➜ Structured Cybersecurity Knowledge Graphs</b>
</p>
<p align="center">
  <img src="https://img.shields.io/badge/Domain-Cybersecurity-blue" />
  <img src="https://img.shields.io/badge/AI-NLP%20%7C%20Knowledge%20Graphs-green" />
  <img src="https://img.shields.io/badge/Journal-Computers%20%26%20Security-red" />
</p>

🌟 Overview
TiKG (Threat Intelligence Knowledge Graphs) is a pipeline-based entity and relation extraction framework designed to transform unstructured cyber threat intelligence (CTI) into structured, machine-readable knowledge graphs.
The framework addresses fundamental challenges in CTI automation, including:


❌ Error propagation in traditional extraction pipelines

❌ Domain ambiguity in generic language models

❌ Noisy entity spans and inconsistent relations

❌ Limited explainability in downstream threat analysis


TiKG enables high-fidelity knowledge graph construction, supporting threat detection, attribution, correlation, and investigation.

📄 Reference (How to Cite)
If you use TiKG, please cite the following peer-reviewed journal paper:
@article{mouiche2025tikg,
  title={Entity and relation extractions for threat intelligence knowledge graphs},
  author={Mouiche, Inoussa and Saad, Sherif},
  journal={Computers \& Security},
  volume={148},
  pages={104120},
  year={2025},
  issn={0167-4048},
  doi={10.1016/j.cose.2024.104120}
}

🔗 DOI: https://doi.org/10.1016/j.cose.2024.104120

🧠 Key Contributions
🔹 Context-Aware Pipeline Architecture
TiKG introduces a security-aware extraction pipeline that integrates:


SecureBERT / SecureBERT⁺ embeddings (cybersecurity-adapted transformers)


Sequential modeling (BiLSTM / BiGRU)


CRF decoding for valid entity boundaries


Ontology-guided error control to reduce cascading extraction errors


🔹 High-Quality Knowledge Graph Construction
Extracted entities and relations are stored as structured triples, enabling:


Threat actor–tool–malware correlation


Campaign attribution


Cross-report reasoning


Query-driven threat investigation



🏗️ Architecture
<p align="center">
  <img src="https://github.com/user-attachments/assets/524ca5ca-21a1-4a96-80d5-4b01ffed1e86" width="90%" />
</p>
Pipeline Flow:


Tokenization & contextual embeddings


Sequence modeling for NER


CRF-based entity decoding


Relation extraction with pooled entity representations


Knowledge graph population



📊 Experimental Validation
TiKG was extensively evaluated across multiple cybersecurity datasets, including:


DNRTI


CyNER


STUCCO


✔️ Key Results


Strong improvements in Precision, Recall, and F1


Robust generalization across heterogeneous CTI sources

Reduced noise propagation compared to baseline pipelines

The table below (from the paper) highlights consistent performance gains across datasets.

<p align="center">
<img width="713" height="169" alt="Image" src="https://github.com/user-attachments/assets/847c4733-17e5-4b96-be40-dbd31196bf83" />

<img width="348" height="113" alt="Image" src="https://github.com/user-attachments/assets/e291d647-7831-484a-ab03-889fca981526" />
</p>

🧩 Sample Knowledge Graph Visualization
<p align="center">
  <img src="https://github.com/user-attachments/assets/5935e04d-fd1c-4096-832f-41bd5a530ced" width="85%" />
</p>

🔍 Example insights enabled by TiKG:


Malware reuse across campaigns


Shared infrastructure among threat actors


Hidden relations not obvious from raw reports



🔧 Use Cases
TiKG supports real-world cybersecurity workflows, including:


🚨 Threat detection & alert enrichment


🕵️ Threat attribution & campaign tracking


📊 Knowledge-driven SOC dashboards


🤖 Automated CTI reasoning & analysis



🌍 Beyond Cybersecurity
While designed for CTI, TiKG is domain-agnostic and transferable to:


🧬 Biomedical text mining


💰 Financial intelligence


🏥 Healthcare analytics


🔐 Safety-critical AI systems



📦 Code & Reproducibility


Sample experiments and configurations are provided


Datasets are publicly available


Extended work (CTiKG) builds on this framework with enhanced context awareness


📩 Questions, collaborations, or industry partnerships are welcome.

👨‍💻 Authors

Inoussa Mouiche:
PhD Candidate, Computer Science
Cybersecurity | AI | ML | Knowledge Graphs

Sherif Saad:
Associate Professor, Computer Science

⭐ If this repository is useful to your work, please star it and cite the paper!
