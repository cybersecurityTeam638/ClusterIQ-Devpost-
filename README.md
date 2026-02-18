# **Elasticsearch Agent Builder Project**

This project is developed for the **Elasticsearch Agent Builder Hackathon**.  
It includes a collection of **9 monitoring tools** and an **Agent Builder** to help build, deploy, and manage Elasticsearch agents efficiently.  
The tools provide insights into cluster health, node performance, shard states, and alerts, while the Agent Builder enables easy configuration and deployment of agents.

---

## **Project Components**

### **1. Monitoring Tools**
The project includes **9 Elasticsearch ES|QL monitoring tools**, each with a **Tool ID, description, labels, and query**:

| Tool ID | Description | Labels |
|---------|-------------|--------|
| `check_cluster_health_daily` | Shows the cluster health over the last day | `cluster-health` |
| `check_nodes_uptime` | Tracks uptime for each node | `node-monitoring` |
| `high_node_resource_alert` | Alerts when node CPU/memory is high | `alerts,node-resources` |
| `last_red_status_check` | Checks last red cluster status | `cluster-health,alerts` |
| `latest_cluster_status` | Retrieves the latest cluster status | `cluster-health` |
| `node_index_search_latency` | Measures search latency per node/index | `performance,node-metrics` |
| `recent_shard_states` | Displays recent shard allocation and state changes | `shards,cluster-health` |
| `red_cluster_alert_30min` | Alerts if the cluster has been red for 30 minutes | `alerts,cluster-health` |
| `top_node_metrics` | Shows top node metrics: CPU, memory, disk | `node-metrics,performance` |

> Each tool includes a ready-to-use **ES|QL query** to retrieve data from Elasticsearch.

---

### **2. Elasticsearch Agent Builder**
The **Agent Builder** component allows you to:  
- Easily create, configure, and deploy Elasticsearch agents.  
- Connect the agents to monitoring tools dynamically.  
- Automate alerting, data collection, and indexing.  
- Build agents for custom use cases in your Elasticsearch clusters.

This tool is particularly useful for **Hackathon participants or teams managing multiple clusters**, providing a simplified interface for agent creation and deployment.

---

## **Features**
- Ready-made **ES|QL monitoring tools** for clusters and nodes.  
- **Agent Builder** to automate agent deployment and management.  
- Real-time cluster health and performance monitoring.  
- Alerts for high resource usage, red cluster status, and shard issues.  
- Simple and modular structure for extending tools and queries.

---

