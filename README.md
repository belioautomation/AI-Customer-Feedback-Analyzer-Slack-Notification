
# 🤖 AI Customer Feedback Analyzer & Slack Notification

<p align="center">
  <strong>AI-powered customer feedback analysis and real-time team notification using Zapier, AI, and Slack.</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Zapier-Automation-FF4A00?style=for-the-badge&logo=zapier&logoColor=white" alt="Zapier">
  <img src="https://img.shields.io/badge/AI-LLM-412991?style=for-the-badge&logo=openai&logoColor=white" alt="AI">
  <img src="https://img.shields.io/badge/Slack-Notifications-4A154B?style=for-the-badge&logo=slack&logoColor=white" alt="Slack">
  <img src="https://img.shields.io/badge/Google%20Sheets-Data%20Source-34A853?style=for-the-badge&logo=google-sheets&logoColor=white" alt="Google Sheets">
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Automation-AI%20Powered-blue?style=flat-square" alt="AI Powered">
  <img src="https://img.shields.io/badge/Workflow-Multi--Step-success?style=flat-square" alt="Multi-Step Workflow">
  <img src="https://img.shields.io/badge/Status-Completed-success?style=flat-square" alt="Status">
</p>

---

## 📌 Project Overview

The **AI Customer Feedback Analyzer & Slack Notification** is an AI-powered workflow automation designed to transform unstructured customer feedback into structured, actionable insights.

The workflow automatically analyzes customer feedback, determines the sentiment, identifies the primary topic, generates a concise summary, and provides a reason for the classification.

The results are then automatically delivered to **Slack**, allowing teams to monitor customer feedback and identify potential issues without manually reviewing every response.

---

## 🎥 Demo

<p align="center">
  <strong>AI Customer Feedback Analysis & Slack Notification</strong>
</p>

https://github.com/belioautomation/AI-Customer-Feedback-Analyzer-Slack-Notification/raw/refs/heads/main/demo.mp4

**Workflow:**  
`Customer Feedback → Zapier → AI Analysis → Sentiment Classification → Slack`

The demo showcases the complete automation, including customer feedback analysis, sentiment classification, and automated Slack notification.

---

## 🎯 Problem

Businesses can receive a large volume of customer feedback through surveys, forms, and other channels.

Manually reviewing every response can be:

- ⏱️ Time-consuming
- 🔁 Repetitive
- 📊 Difficult to scale
- ⚠️ Inconsistent
- 🚨 Slow when identifying negative feedback

### Solution

This automation introduces an AI-powered analysis layer that automatically processes customer feedback and delivers structured insights directly to the team through Slack.

---

## 🔄 Workflow Architecture

```text
┌──────────────────────┐
│  Customer Feedback   │
│    Form / Survey     │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│        Zapier        │
│       Trigger        │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│       AI / LLM       │
│  Feedback Analysis   │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│ Sentiment & Topic    │
│    Classification    │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│   Structured Output  │
│   Summary + Reason   │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│        Slack         │
│  Team Notification   │
└──────────────────────┘
````

---

## ✨ Key Features

### 🧠 AI-Powered Feedback Classification

The AI classifies customer feedback into six categories:

| Classification    | Description                                                      |
| ----------------- | ---------------------------------------------------------------- |
| 🟢 **POSITIVE**   | Customer expresses satisfaction or praise                        |
| 🔴 **NEGATIVE**   | Customer reports dissatisfaction, problems, or complaints        |
| 🟡 **MIXED**      | Customer expresses both positive and negative opinions           |
| ⚪ **NEUTRAL**     | Feedback does not express a clear positive or negative sentiment |
| 🔵 **SUGGESTION** | Customer recommends an improvement or new feature                |
| ❓ **QUESTION**    | Customer is primarily asking a question                          |

### 🏷️ Topic Identification

The AI identifies the primary topic of the feedback, such as:

* App Performance
* User Experience
* Customer Support
* Pricing
* Features
* Bugs
* Account Issues

### 📝 Automatic Summarization

Customer responses are converted into concise summaries that allow teams to quickly understand the issue or opinion.

### 💡 Classification Reason

The AI provides a short explanation for why the feedback was assigned to a particular category.

### 🔔 Slack Notifications

The analyzed feedback is automatically sent to Slack for real-time team visibility.

---

## 🧠 AI Output

The AI is instructed to return structured JSON:

```json
{
  "sentiment": "NEGATIVE",
  "topic": "App Performance",
  "summary": "The customer reported that the app frequently crashes.",
  "reason": "The customer expressed dissatisfaction because of a recurring technical issue."
}
```

Structured output makes the AI response easier to process and map into subsequent automation steps.

---

## 💬 Slack Notification Example

Example notification sent to the team:

```text
📊 NEW CUSTOMER FEEDBACK

