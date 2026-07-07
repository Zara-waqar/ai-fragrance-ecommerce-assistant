# AI Fragrance E-commerce Assistant

This project is an AI-powered assistant built for an online fragrance store using **n8n** and **GPT-5 mini**. The goal was to automate customer support, order management, and payment verification while giving customers a smooth shopping experience through Instagram.

Unlike a traditional chatbot, the assistant can answer product-related questions, recommend perfumes, verify payment screenshots using AI vision, process voice messages, and manage customer orders automatically.

> **Note:** The workflow was built for Instagram integration. The public deployment is currently inactive.

---

## What this assistant can do

- Answer customer questions about products and the brand
- Recommend perfumes based on customer preferences
- Search the product catalog using a Supabase Vector Store (RAG)
- Verify payment screenshots before confirming orders
- Detect incorrect or invalid payment screenshots
- Accept and transcribe voice messages
- Create new orders
- Update existing orders
- Cancel customer orders
- Store order information in Google Sheets
- Send confirmation emails

---

## Technologies Used

- n8n
- GPT-5 mini (OpenAI)
- GPT Vision
- OpenAI Speech-to-Text
- Supabase Vector Store
- Google Sheets
- Gmail
- Instagram
- Tavily API
- HTTP APIs

---

## How the workflow works

The assistant first understands the customer's request.

For product-related questions, it searches the fragrance knowledge base stored in Supabase before generating a response.

If the customer places an order, the assistant collects the required information and stores it in Google Sheets.

When a payment screenshot is uploaded, GPT Vision extracts the payment details from the image. The workflow then checks whether the receiver name, payment amount, transaction date, and reference ID match the expected payment. The order is confirmed only if all required details are valid.

Voice messages are automatically transcribed before being processed by the AI, allowing customers to communicate naturally.

---

## Why I built this project

I wanted to explore how AI agents can automate real e-commerce workflows instead of only answering questions.

This project combines customer support, Retrieval-Augmented Generation (RAG), OCR, AI vision, voice processing, and order management into a single workflow. Building it helped me understand how different AI services can work together to solve real business problems.

---

## Skills Demonstrated

- AI Agent Development
- Workflow Automation
- Prompt Engineering
- Retrieval-Augmented Generation (RAG)
- GPT Vision
- OCR-Based Payment Verification
- Voice AI Integration
- API Integration
- Business Process Automation
- Order Management

---

## Repository Contents

- `workflow.json` – Exported n8n workflow
- `README.md` – Project documentation
- `screenshots/` – Project screenshots
- `architecture/` – Workflow architecture diagram *(coming soon)*

---

## Future Improvements

- Online payment gateway integration
- Inventory management
- Customer order tracking
- Multi-language support
- Customer account management

---

## Author

**Zara Bukhari**

BS Software Engineering Student

Interested in AI Automation, LLM Applications, and Workflow Engineering.
