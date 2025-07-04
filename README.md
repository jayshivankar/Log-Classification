# 🔍 Log Classification with Hybrid Classification Framework

This project is a flexible and intelligent **log classification system** designed to process and label log messages originating from various software systems. It supports both simple and complex patterns, offering a **hybrid approach** that combines the strengths of multiple classification techniques.

---

## 💡 What the Project Does

- Automatically labels log messages based on their content and source.
- Handles both **structured (predictable)** and **unstructured (free-form)** logs.
- Improves classification accuracy by intelligently switching between different methods.
- Especially useful for logs coming from diverse systems like legacy applications, modern microservices, or third-party APIs.

---

## 🧠 Classification Techniques Used

### 1. **Regular Expression (Regex)**
- Used for logs with predictable, rule-based patterns.
- Fast and interpretable.

### 2. **Sentence Transformer + Logistic Regression**
- Applied when there is enough labeled data.
- Uses deep semantic embeddings from transformers and a logistic regression classifier.

### 3. **LLM (Large Language Models)**
- Handles edge cases and logs where traditional models or regex don't perform well.
- Especially effective for **LegacyCRM** or logs without consistent patterns.

---

## 🏗️ Architecture Overview

![arch](https://github.com/user-attachments/assets/b60e5ea1-e0fe-4901-96e3-ca9dd9a3024c)


---

## ✅ Key Features

- **Hybrid Framework:** Combines traditional rule-based and machine learning methods.
- **Source-Aware:** Adjusts strategy based on the origin of the log message.
- **Plug-and-Play:** Easily integrate your own models, regex rules, or extend to APIs.
- **Scalable:** Designed to work with large datasets and real-time log streams.

---

## 📦 How to Use

1. Place your input CSV with `source` and `log_message` columns in the `resources/` folder.
2. Run the classification script to label each log.
3. Get the output with predicted labels saved to a new file.

---

## 🔗 Applications

- Automated log analysis for DevOps and SRE teams.
- Intelligent alert routing and triaging.
- Log summarization and error pattern detection in large systems.

---

