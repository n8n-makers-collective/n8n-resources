# Workflows

This folder contains shared **n8n workflow examples** contributed by members of the n8n Makers Collective. The goal is to provide practical, reusable automation patterns that others can import, adapt, and extend.

These workflows are intended to be:

- Real-world use cases, not toy examples  
- Easy to understand and modify  
- Focused on common automation needs  
- Compatible with self-hosted or cloud n8n setups  

---

## 📚 Table of Contents

- ⚙️ [How to Use These Workflows](#%EF%B8%8F-how-to-use-these-workflows)  
- 🤝 [Contributing New Workflows](#-contributing-new-workflows)  
- 🧩 [File Structure Guidelines](#-file-structure-guidelines)  
- 📦 [Available Workflows](#-available-workflows)  

---

## ⚙️ How to Use These Workflows

1. Download the JSON file for the workflow.  
2. In n8n, go to **Workflows → Import from File**.  
3. Upload the JSON file.  
4. Configure credentials and environment-specific settings.  
5. Activate and test.  

Most workflows assume you will need to update:

- Credentials (email providers, APIs, databases)  
- Connection details (hosts, ports, auth)  
- Any organization-specific logic  

---

## 🤝 Contributing New Workflows

To add a workflow:

1. Export your workflow from n8n as JSON.  
2. Place it in this folder.  
3. Add a short description section to this README.  
4. Submit a pull request.  

Recommended contribution guidelines:

- Use clear naming  
- Include only necessary nodes  
- Remove personal credentials  
- Document required setup steps  

---

## 🧩 File Structure Guidelines

Each workflow should include:

- A descriptive filename  
- Clean, readable node names  
- Minimal environment-specific configuration  
- Clear separation of logic steps  

Optional but recommended:

- Comments inside nodes  
- Error handling branches  
- Logging or debugging nodes  

---

## 📦 Available Workflows

### 📨 Store Email Threads in PostgreSQL

**File:** `store-email-threads.json`

#### Overview

This workflow collects email messages, groups them into threads, and stores them in PostgreSQL for future use.

It is designed for teams that want to:

- Preserve email conversations for knowledge management  
- Build AI context or memory systems  
- Enable search, analytics, or summarization workflows  
- Maintain structured communication history  

#### What This Workflow Does

- Retrieves email messages from a configured source  
- Groups messages into threads  
- Normalizes message content  
- Inserts structured data into PostgreSQL  
- Supports long-term storage and downstream automation  

#### Typical Use Cases

- AI agent memory systems  
- Customer support knowledge bases  
- Email analytics pipelines  
- Compliance archiving  
- Automated summarization workflows  

#### Requirements

You will need:

- A configured email integration (IMAP, Gmail, or similar)  
- A PostgreSQL database  
- A table designed to store email thread data  
- n8n database credentials configured  

---

## 🎯 Purpose of This Collection

This folder serves as a shared library of practical automation patterns. Over time, it is expected to grow into a reference set of reusable workflows that help teams accelerate automation, reduce duplication, and support AI-driven processes.

---

*Add more workflows above this line.*
