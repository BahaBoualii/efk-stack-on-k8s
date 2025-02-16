# 🚀 EFK Stack on Kubernetes  

This project provides a simple and effective way to deploy Elasticsearch, Fluentd, and Kibana on a Kubernetes cluster for centralized log management and visualization.  

![EFK-stack-on-Kubernetes](https://github.com/user-attachments/assets/623419a9-b149-4e0d-8d95-dc0d922787b8)


## 📌 Overview  

EFK is a powerful stack used for log aggregation and monitoring in Kubernetes environments. Here's what each component does:  

- **Elasticsearch** 🛠️ – Stores and indexes logs efficiently.  
- **Fluentd** 🔄 – Collects, processes, and forwards logs to Elasticsearch.  
- **Kibana** 📊 – Visualizes logs and provides insights via an intuitive dashboard.  

## 🏗️ Deployment Guide  

### 📋 Prerequisites  
Before you begin, ensure you have:  

✅ A running Kubernetes cluster  
✅ `kubectl` installed and configured  
✅ Adequate resources to run EFK smoothly  

### 🚀 Installation Steps  

#### 1️⃣ Deploy Elasticsearch  

```sh
kubectl apply -f elasticsearch/elasticsearch-deployment.yaml
```

#### 2️⃣ Deploy Fluentd

```sh
kubectl apply -f fluentd/fluentd-daemonset.yaml
```
#### 3️⃣ Deploy Kibana

```sh
kubectl apply -f kibana/kibana-deployment.yaml
```

## 📌 Notes

-   Adjust resource limits in the YAML files based on your cluster capacity.
-   Modify Fluentd configurations to match your logging needs.
-   If you encounter any issues, feel free to create an issue in this repository.
