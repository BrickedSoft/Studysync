<p align="center">
  <img src="https://github.com/user-attachments/assets/c68c1c9b-d6c1-43b0-b361-0fbf04d00c75" width="20%" alt="STUDYSYNC">
</p>

<p align="center">
    <em>This is the repository for Studysync project combining all parts of it.</em>
</p>
<p align="center">
  <img src="https://img.shields.io/github/last-commit/BrickedSoft/Studysync?style=default&logo=git&logoColor=white&color=0080ff" alt="last-commit">
  <img src="https://img.shields.io/github/languages/top/yashrif/study-sync-client?style=default&color=0080ff" alt="repo-top-language">
  <img src="https://img.shields.io/github/languages/top/jahidem/studysync-ai?style=default&color=0080ff" alt="repo-top-language">
  <img src="https://img.shields.io/github/languages/top/yashrif/study-sync-server?style=default&color=0080ff" alt="repo-top-language">
</p>


#####  Table of Contents

- [ Overview](#overview)
- [ Features](#features)
- [ Project Structure](#project-structure)
- [ Technology Stack](#technology-stack)
- [ Getting Started](#getting-started)
    - [ Prerequisites](#prerequisites)
    - [ Installation](#installation)
    - [ Usage](#usage)
- [ Contributors](#contributors)


##  Overview

**StudySync** is a digital platform designed to streamline and enhance the study process with the help of AI. It offers students a complete suite of features, from loading study materials to creating personalized study plans, tracking progress, and conducting self-evaluation. Leveraging AI-assisted technologies, StudySync helps generate questions, summarize content, create study plans (e.g., GROW method), and provide interactive features like flashcards and multiple-choice questions (MCQs).


##  Features
### 1. Organized Study Content
- **Content Uploading:** upload your study contents right in Studysync with intuitive interface. Also find, sort and manage your contents as needed.
- **Index Content:** Content is indexed into our vector database Qdrant on demand, so the Generative AI can have full context of it where needed.

### 2. Progress Tracking
- **Practice Statistics:** Studysync home tab offers an overview of how much Flashcards review, and acquired proficiency of generated CQ and MCQ.
- **Study Plan Progress:** Get an idea of overall progress for study plans at a glance with our intuitive activity graphs.

### 5. AI-Assisted Study
- **Integrated PDF Reader & Annotation:** Open and read your study materials directly within the application. With full PDF annotation and marking features powered by PSPDFKit, you can highlight, add notes, and reference key sections for a more interactive and organized study experience.

- **AI-Enhanced Explanation & Examples:** Select any portion of text from the opened PDF and use Generative AI to explain difficult concepts or provide examples, helping you deepen your understanding of the material.

- **Context-Aware Q&A:** The Generative AI has full context of the opened study content. You can ask questions related to the topics within the document, and it will provide answers aligned with the content you’re studying. This is achieved through Retrieval-Augmented Generation (RAG), ensuring accurate and relevant responses based on your current study material.

### 4. AI-Assisted Self Evaluation
- **Question Generation:** Instantly generate questions from uploaded documents, slides, or PDFs using Generative AI. Choose between MCQ or CQ formats and save them for future practice. Test your understanding by answering these questions and receive evaluations to identify areas for improvement.
- **Flashcards:** When you're too fatigued to keep reading, generate flashcards with a single tap to review key concepts. Use these flashcards to reinforce your comprehension.

### 5. AI-Assisted Planning
- **GROW Method:** Leverage AI to automatically generate a list of topics from your selected study content. You can adjust or refine the suggested topics as needed before creating a personalized GROW study plan. Track your progress daily by marking your understanding of each topic, with a visual indicator transitioning from red (low comprehension) to yellow and green (full comprehension). This integrated approach allows you to plan and execute your study strategy simultaneously, providing a highly effective method for mastering your material.

### 6. AI-Assisted Content Generation

- **AI-Generated Learning Material:** Explore topics beyond your existing study materials by generating AI-assisted content on any given subject. This feature allows you to broaden your knowledge base and access additional learning resources directly within the application.

- **Interactive AI Chat:** A chat bubble located at the bottom-right corner of the application enables real-time interaction with Generative AI providing on-demand assistance while studying.

### 7. Slash Command Integration

- **Generate MCQs and CQs with Slash Commands:** StudySync features slash command functionality, allowing you to generate multiple-choice questions (MCQs) and conceptual questions (CQs) directly within the chat interface. Simply use the specified slash commands to instantly create questions based on your study content, making it easier to engage with and evaluate your understanding during study sessions.

##  Project Structure

```sh
└── Studysync
    ├── study-sync-client
    ├── study-sync-server
    ├── studysync-ai
    └── studysync-k8s
```
- Frontend: [`yashrif/study-sync-client`](https://github.com/yashrif/study-sync-client)
- Backend: [`yashrif/study-sync-server`](https://github.com/yashrif/study-sync-server)
- AI integration: [`jahidem/studysync-ai`](https://github.com/jahidem/studysync-ai)
- Kubernetes config: [`jahidem/studysync-k8s`](https://github.com/jahidem/studysync-k8s)

## Technology Stack

- **Backend:** Spring Boot, Spring Security JPA, Hibernate
- **Frontend:** Next.js, Tailwind CSS, Shadcn UI, Framer Motion
- **AI & PDF:** FastAPI, Langchain, Qdrant (Vector Database), Gemini API
- **Database:** PostgreSQL
- **Build Tools:** Maven, Yarn
- **Deployment:** Docker, Kubernetes

## Getting Started

### Prerequisites
- Java 21+
- Node.js 20+
- PostgreSQL
- Maven & Yarn
- Python 3.11.7
- 
### Installation
You need to habe kubernetes setup and be able to use `kubectl` on terminal.
#### Using Kubernetes
1. Clone and navigate to the project directory:
    ```bash
    git clone https://github.com/jahidem/studysync-k8s.git
    cd studysync-k8s
    ```
2.  Open studysync-configmap.yml file and add API keys as needed.
3. Deploy on k8s:
    ```bash
    kubectl apply -f .
    ```
#### Individual Build
Follow instructions for:
- [`yashrif/study-sync-client`](https://github.com/yashrif/study-sync-client)
- [`yashrif/study-sync-server`](https://github.com/yashrif/study-sync-server)
- [`jahidem/studysync-ai`](https://github.com/jahidem/studysync-ai)
- Open browser window on [localhost:3000](http://localhost:3000)
### Usage
TODO

##  Contributors
<p align="left">
   <a href="https://github.com/BrickedSoft/Studysync/graphs/contributors">
      <img src="https://contrib.rocks/image?repo=BrickedSoft/cs24-p2-ju_amadeus">
   </a>
  
</p>
