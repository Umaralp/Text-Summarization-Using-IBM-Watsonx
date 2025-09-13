# Generative AI Text Summarization Using IBM Watsonx

This repository contains the assets for a project that demonstrates how to build a powerful text summarization tool using Generative AI on the IBM Watsonx platform.

## 📝 Project Overview

In an era of information overload, quickly understanding the core message of long documents is crucial. This project leverages a large language model to automatically generate concise and accurate summaries of lengthy text, saving time and improving productivity.

## 🎯 The Problem

Manually reading and summarizing articles, reports, and research papers is inefficient and time-consuming. This tool was created to solve that problem by providing instant, high-quality summaries on demand.

## 🛠️ Technology Stack

* **Cloud Platform:** IBM Watsonx.ai [cite: 2]
* **Foundation Model:** `flan-t5-xl-3b` provided by Google [cite: 1, 2]
* **Core Technique:** Few-Shot Prompt Engineering [cite: 2]

## ⚙️ Methodology

The summarization tool was built and configured entirely within the **IBM Watsonx Prompt Lab**[cite: 2].

1.  **Model Selection**: The `flan-t5-xl-3b` model was chosen for its strong capabilities in summarization and other natural language tasks[cite: 1, 2].

2.  **Instruction Prompting**: The model was given a clear role and instruction: "You are a summarization assistant. Summarize the following topic into a short paragraph..."[cite: 2].

3.  **Few-Shot Learning**: To improve accuracy and guide the output style, the model was provided with five examples of high-quality topic-summary pairs[cite: 2]. [cite_start]These examples included topics like Artificial Intelligence, Cybersecurity, and Blockchain[cite: 2].

4.  **Parameter Tuning**: Key model parameters were set to control the output[cite: 2]:
    * **Decoding:** Sampling [cite: 2]
    * **Max Tokens:** 200 [cite: 2]
    * **Min Tokens:** 25 [cite: 2]

## 📊 Results

The configured model was tested with new, unseen text and produced excellent results.

**Test Case: "Cloud Computing"**
* **Input**: A detailed paragraph defining cloud computing, its benefits, major providers, and challenges[cite: 3].
* **Generated Output**: "Cloud computing is the delivery of computing services over the internet. It eliminates the need for companies to invest in expensive hardware and maintenance"[cite: 3].
* **Performance**: The summary was generated in just **1.5 seconds**[cite: 3].

This demonstrates the model's ability to quickly distill a complex topic into its most essential points.

## 🚀 Demo

A brief video demonstrating the summarizer in action can be found in the repository.

🎥 **[Watch the Demo Video (Text Summarization.mp4)](Text%20Summarization.mp4)**

## 📚 Presentation

For a detailed overview of the project, please see the project presentation PDF.

📄 **[View Project Presentation (Text Summarization Using IBM Watsonx.pdf)](Text%20Summarization%20Using%20IBM%20Watsonx.pdf)**
