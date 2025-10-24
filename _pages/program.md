---
layout: page
permalink: /papers/
title: Accepted papers
nav: true
nav_order: 1
---

## Regular paper

### Robustness Evaluation under RGB-Camera Attacks in CARLA: A Systematic Evaluation of Color Modes and Attack Types

Yufeng Lin (The University of Queensland); Sangmin Park (Korea University); Hyunjae Kang (The University of Queensland); Huy Kang Kim (Korea University); Dan Dongseong Kim (The University of Queensland)

**Abstract.** Abstract
The robustness of YOLOv5-based camera perception for autonomous driving was systematically evaluated under diverse visual perturbations and spectral configurations using the CARLA simulation environment. An agent-camera framework decoupled perception from vehicle control, enabling consistent testing across 20 configurations and 200 trials (104,231 frames) covering four color modes (RGB, red, green, blue) and five perturbation types (salt-and-pepper noise, Gaussian noise, blur, contrast enhancement, baseline). Results revealed counterintuitive robustness patterns: contrast enhancement and green-channel filtering each improved detection by 37%, while salt-and-pepper noise caused an 83% degradation. The optimal combination—red filtering with contrast enhancement—yielded a 42% gain, demonstrating synergistic effects between spectral and photometric factors. However, confidence scores remained nearly constant (0.55-0.65 range) despite large accuracy fluctuations, indicating that confidence-based monitoring fails to reflect true perception reliability. These findings highlight that lightweight spectral filtering and contrast optimization can enhance perception robustness, while safe deployment requires complementary reliability modeling and sensor redundancy to ensure dependable autonomous vision.


### Automated Timeline-Based Forensic Report Generation with Anomaly Detection and LLM-Based CTI Mapping

Yongsik Kim, Saehee Jun, Junho Jang, Huy Kang Kim (Korea University)

**Abstract.**
Diverse vehicle forensics and in-vehicle intrusion detections researches are effectively adopted to the vehicle domain. However, known vehicle forensic researches rarely comprise outputs that are directly usable for investigators; outputs can ideally be auditable, mapped with Cyber Threat Intelligence (CTI), and presented as a timeline-driven incident report. This gap between research outputs and practical requirements creates tangible difficulties in real-world investigations. When forensic analysis fails to yield usable results, investigators must revert to manual spreadsheets and makeshift documents, increasing time and operational costs. Furthermore, even when connections between evidence are established, improper structuring of the attack, such as failing to build a coherent timeline, compromises traceability. To address these challenges of manual analysis and inadequate traceability, we propose a DataBase CAN (DBC)-independent vehicle forensics framework. First, the framework processes raw data by reconciling clocks, normalizing multi-source evidence, and segmenting attacks into episodes using Isolation Forest and change-point detection. Finally, it utilizes a small LLM integrated with the Threat Report ATT&CK Mapper (TRAM) and Automotive Information Sharing and Analysis Center (Auto-ISAC) Automotive Threat Matrix (ATM) to automatically generate CTI-mapped, evidence-linked timeline reports. To demonstrate the robustness and versatility of our framework, we validated it against three diverse public datasets: the VeReMi dataset, the HCRL Car-Hacking dataset, and the OTIDS dataset. Our evaluation focused on three key metrics: timeline fidelity, detection and segmentation quality, and CTI mapping accuracy. The results confirmed that the framework successfully generates systematic reports, organizing observed attacks into evidence-linked timelines with CTI mappings. This approach enhances auditability and traceability, reduces the time to report, and ultimately makes the findings directly actionable for investigators.


### A Self-Synchronizing Cyber Deception Framework via Infrastructure as Code Reflection

Junyeong Park (Undergraduate Student); Sayeon Kim, Woohyun Jang, Yeon-Jae Kim, Shinwoo Shim, Olmi Lee (LIG Nex1 R&D Researcher); Ki-Woong Park (Professor)

