# Virtual Research Assistant

![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white) ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white) ![Groq API](https://img.shields.io/badge/Groq%20API-000000?style=for-the-badge&logo=api&logoColor=white)

The **Virtual Research Assistant** is an AI-powered tool designed to help researchers quickly find, summarize, and analyze academic papers. By leveraging AI agents, the application automates the process of summarizing research papers and provides detailed advantages and disadvantages for each paper, enabling users to make informed decisions about their relevance.

---

## Table of Contents

- [Overview](#overview)
- [Key Features](#key-features)
- [Technical Stack](#technical-stack)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

---

## Overview

The Virtual Research Assistant streamlines the research process by:
1. Fetching relevant research papers from sources like **ArXiv** (and optionally **Google Scholar**).
2. Generating concise summaries of the papers using an AI-powered **Summarizer Agent**.
3. Analyzing the summarized content to provide a pointwise list of **advantages** and **disadvantages** using another AI agent.

The application is built using **Streamlit** for the front-end interface and integrates with **Groq API** for AI-driven summarization and analysis.

---

## Key Features

- **AI-Powered Summarization**: Automatically generates concise summaries of research papers using the **Llama-3.3-70b-versatile** model via Groq API.
- **Advantages & Disadvantages Analysis**: Provides a detailed pointwise list of pros and cons for each paper.
- **Dynamic Search Expansion**: If fewer than 5 papers are found, the system suggests related topics and expands the search to ensure diverse results.
- **Multi-Source Data Fetching**: Fetches papers from **ArXiv** and optionally from **Google Scholar**.
- **Interactive UI**: Built using **Streamlit**, the web interface allows users to input research topics and view processed results in real-time.

---

## Technical Stack

- **Programming Languages**: Python
- **Frameworks/Libraries**:
  - **Streamlit**: For building the interactive front-end UI.
  - **Autogen**: For creating and managing AI agents.
  - **Requests** and **xml.etree.ElementTree**: For interacting with the ArXiv API.
  - **Scholarly**: For fetching data from Google Scholar.
  - **dotenv**: For managing environment variables.
- **AI Models**: Groq API with Llama-3.3-70b-versatile model.
- **APIs**: ArXiv API, Groq API.

---

## Installation

### Prerequisites

- Python 3.8 or higher
- Install required dependencies using `pip`:

```bash
pip install -r requirements.txt
```

### Environment Variables

Create a `.env` file in the root directory. Add your Groq API Key to the `.env` file:

```env
GROQ_API_KEY=your_groq_api_key_here
```

### Running the Application

Clone the repository:

```bash
git clone https://github.com/yourusername/virtual-research-assistant.git
cd virtual-research-assistant
```

Run the Streamlit app:

```bash
streamlit run app.py
```

Open the provided URL in your browser to access the application.