Sentiment: 🔴 NEGATIVE
Topic: App Performance

Customer Feedback:
"The app keeps crashing whenever I try to upload photos."

Summary:
Customer reported frequent crashes during photo uploads.

Reason:
The customer is dissatisfied because of a recurring technical issue.
```

---

## 🛠️ Technology Stack

| Technology        | Purpose                               |
| ----------------- | ------------------------------------- |
| **Zapier**        | Workflow automation and orchestration |
| **AI / LLM**      | Feedback analysis and classification  |
| **Slack**         | Real-time team notifications          |
| **Google Sheets** | Feedback data source and storage      |

---

## ⚙️ Workflow Process

### 1. Collect Feedback

A customer submits feedback through the configured form or survey.

### 2. Trigger Zapier

Zapier detects the new response and starts the automation.

### 3. Analyze with AI

The customer feedback is passed to an AI model using a structured analysis prompt.

### 4. Classify Feedback

The AI determines:

* Sentiment
* Topic
* Summary
* Reason

### 5. Process the Result

The structured AI response is mapped into the required fields.

### 6. Notify Slack

Zapier sends the analyzed feedback to the configured Slack channel.

---

## 📈 Business Value

This automation can help businesses:

### Reduce Manual Work

Automates the initial review and categorization of customer feedback.

### Improve Response Time

Important or negative feedback can be surfaced to teams immediately.

### Identify Recurring Issues

Topic classification helps identify common customer problems and trends.

### Scale Feedback Processing

AI allows businesses to process larger volumes of feedback without manually reviewing every response.

### Turn Feedback Into Actionable Insights

Unstructured customer comments are transformed into structured information that teams can use for decision-making.

---

## 🚀 Potential Improvements

Future versions could include:

* 🔴 Automatic escalation of critical complaints
* 🎫 Automatic support ticket creation
* 📧 Email notifications for high-priority feedback
* 📊 Customer sentiment dashboards
* 📈 Weekly or monthly sentiment reports
* 🗂️ CRM integration
* 🧠 Historical sentiment tracking
* 🏷️ Automatic priority scoring
* 🔄 Product-management integration
* 🤖 Automated response suggestions

---

## 🔐 Security & Privacy

This project is intended for portfolio and demonstration purposes.

> **Never commit API keys, authentication tokens, credentials, or private customer information to a public repository.**

Sensitive credentials should be managed through Zapier's secure authentication system or an appropriate secrets-management solution.

---

## 📚 Skills Demonstrated

* AI Workflow Automation
* Zapier
* LLM Integration
* Prompt Engineering
* Sentiment Analysis
* Structured AI Output
* Workflow Design
* Slack Integration
* Data Transformation
* Business Process Automation
* Customer Feedback Analysis
* Automation Architecture

---

## 🎓 Project Purpose

This project was built as part of my ongoing development in **AI Automation and Workflow Development**.

The goal was to create a practical business automation that transforms **unstructured customer feedback into structured insights** and automatically delivers those insights to the appropriate team.

---

## 👨‍💻 Author

**Belio Sinangote**

**AI Automation & Workflow Developer**

Interested in building practical solutions using:

`AI` • `Automation` • `LLMs` • `Zapier` • `n8n` • `APIs` • `Workflow Integration`

---

## 📄 License

This project is available for educational and portfolio purposes.

````
