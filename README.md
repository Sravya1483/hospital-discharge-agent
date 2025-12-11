# 🏥 AI Hospital Discharge Assistant  
Automated hospital discharge workflow built using **IBM watsonx Orchestrate**, **FastAPI**, and **Twilio SMS integration**.  

This system simplifies and accelerates the patient discharge process by automatically generating discharge summaries, validating details through doctor/nurse approval.

---

## 🚀 Features

- **AI-Powered Summary Generation** — Generates professional discharge summaries using IBM watsonx Orchestrate.  
- **Doctor Validation Step** — Human-in-the-loop workflow for medical accuracy and accountability.   
- **Modular Workflow Design** — Each step (form input, AI generation, validation, communication) is implemented as a distinct node in the Orchestrate flow.  

---

## 🧠 System Architecture

IBM watsonx Orchestrate
 Patient Data Form
↓
├── AI Discharge Summary Generator (LLM Node)
├── Doctor/Nurse Review & Approval (Form Node)
└── Twilio Webhook for SMS Notification (Future implementation)
↓
Twilio Messaging API → Patient receives discharge SMS (Idea stage)

## Work flow

Fill out the Patient Data Form (e.g., Typhoid Fever case).

Get the summary generating instructions.

Approve in Nurse Review Form.

Let the AI Discharge Summary Generator create the summary.
