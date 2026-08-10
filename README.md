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

The **AI Customer Feedback Analyzer & Slack Notification** is an automated workflow designed to transform unstructured customer feedback into actionable insights.

Instead of manually reviewing every customer response, the workflow uses an AI model to analyze the feedback, classify its sentiment, identify the primary topic, generate a concise summary, and explain the classification.

The analyzed result is then automatically delivered to a designated **Slack channel**, allowing teams to monitor customer sentiment and identify potential issues in real time.

---

## 🎯 Problem

Businesses can receive large amounts of customer feedback through forms, surveys, and other channels.

Manually reviewing every response can be:

- ⏱️ Time-consuming
- 🔁 Repetitive
- 📊 Difficult to scale
- ⚠️ Prone to inconsistent classification
- 🚨 Slow when identifying negative feedback

### Solution

This automation introduces an AI-powered processing layer that automatically analyzes incoming feedback and delivers structured insights directly to the team.

---

## 🔄 Workflow Architecture

```text
┌─────────────────────┐
│  Customer Feedback  │
│   Form / Survey     │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│       Zapier        │
│      Trigger        │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│      AI / LLM       │
│  Feedback Analysis  │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│ Sentiment & Topic   │
│    Classification   │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│ Structured Results  │
│ Summary + Reason    │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│        Slack        │
│ Team Notification   │
└─────────────────────┘
````

---

## ✨ Key Features

### 🧠 AI-Powered Sentiment Analysis

Automatically classifies customer feedback into six categories:

| Classification    | Description                                               |
| ----------------- | --------------------------------------------------------- |
| 🟢 **POSITIVE**   | Customer expresses satisfaction or praise                 |
| 🔴 **NEGATIVE**   | Customer reports dissatisfaction, problems, or complaints |
| 🟡 **MIXED**      | Customer expresses both positive and negative opinions    |
| ⚪ **NEUTRAL**     | Feedback is factual or does not express clear sentiment   |
| 🔵 **SUGGESTION** | Customer recommends an improvement or feature             |
| ❓ **QUESTION**    | Customer is primarily asking a question                   |

### 🏷️ Topic Detection

The AI identifies the primary subject of the feedback.

Examples:

* App Performance
* User Experience
* Customer Support
* Pricing
* Features
* Bugs
* Account Issues

### 📝 Automatic Summarization

Long customer responses are converted into concise summaries that are easier for teams to review.

### 💡 Classification Reasoning

The workflow also generates a short explanation describing why the feedback received its classification.

### 🔔 Real-Time Slack Notifications

Analyzed feedback is automatically sent to Slack so teams can respond quickly.

---

## 🧠 AI Output Structure

The AI is instructed to return structured JSON:

```json
{
  "sentiment": "NEGATIVE",
  "topic": "App Performance",
  "summary": "The customer reported that the app frequently crashes.",
  "reason": "The customer expressed dissatisfaction because of a recurring technical issue."
}
```

This structured approach makes the AI output easier to map into downstream automation steps.

---

## 💬 Slack Notification Example

The final Slack notification follows a format similar to:

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

| Technology        | Role                                 |
| ----------------- | ------------------------------------ |
| **Zapier**        | Workflow orchestration               |
| **AI / LLM**      | Feedback analysis and classification |
| **Slack**         | Real-time team notifications         |
| **Google Sheets** | Feedback data source/storage         |

---

## ⚙️ Workflow Steps

### 01 — Capture Customer Feedback

A customer submits feedback through the configured form or survey.

### 02 — Trigger Automation

Zapier detects the new response and starts the workflow.

### 03 — Send Feedback to AI

The customer's response is passed to the AI model with a structured analysis prompt.

### 04 — Classify Feedback

The AI determines the sentiment and identifies the primary topic.

### 05 — Generate Insights

The AI produces:

* Sentiment
* Topic
* Summary
* Reason

### 06 — Notify the Team

Zapier sends the processed result to the configured Slack channel.

---

## 📈 Business Value

This automation can help organizations:

### Reduce Manual Work

Automates the initial review and categorization of customer feedback.

### Improve Response Time

Negative or important feedback can reach the appropriate team immediately.

### Identify Recurring Issues

Topic classification makes it easier to discover common customer problems.

### Scale Feedback Processing

AI can analyze large volumes of feedback without requiring every response to be manually reviewed.

### Create Actionable Insights

Raw customer comments are transformed into structured information that teams can act on.

---

## 🚀 Potential Enhancements

Future versions could extend the workflow with:

* 🔴 Automatic escalation of high-priority complaints
* 🎫 Automatic support ticket creation
* 📧 Email alerts for critical feedback
* 📊 Sentiment dashboards
* 📈 Weekly/monthly sentiment reports
* 🗂️ CRM integration
* 🧠 Historical sentiment tracking
* 🏷️ Automatic priority classification
* 🔄 Product-management integration for feature requests

### Advanced Workflow

```text
Customer Feedback
       │
       ▼
    AI Analysis
       │
       ▼
  Sentiment Router
   ┌───┼────┬────┐
   ▼   ▼    ▼    ▼
Positive Mixed Negative Suggestion
   │   │    │       │
   ▼   ▼    ▼       ▼
 Slack Slack Alert  Product
              │     Team
              ▼
        Support Team
```

---

## 🔐 Security & Privacy

This project is intended for portfolio and demonstration purposes.

> **Never commit API keys, authentication tokens, credentials, or private customer information to a public repository.**

Sensitive information should be stored using Zapier's secure connection system or appropriate secret management solutions.

---

## 📚 Skills Demonstrated

This project demonstrates practical experience with:

* AI workflow automation
* Zapier
* LLM integration
* Prompt engineering
* Sentiment analysis
* Structured AI outputs
* Workflow design
* Slack integration
* Data transformation
* Business process automation
* Customer feedback analysis
* Automation architecture

---

## 🎓 Project Purpose

This project was built as part of my ongoing development in **AI Automation and Workflow Development**, with a focus on applying AI to practical business processes.

The goal is not simply to automate a task, but to design workflows that turn **unstructured information into actionable business insights**.

---

## 👨‍💻 Author

**Belio Sinangote**

AI Automation & Workflow Developer

Interested in building practical solutions using:

`AI` • `Automation` • `LLMs` • `Zapier` • `n8n` • `APIs` • `Workflow Integration`

---

## 📄 License

This project is available for educational and portfolio purposes.

```
```
