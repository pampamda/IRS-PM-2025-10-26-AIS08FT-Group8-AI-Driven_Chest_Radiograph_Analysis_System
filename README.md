---

## SECTION 1: PROJECT TITLE

## AI-Driven_Chest_Radiograph_Analysis_System

---

## SECTION 2 : EXECUTIVE SUMMARY / PAPER ABSTRACT

 This project develops an AI-driven chest radiograph analysis system to address radiologist shortages, diagnostic delays, and accessibility gaps in healthcare ecosystem. The core goal is to automate the detection of 14 thoracic pathologies (e.g., pneumonia, pleural effusion) and generate structured, clinically plausible reports for both clinicians and patients. The system integrates two classification models (federated Chex model and centralized Pathology model, both based on DenseNet121), two fine-tuned multimodal LLaVA models (LLaVA-4B and LLaVA-7B via LoRA), and a Retrieval-Augmented Generation (RAG) module—complemented by GLM-4V API integration—to balance accuracy, interpretability, and scalability.

Key results confirm the system’s effectiveness: the DenseNet121-based classifiers achieve a macro-averaged AUROC of 0.8245, while the hybrid CheXpert+Wiki RAG configuration outperforms baselines with a human evaluation score of 4.5/5 and RadGraph F1 of 58.7%. The fine-tuned LLaVA models generate coherent structured reports, and the full-stack deployment (React frontend, FastAPI backend, Colab-based inference) enables end-to-end image upload, analysis, and report delivery. This solution enhances diagnostic efficiency, reduces turnaround time, and expands access to expert-level support for community clinics and regional settings.

---

## SECTION 3 : CREDITS / PROJECT CONTRIBUTION

| Official Full Name  | Student ID (MTech Applicable)  | Work Items | Email (Optional) |
| :------------ |:---------------:| :-----| :-----|
| Gu ShuoHan | A0327973X | Pathology model |  |
| Pan Linyu | A0329069U | LLaVA-7b model |  |
| Wang Siwei | A0329955L | Chex model |  |
| Yang Minyue | A0329709R | LLaVA-4b model |  |
| Yang Ziyu | A0326794N | GLM-4V+RAG     |  |

---

## SECTION 4 : VIDEO OF SYSTEM MODELLING & USE CASE DEMO

`Refer to videos in project report at Github Folder: Video`

---

## SECTION 5 : USER GUIDE

`Refer to appendix <Installation & User Guide> in project report at Github Folder: ProjectReport`

### [ 1 ]  Backend Installation

> cd Chexpert_back
>
> python -m venv venv
>
> venv\Scripts\activate
>
> pip install -r requirements.txt
>
> uvicorn app.main:app --reload --host 0.0.0.0 --port 8000

### [ 2 ] Frontend Installation
> cd Chexpert_front
>
> npm install
>
> npm start

---
## SECTION 6 : PROJECT REPORT / PAPER

`Refer to project report at Github Folder: ProjectReport`

---

## SECTION 7 : MISCELLANEOUS

`Refer to Github Folder: Miscellaneous`