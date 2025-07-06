# 📧 Cold Email Generator

A streamlined AI-powered cold outreach tool built using **Groq**, **LangChain**, and **Streamlit**. This application automates the generation of personalized cold emails for service-based companies targeting job postings.

Given a company's **careers page URL**, the tool:
- Extracts active **job listings** using web scraping.
- Analyzes job descriptions with **LLM inference via Groq API**.
- Retrieves matching **portfolio links** from a **ChromaDB vector store**.
- Crafts context-aware cold emails tailored to each job role.

This significantly reduces manual outreach efforts for business development teams by aligning service capabilities with open job requirements at scale.

---

## 💡 Use Case Example
> Atliq, a software service provider, wants to offer its engineers to Nike, which has an open role for a Principal Software Engineer. Using this tool, Atliq’s executive can auto-generate a targeted cold email referencing Nike’s job post and Atliq’s relevant work portfolio.

---

## ⚙️ Tech Stack
- **Groq LPU** for high-speed inference on LLM prompts  
- **LangChain** for prompt chaining and memory  
- **ChromaDB** as the vector database for portfolio-document similarity matching  
- **Streamlit** for a simple, interactive UI  

---

## 🧩 Architecture
![Architecture Diagram](imgs/architecture.png)

---

## 🚀 Setup Instructions

1. **Add your Groq API key** to the `.env` file:
   ```env
   GROQ_API_KEY=your_api_key_here
   ```

2. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Streamlit app**:
   ```bash
   streamlit run app/main.py
   ```

---

This project showcases seamless integration between modern LLM infrastructure and real-world business automation workflows — ideal for startups and agencies focused on outbound lead generation.
