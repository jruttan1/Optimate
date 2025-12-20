# Optimate  

[![Deployed on Vercel](https://img.shields.io/badge/Live%20Demo-Vercel-blue?logo=vercel)](https://optimate-two.vercel.app/) 

https://github.com/user-attachments/assets/e16653b8-a15a-481d-a4b2-122dfcbfecd0

**Optimate** is an AI-powered underwriting dashboard that transforms raw insurance policy data into actionable insights, helping underwriters make faster, smarter, and more confident decisions.  

---

## Elevator Pitch  

**“Optimate: AI dashboards, insights, and reinforcement learning for smarter underwriting.”**  

Optimate reimagines the underwriting process by blending **AI, reinforcement learning, real-time tracking, and intuitive visualizations** into one seamless platform.  

---

## Features  

- **Top Matches** → View the top 10 submissions that best align with appetite guidelines.  
- **Explainability** → Get detailed AI-driven justifications for why a policy is prioritized.  
- **Approve/Decline Actions** → Take decisions directly from the dashboard.  
- **Reinforcement Learning** → Provide satisfaction feedback so the AI improves over time.  
- **Visual Analytics** → Explore plots, live tracking, and interactive heatmaps of U.S. states colored by appetite and risk scores.  
- **Contextual AI Chatbot** → Two-way conversations with the AI at the **individual policy level**, enabling clarifications and co-decision making.  

---

## How We Built It  

- **Frontend & Deployment**:  
  - [Next.js (App Router)](https://nextjs.org/) + [TailwindCSS](https://tailwindcss.com/) + [shadcn/ui](https://ui.shadcn.com/)  
  - Deployed on [Vercel](https://vercel.com/) for fast CI/CD and scalability.  
  - [Auth0](https://auth0.com/) for secure authentication and role-based access.  

- **Data Layer**:  
  - Policy data ingested from the [Federato API](https://product.federato.ai/).  
  - Enriched in **Python** with risk scores, appetite scores, and account-level analytics.  

- **AI & Insights**:  
  - **CohereAI LLMs** + **Retrieval-Augmented Generation (RAG)** to explain why submissions are in-appetite.  
  - **Reinforcement learning loop** powered by underwriter feedback (approve/decline, satisfaction scores).  
  - Context-aware **AI chatbot** at the policy level.  

- **Storage & State Management**:  
  - **AWS DynamoDB** for user preferences, chat history, cached embeddings, and saved searches.  

- **Visualization**:  
  - Built with **Recharts** and **D3.js** to show:  
    - Interactive plots  
    - Risk & appetite heatmaps  
    - Portfolio leaderboards  

---

## Inspiration  

We were inspired by Federato’s challenge:  

> *“Reimagine the RiskOps landing page experience… intelligently surface a curated set of submissions that are most aligned with the carrier's appetite—enabling faster and more effective underwriting decisions.”*  

Underwriters often juggle complex and conflicting factors like TIV, loss ratios, building age, and state regulations. Optimate was built to simplify this decision-making by combining **AI, reinforcement learning, and visual storytelling** into one dashboard.  

---

## Challenges We Ran Into  

- Understanding new insurance/underwriting concepts like **TIV, appetite guidelines, and loss ratios**.  
- Handling **merge conflicts** in a 4-dev hackathon team under time pressure.  
- Designing a **reinforcement learning loop** that balanced rule-based scoring with AI reasoning.  
- Securing **AWS DynamoDB** with the right IAM roles and schema design.  
- Optimizing **visualizations** for responsiveness while handling large datasets.  

---

## Accomplishments  

- Delivered a **production-ready product** within the hackathon timeframe.  
- Rapidly learned and integrated **CohereAI, Auth0, DynamoDB, and shadcn/ui**.  
- Implemented **reinforcement learning foundations** for underwriting feedback loops.  
- Built **heatmaps, live tracking, and plots** that made underwriting metrics intuitive.  

---

## What We Learned  

- Clear **team communication** is crucial under time pressure.  
- How to design and deploy a **RAG pipeline with Cohere**.  
- Practical application of **reinforcement learning** in a real-world use case.  
- Insights into the **insurance industry** and underwriters’ real challenges.  
- How to take a **vague problem statement** and ship a polished end-to-end solution.  

---

## What’s Next  

- **Deeper AI** → Fine-tune LLMs for nuanced underwriting strategies.  
- **Dynamic Data Feeds** → Add weather, property valuation, and catastrophe models.  
- **Explainability** → Richer visual cues (confidence intervals, score breakdowns).  
- **Collaboration** → Shared views, notes, and histories for underwriting teams.  
- **Mobile** → Extend Optimate to iOS/Android for underwriting on the go.  
- **Enterprise-Ready Infra** → Multi-region cloud deployment, audit trails, and monitoring.  

---

## 🛠️ Built With  

`Next.js, Vercel, TailwindCSS, shadcn/ui, Auth0, CohereAI, Python, AWS DynamoDB, Federato API, Recharts, D3.js, Retrieval-Augmented Generation (RAG), Reinforcement Learning, OAuth 2.0`  

---

## 🔗 Links  

- **Deployed App** → [Optimate on Vercel](https://optimate-two.vercel.app/auth)  
- **Hackathon Challenge** → [Federato RiskOps Hackathon](https://hackthenorth.com/)  

---

## Team  

Built with ☕ and teamwork by four developers at **Hack the North 2025**.  
