# 🧠 Hackathon II – Phase IV  
## **Evolution of Todo: Local Kubernetes Deployment**

Phase IV evolves the **Phase III Todo AI Chatbot** into a **cloud-native, locally deployed application** using Kubernetes, Helm Charts, and AI-assisted DevOps tools.  

All deployment tasks are implemented via **Claude Code + Spec-Kit Plus**, no manual scripting required.  

---

## 🎯 Phase IV Goal

- Containerize frontend & backend applications  
- Deploy the AI Todo Chatbot on **local Kubernetes (Minikube)**  
- Use **Helm Charts** for deployment  
- Apply **AI-assisted Docker & Kubernetes operations** with Gordon, kubectl-ai, and Kagent  

💡 **Development Approach:** Spec → Plan → Tasks → Claude Code → Test & Deploy

---

## 🛠️ Technology Stack

| Component         | Technology |
|------------------|------------|
| Containerization  | Docker Desktop + Gordon (AI Agent) |
| Orchestration     | Kubernetes (Minikube) |
| Package Manager   | Helm Charts |
| AI DevOps         | kubectl-ai, Kagent |
| Application       | Phase III Todo Chatbot (Frontend & Backend) |

---

## 🚀 Key Deployment Steps

1. **Enable Gordon** (Docker AI Agent)  
   - Settings → Beta features → Toggle AI Agent  
   - Example:  
     ```bash
     docker ai "What can you do?"
     ```

2. **Containerize apps**  
   - Frontend & Backend via Docker or Gordon AI-assisted commands  

3. **Helm Charts**  
   - Generate deployment charts for frontend & backend  
   - Use kubectl-ai / Kagent to create and optimize  

4. **Deploy to Minikube**  
   - Start local cluster:  
     ```bash
     minikube start
     ```  
   - Deploy with Helm:  
     ```bash
     helm install todo-frontend ./helm/frontend
     helm install todo-backend ./helm/backend
     ```

5. **AI-assisted Kubernetes Management**  
   - kubectl-ai example:  
     ```bash
     kubectl-ai "deploy the todo frontend with 2 replicas"
     kubectl-ai "scale the backend to handle more load"
     kubectl-ai "check why the pods are failing"
     ```
   - Kagent example:  
     ```bash
     kagent "analyze the cluster health"
     kagent "optimize resource allocation"
     ```

---

## 🔑 Key Architecture Benefits

- **Stateless Server:** Any pod can handle any request  
- **Scalable & Resilient:** Server restarts do not affect conversation state  
- **Spec-Driven Deployment:** Claude Code + Agent Skills for automated infrastructure  
- **Blueprints for IaC:** Standardized templates for future cloud deployments  

---

## ▶️ How to Run Locally

1. Ensure **Docker Desktop 4.53+**, **Minikube**, and **Helm** installed  
2. Enable Gordon (Docker AI Agent)  
3. Start Minikube:  
   ```bash
   minikube start
Build & deploy containers:

docker build -t todo-frontend ./frontend
docker build -t todo-backend ./backend
helm install todo-frontend ./helm/frontend
helm install todo-backend ./helm/backend
