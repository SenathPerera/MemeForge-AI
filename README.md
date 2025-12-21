# MemeForge AI 🗿
![MemeForge AI Banner](https://github.com/SenathPerera/MemeForge-AI/blob/main/MemeForge%20AI%20Banner.png)
**MemeForge-AI** is an open-source AI-powered meme generator designed to create, customize, and share memes easily. It combines natural language processing (NLP), caption generation, and user-friendly interfaces to provide a seamless meme creation experience.<br/>

At its core, the system is driven by four specialized agents, each responsible for a key step in the meme creation pipeline:

### 1. Meme Idea Agent
Understands the user prompt, extracts context, and generates witty and relevant meme captions.<br/>
Uses OpenAI and Grok APIs for caption generation.

### 2. Template Retrieval Agent
Fetches meme templates from multiple sources:
- Imgflip API
- Memegen API
- Reddit API<br/>

It builds a pool of template candidates, embeds both template names and the user prompt into vectors, and uses cosine similarity to select the top 6 most relevant templates.

### 3. Security Compliance Agent
Ensures the safety and appropriateness of generated captions and retrieved templates.<br/>
NSFW, offensive, or unsafe content is filtered out by default.<br/>
Users can optionally disable the safety filter, in which case the system bypasses security checks.<br/>

### 4. Meme Generator Agent
Combines the selected caption and meme template to produce the final AI-generated meme image.<br/>
This project demonstrates end-to-end integration of LLMs, information retrieval, API fusion, and content safety mechanisms, all wrapped into a smooth meme-generation experience.

# System Architecture
![System Architecture](https://github.com/SenathPerera/MemeForge-AI/blob/main/System%20Architecture.gif)

# Project Structure
```
Meme-Generator-AI/
├── data/              # Datasets, seed images, captions, or meme templates
├── docs/              # Documentation, notes, and guides
├── frontend/          # Web interface for user interaction
├── outputs/           # Generated memes and results
├── src/               # Core source code: AI pipelines, model logic, backend scripts
├── tests/             # Unit and integration tests
├── requirements.txt   # Python dependencies
└── .gitignore         # Files and directories to be ignored by Git
```
# Features
- AI Meme Generation: Generates memes based on user input using advanced AI techniques.
- Template Retrieval: Selects appropriate meme templates from a curated dataset.
- Text Generation: Suggests witty captions using NLP models.
- Security & Compliance: Ensures content adheres to ethical guidelines and avoids offensive material.
- User-Friendly Interface: Web-based front end for easy meme creation without coding knowledge.
- Output Storage: All generated memes are saved for easy access and sharing.

## Installation & Setup
**1. Clone the repository**
```
git clone https://github.com/SenathPerera/MemeForge-AI.git
```
**2. Install dependencies**</br>
```
pip install -r requirements.txt
```
**3. Launch backend**
```
activate .venv - & <Your folder path to Meme-Generator-2\.venv\Scripts\Activate.ps1>
python -m uvicorn src.main:app --reload
```
**4. Launch frontend**
```
npm start
```

# Authors
<a href="https://github.com/SenathPerera/MemeForge-AI/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=SenathPerera/MemeForge-AI" />
</a>
