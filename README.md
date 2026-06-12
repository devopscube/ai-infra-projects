## 🤖 AI Era Projects

The skills that got you hired three years ago are not the skills that keep you hired now.

Models run on GPUs. Inference has SLOs. A bad rollout serves wrong answers instead of 500 errors. Cost can 10x overnight if a node pool autoscales the wrong way.

This track turns DevOps, SRE, and Platform engineers into the people who run AI in production. You already know Kubernetes, Terraform, and observability. Here you apply them to GPUs, models, pipelines, and LLMs.

**You do not need to be a data scientist.** You need to know how to ship, scale, and keep AI workloads alive. That is an infrastructure problem, and that is what this track teaches.

> 🧭 **Suggested order:** Work the AI Foundations projects first even if you are senior. The GPU and serving basics underpin everything in MLOps and LLMOps.

---

### 🟢 AI Foundations — Run a model in production without the ML theory

Start here. These projects get a real model serving traffic and teach the primitives every later project depends on.

| # | Project | What You Will Learn |
|---|---------|---------------------|
| A1 | Containerize and Serve Your First Model | Package a model behind a FastAPI endpoint, Dockerize it, and serve real predictions. Learn why ML containers are huge and how to slim them |
| A2 | GPU Fundamentals for Engineers | Understand CUDA, drivers, the NVIDIA Container Toolkit, and how a GPU actually gets attached to a container. The mental model for everything that follows |
| A3 | Serve an LLM on a Single GPU with vLLM | Run Llama 3 on one GPU with vLLM. Measure tokens/sec, understand KV cache, batching, and why naive serving wastes 80% of your GPU |
| A4 | Model Registry and Versioning Basics | Track models, datasets, and metrics with MLflow. Treat a model like an artifact with a version, not a file someone DMs you |

---

### 🟡 MLOps — CI/CD and pipelines for models

For engineers ready to treat ML like software: versioned data, reproducible pipelines, automated retraining, and monitoring that catches a model going stale.

| # | Project | What You Will Learn |
|---|---------|---------------------|
| A5 | Data Versioning with DVC and S3 | Version large datasets the way you version code. Reproduce any training run from a Git commit. The foundation of reproducible ML |
| A6 | Build an ML Pipeline with Airflow on EKS | Orchestrate ingest, train, evaluate, and register as a DAG on Kubernetes. The same orchestration skills you already use, pointed at models |
| A7 | Feature Store with Feast | Stand up a feature store so training and serving use the same features. Kill training-serving skew, the bug that silently breaks models |
| A8 | CI/CD Pipeline for Models with GitHub Actions | Build a pipeline that trains, tests, and gates a model on metrics before it ships. A model that fails accuracy checks should never reach prod |
| A9 | Kubeflow Pipelines End to End | Run a full training-to-deployment pipeline on Kubernetes with Kubeflow. Reusable components, artifacts, and lineage |
| A10 | Model Monitoring and Drift Detection | Detect data drift and prediction drift in production. Alert before a model quietly starts giving bad answers. SRE for ML |

---

### 🔴 GPU on Kubernetes — Make the cluster schedule and share GPUs

For platform engineers who own the cluster. GPUs are expensive, scarce, and do not behave like CPU. This is how you run them efficiently for a whole team.

| # | Project | What You Will Learn |
|---|---------|---------------------|
| A11 | GPU Scheduling with the NVIDIA Device Plugin | Expose GPUs as a schedulable resource, request them in pods, and understand how the scheduler places GPU workloads |
| A12 | GPU Sharing with Time-Slicing and MIG | Let multiple workloads share one GPU with time-slicing and Multi-Instance GPU. Stop paying for whole A100s to run small models |
| A13 | Autoscale GPU Nodes with Karpenter | Scale GPU node pools up for jobs and down to zero when idle. The single biggest lever on your AI infra bill |
| A14 | GPU Observability with DCGM and Prometheus | Scrape GPU utilization, memory, and temperature into Grafana. Answer "is the GPU actually busy or just allocated?" |
| A15 | Multi-Tenant GPU Platform with Quotas and Priority | Give teams fair GPU access with namespaces, ResourceQuotas, and priority classes. The platform engineering layer over raw GPUs |

---

### 🔴 LLMOps — Run LLMs and AI applications at scale

The newest and most in-demand layer. Serving LLMs, RAG infrastructure, gateways, guardrails, and the observability and cost controls that LLMs specifically need.

| # | Project | What You Will Learn |
|---|---------|---------------------|
| A16 | Scalable LLM Serving with vLLM on Kubernetes | Go from one GPU to an autoscaling LLM service with replicas, health checks, and rolling updates. Production inference, not a demo |
| A17 | RAG Infrastructure with a Vector Database | Deploy a vector DB and build the retrieval layer behind a RAG app. The infra under every "chat with your docs" product |
| A18 | LLM Gateway and Multi-Model Routing | Put a gateway in front of multiple models for routing, rate limiting, fallback, and a single API. The reverse proxy of the AI stack |
| A19 | LLM Observability — Tokens, Latency, and Cost | Trace requests, track token usage, and attribute cost per team and per feature. You cannot optimize a bill you cannot see |
| A20 | Guardrails and Safety for LLM Apps | Add input/output filtering, prompt-injection defenses, and PII redaction in front of an LLM. The security layer for AI in production |
| A21 | Self-Hosted AI Coding Assistant Platform | Run an open model as an internal coding assistant with auth, logging, and quotas. A real internal developer platform for the AI era |

---

### 🚀 Capstone — Inference Platform on Kubernetes

Tie it all together. Build a self-service platform where a team pushes a model and gets an autoscaling, observable, cost-tracked, GPU-backed endpoint with no tickets.

| # | Project | What You Will Learn |
|---|---------|---------------------|
| A22 | Build a Self-Service Inference Platform | Combine GPU autoscaling, model serving, observability, guardrails, and a GitOps deploy flow into one platform. The portfolio project that gets you the AI platform job |

---

> 💬 **Want a project that is not here?** Open an [Issue](https://github.com/techiescamp/devops-projects/issues) with the title and use case. AI infra moves fast and this track grows with it.