**Abstract.**
As cyberattacks become more sophisticated, the use of honeypots has emerged as an alternative to proactively collect attackers’ exploit strategies. However, conventional honeypots often lack realism and require much human effort to deploy and maintain in modern IT infrastructures. This high cost in resources creates a major obstacle to their widespread use. To address these challenges, this paper proposes a self-synchronizing cyber deception framework that upholds the declarative approach of Infrastructure as Code (IaC), maintaining idempotency and consistency while automatically generating a deceptive environment. Our framework treats the target system's IaC files as a blueprint to automatically generate and deploy a high-fidelity, "digital twin" deception environment. Our framework uses an automated pipeline to analyze the IaC file, apply the predefined transformation rules, and dynamically build new container images - replicating structural elements while replacing the core application logic with a honeypot. After deployment, the framework keeps the deceptive environment synchronized with the original system by automatically re-deploying the pipeline in response to any changes in the source IaC file, increasing fidelity and reducing management costs. The implementation of this prototype successfully shows a reduction in the manual effort required for deploying and maintaining deception environments, presenting a scalable and sustainable framework for active defense. This provides a strong foundation for building the next-generation defense mechanisms that can adapt to both evolving cyberattacks and changing infrastructure.

### Automated Vulnerability Repair of Obfuscated and Non-Obfuscated Smart Contracts Using Large Language Models

Chihiro Kado, Tatsuhiro Tsuchiya (The University of Osaka)

**Abstract.**
Recently, automated program repair using large language models (LLMs) has attracted growing attention. In the context of Ethereum smart contracts, where addressing vulnerabilities before deployment is essential, several studies have begun exploring LLM-based vulnerability repair. These studies typically evaluate repair methods on publicly available contracts. However, the effectiveness of LLMs in fixing vulnerabilities in previously unseen contracts remains unclear. To address this question, we applied an obfuscation technique to simulate unknown contracts and used Code Llama – Instruct and GPT-3.5 Turbo to attempt automated repairs. We collected 11 publicly available vulnerable contracts and generated obfuscated versions of each to simulate previously unseen contracts. We then evaluated the performance of the LLMs on both sets. Code Llama – Instruct successfully repaired one original contract and four obfuscated ones. In contrast, GPT-3.5 Turbo correctly fixed seven contracts in each group. These results suggest that LLMs are capable of consistently addressing vulnerabilities in both existing and obfuscated (i.e., simulated unknown) contracts.

### A Study on User Approval Criteria and User Interfaces for Dependability of AI-based Code Generation Tools

Minseo Ju (Department of Software Convergence, Seoul Women’s University); Hyung Kook Jun (ETRI(Electronics and Telecommunications Research Institute)); Taeho Kim (IITP (Institute of Information & Communications Technology Planning & Evaluation); Hyung-Jong Kim (Division of Information Security, Seoul Women’s University)

**Abstract.** AI-based code generation tools significantly enhance development productivity, but the code modifications proposed by generative AI are not always safe or consistent with the intended objectives. Even if AI-based code generation tools perform code modifications based on prompts or user-defined goals, the entity that holds the actual responsibility for the impact of the generated code on users is not the code generation tool itself, but the developer who provides the prompts and goals. Based on this situation, this study considered that the important issue for improving the functionality of dependency assurance in AI-based code generation tools is how to implement human approval and intervention. In this study, we analyzed the traits (features) of AI-generated code, presented them as vectorized values, and designed and implemented an interface that allows developers to make intuitive decisions by visualizing them. When using this tool, developers can utilize additional visualized information during the process of reviewing code changes, allowing them to consider the impact of their decisions while using AI-based code generation tools. The main contribution of this study lies in the conceptual design and implementation of providing visualized importance information of generated code changes to improve the user experience of utilizing code generation tools.


### An approach to creating the optimal attack path based on reinforcement learning

Hyo Sun Lee, Min Geun Song, Huy Kang Kim (Korea University)

**Abstract.** Botnet attacks pose persistent security threats in IoT networks by sequentially infecting devices to create zombie networks for DDoS attacks. Analyzing botnet propagation requires approaches that consider entire system traversal rather than isolated targets. We propose a reinforcement learning-based model that identifies optimal attack paths from an attacker's perspective. Our approach employs Graph Attention Networks (GAT) to analyze network structure and trains using policy gradient techniques to select high-vulnerability nodes during exploration. We implemented a depth-first search algorithm with branch tracking that reflects realistic attacker behavior, evaluating neighbors based on CVSS scores and maximizing cumulative vulnerability scores as rewards. Experimental validation on the UNSW IoT traffic dataset demonstrates effective identification of vulnerability-based attack paths. The model successfully reconstructed network topologies by eliminating non-essential edges while retaining critical paths, providing actionable intelligence for defensive resource allocation. Results show our approach effectively discovers high-risk paths by jointly considering node connectivity and vulnerability scores in realistic IoT environments.


## R&D track

TBD