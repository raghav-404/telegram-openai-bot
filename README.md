# 🤖 Telegram + OpenAI Bot (n8n Workflow)

Welcome to the **Telegram OpenAI Bot**, a powerful and easy-to-deploy chatbot powered by **OpenAI GPT-4.1-mini** and managed through the visual automation tool **n8n**.

> 🚀 This workflow allows you to connect Telegram and OpenAI in a seamless conversation loop using no-code!

---

## ✨ Features

✅ **Telegram Integration** – Automatically triggers on new Telegram messages  
🧠 **AI-Powered Responses** – Uses GPT-4.1-mini to generate intelligent replies  
🛠️ **No-Code Setup** – Fully managed in n8n  
🔁 **Bi-directional Messaging** – Replies to users in real time  
📦 **Customizable** – Modify logic, prompts, and AI behavior easily

---

## 🔁 Workflow Overview

| 🔢 Step | 🧩 Node                 | 🔍 Description                                        |
|--------:|-------------------------|--------------------------------------------------------|
| 1       | **Telegram Trigger**    | Listens for incoming messages from Telegram            |
| 2       | **AI Agent**            | Processes input and formats a prompt for OpenAI        |
| 3       | **OpenAI Chat Model**   | Calls `gpt-4.1-mini` to generate a conversational reply |
| 4       | **Send Text Message**   | Sends the reply back to the Telegram user              |

---

## 🧠 Workflow Structure

```mermaid
graph TD
    A[📩 Telegram Message] --> B[🧠 AI Agent]
    B --> C[🧬 GPT-4.1-mini via OpenAI API]
    C --> D[📤 Reply to Telegram User]
