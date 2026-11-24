# Hi, I'm Salvatore Francesco Tartaglione 👋

**MSc student in Computer Engineering (Artificial Intelligence) at the University of Salerno**, graduating in March 2027.
I build and evaluate machine learning systems across **LLM applications**, **computer vision**, and **trustworthy / secure AI**.

🔎 **Looking for AI / ML Engineer roles in Europe** (EU citizen, open to relocation).

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Salvatore%20Francesco%20Tartaglione-0A66C2?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/salvatore-francesco-tartaglione-06004933b/)
[![Email](https://img.shields.io/badge/Email-salvatorefrancesco2015%40outlook.com-D14836?logo=microsoftoutlook&logoColor=white)](mailto:salvatorefrancesco2015@outlook.com)

---

## What I focus on

- **LLM applications:** agentic RAG with hybrid retrieval, re-ranking and measurable evaluation (RAGAS).
- **Computer vision:** detection, multi-object tracking, semantic segmentation, face recognition, generative models.
- **Robustness and security of ML:** adversarial attacks and defenses, liveness (replay-attack) detection.
- **Engineering habits:** leakage-aware data splits, honest reporting of limitations, automated tests, reproducible pipelines.

---

## ⭐ Featured AI projects

### 🤖 [DIEM Assistant: hybrid agentic RAG](https://github.com/SalvatoreFTartaglione/DIEM-Assistant-RAG)
`Python` `LangGraph` `ChromaDB` `BM25` `Chainlit` `RAGAS`

A conversational assistant that answers students' questions about a university department using only official sources, with inline citations.
- Custom crawler over 4 university portals and linked PDFs, deduplication and parent-child chunking.
- LangGraph agent: domain guardrail, query rewriting, hybrid dense + dual BM25 retrieval fused with Reciprocal Rank Fusion, cross-encoder re-ranking.
- Evaluated on a 62-question benchmark with RAGAS: **context recall 0.85, faithfulness 0.76**.

### ⚽ [Soccer player tracking](https://github.com/SalvatoreFTartaglione/soccer-player-tracking)
`PyTorch` `YOLO11` `BoT-SORT` `OSNet`

End-to-end pipeline that detects and tracks every player and referee in 1080p broadcast footage, keeping consistent IDs despite camera motion and occlusions.
- YOLO11-L fine-tuned on SoccerNet: **mAP@50 0.979**; fine-tuned OSNet re-ID: **rank-1 97.5%**.
- BoT-SORT with camera-motion compensation and offline tracklet stitching; counts players inside pitch regions.
- **HOTA@0.5 of 67.5%** on the 49-sequence SoccerNet test split.

### 🛡️ [Adversarial attacks on face recognition](https://github.com/SalvatoreFTartaglione/adversarial-face-recognition)
`PyTorch` `Adversarial Robustness Toolbox` `facenet-pytorch`

Security evaluation of a face-recognition access-control system.
- FGSM, BIM, PGD, Carlini-Wagner and DeepFool against a VGGFace2 FaceNet model: accuracy dropped from 85.1% to **2.6%** under PGD at ε = 0.01; transferability studied on a ResNet-50.
- Defenses: JPEG pre-processing and an EfficientNet-B0 adversarial detector (**AUROC 0.991**, blocks **96.1%** of attacks).
- Command-line tool and 71 automated tests.

### 🪪 [Face recognition attendance system](https://github.com/SalvatoreFTartaglione/face-recognition-attendance-system)
`PyTorch` `MTCNN` `InceptionResnetV1` `MobileNetV2` `MagFace`

Replaces badge-based attendance with face recognition on smartphone pictures, robust to replay attacks.
- Pipeline: MTCNN detection → MobileNetV2 liveness check → MagFace quality gate → identification and verification.
- On a custom 20-subject dataset: **99.17% rank-1 identification**, verification **FAR 0.21% / FRR 2.29%**, **100% liveness accuracy** on screen-replay attacks.

### 🚗 [Off-road semantic segmentation](https://github.com/SalvatoreFTartaglione/off-road-semantic-segmentation)
`PyTorch` `Albumentations`

Pixel-wise segmentation of rural-road camera frames into 8 classes, with a focus on trustworthy evaluation.
- U-Net with ImageNet-pretrained ResNet18 encoder; class-weighted cross-entropy + Dice loss.
- Leakage-aware block split of highly correlated frames and a re-implementation of the official metric.
- **0.51** on the official per-image IoU metric (145 test images); 206 automated tests.

---

## More projects

| Project | Area | What it is | Stack |
|---|---|---|---|
| [Conditional face generation](https://github.com/SalvatoreFTartaglione/conditional-face-generation) | Generative AI | Conditional VAE, DCGAN and autoregressive Mamba model written from scratch on CelebA (202k images), conditioned on 3 attributes and compared qualitatively | PyTorch |
| [TORCS behavioral cloning](https://github.com/SalvatoreFTartaglione/TORCS-behavioral-cloning) | Imitation learning | Autonomous driver for the TORCS simulator: a k-NN classifier imitates human keyboard driving from 21,243 recorded samples (22 sensor features), with recovery routines for off-track and stuck cars | Java |
| [Erasmus credential sharing](https://github.com/SalvatoreFTartaglione/erasmus-credential-sharing) | Security | Privacy-preserving verifiable credentials with selective disclosure (W3C VCs, DIDs, salted Merkle trees, X.509) on a simulated ledger; 84 tests including six simulated attacks | Python |
| [Smart Home Manager](https://github.com/SalvatoreFTartaglione/smart-home-manager) | Mobile app | Cross-platform Flutter app to monitor and control a smart home; I built the SQLite data layer, security and automation pages, push notifications, tests and CI (49 tests, GitHub Actions) | Flutter, Dart |
| [Paint](https://github.com/SalvatoreFTartaglione/paint) | Software engineering | JavaFX vector drawing tool built by a team of four in 3 sprints; I was Scrum Master. MVC and Command, Factory, Singleton, Observer patterns, 300+ unit tests | Java |

---

## Tech stack

| | |
|---|---|
| **Languages** | Python · Java · SQL · R  |
| **Deep learning & vision** | PyTorch · Ultralytics YOLO · OpenCV · Albumentations · facenet-pytorch · Torchreid · BoxMOT · Adversarial Robustness Toolbox |
| **LLM & NLP** | LangGraph · LangChain · ChromaDB · BM25 · RAGAS · Hugging Face · spaCy · Ollama |
| **Engineering** | Git · GitHub Actions · pytest · JUnit · Maven · Flutter · REST APIs · Scrum |
| **Security & crypto** | Adversarial ML · PKI / X.509 · Merkle trees · digital signatures |

---

## Background

- 🎓 **MSc in Computer Engineering, AI Applications track**, University of Salerno, expected March 2027
- 🎓 **BSc in Computer Engineering**, University of Salerno, 108/110
- 💼 **Intern (BSc thesis project)**, Rebitral S.r.l.: IoT system on Raspberry Pi with text-to-speech, REST API and telemetry monitoring
- 🌍 Italian (native), English (B2)

---

*Most projects were developed for university courses; each repository documents its results and known limitations.*
