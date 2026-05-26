# 🔐 SIEM Log Dashboard Using ELK Stack

## 📌 Project Overview
The **SIEM Log Dashboard Using ELK Stack** project is designed to demonstrate centralized log monitoring and cybersecurity event analysis using the ELK Stack.

The system collects logs from systems or applications, processes and parses them using Logstash, stores them in Elasticsearch, and visualizes them through Kibana dashboards.

This project helps in monitoring suspicious activities such as failed login attempts and provides better visibility into security events.

---

# 📌 Problem Statement
Modern organizations generate huge amounts of logs from servers, systems, applications, and network devices. Manually monitoring these logs is difficult, time-consuming, and inefficient.

Without centralized monitoring:
- suspicious activities may go unnoticed,
- security incidents may not be detected quickly,
- log analysis becomes difficult.

This project provides a centralized SIEM dashboard for efficient log collection, processing, storage, searching, and visualization using the ELK Stack.

---

# 📌 Objectives
- To collect system and security logs
- To process logs using Logstash
- To store logs in Elasticsearch
- To visualize logs using Kibana dashboards
- To analyze failed login attempts and suspicious activities
- To understand SIEM architecture and ELK Stack implementation

---

# 📌 Technologies Used

| Technology | Purpose |
|---|---|
| Kali Linux | Development environment |
| Elasticsearch | Log storage and searching |
| Logstash | Log collection and processing |
| Kibana | Data visualization and dashboards |
| Python | Sample log generation |
| Virtual Machine | Running Linux environment |

---

# 📌 ELK Stack Components

## 🔹 Elasticsearch
Elasticsearch is a distributed search and analytics engine used for:
- storing logs,
- indexing data,
- fast searching,
- log analysis.

Default Port:
```text
9200
```

---

## 🔹 Logstash
Logstash is a data processing pipeline used for:
- collecting logs,
- filtering logs,
- parsing log data,
- sending logs to Elasticsearch.

Pipeline Structure:
```text
Input → Filter → Output
```

---

## 🔹 Kibana
Kibana is a visualization tool used for:
- creating dashboards,
- generating charts and graphs,
- analyzing logs,
- monitoring security events.

Default Port:
```text
5601
```

---

# 📌 System Architecture

```text
Log Sources
     ↓
Logstash
(Log Collection & Processing)
     ↓
Elasticsearch
(Log Storage & Indexing)
     ↓
Kibana
(Visualization & Analysis)
     ↓
Security Analyst
```

---

# 📌 Working of the Project

## Step 1 – Log Collection
Logs are generated from system activities and failed login attempts.

Example:
```text
Failed password for admin from 192.168.1.10
```

---

## Step 2 – Log Processing
Logstash collects raw logs and:
- extracts IP addresses,
- identifies usernames,
- parses timestamps,
- categorizes events.

---

## Step 3 – Log Storage
Processed logs are stored in Elasticsearch in structured JSON format.

---

## Step 4 – Visualization
Kibana visualizes logs using:
- dashboards,
- graphs,
- tables,
- alert monitoring.

---

# 📌 Installation Steps

## 🔹 Install Elasticsearch
```bash
sudo apt install elasticsearch
```

## 🔹 Start Elasticsearch
```bash
sudo systemctl start elasticsearch
```

## 🔹 Verify Elasticsearch
```bash
curl http://localhost:9200
```

---

## 🔹 Install Logstash
```bash
sudo apt install logstash
```

---

## 🔹 Install Kibana
```bash
sudo apt install kibana
```

## 🔹 Start Kibana
```bash
sudo systemctl start kibana
```

---

# 📌 Access Kibana Dashboard

Open browser and visit:
```text
http://localhost:5601
```

---

# 📌 Important Commands Used

## Check Elasticsearch Status
```bash
sudo systemctl status elasticsearch
```

## Check Kibana Status
```bash
sudo systemctl status kibana
```

## Check Kibana Port
```bash
sudo ss -tulnp | grep 5601
```

## Restart Elasticsearch
```bash
sudo systemctl restart elasticsearch
```

---

# 📌

---

# 📌 Kibana Dashboard Features
- Failed login monitoring
- Log searching and filtering
- Time-based analysis
- Alert monitoring
- Dashboard visualization
- Security event analysis

---

# 📌 Results
- Successfully implemented SIEM Log Dashboard using ELK Stack
- Logs were collected and processed successfully
- Elasticsearch stored and indexed log data
- Kibana dashboards visualized failed login activities
- Security-related logs were analyzed effectively

---

# 📌 Advantages
- Open-source solution
- Fast searching and indexing
- Centralized log monitoring
- Easy dashboard visualization
- Scalable architecture
- Useful for cybersecurity analysis

---

# 📌 Limitations
- Basic implementation
- No advanced AI-based detection
- Limited real-time monitoring
- Requires system resources and configuration

---

# 📌 Future Scope
- Real-time log monitoring using Filebeat
- Automated alert notifications
- AI-based anomaly detection
- Cloud deployment
- SOC integration
- Advanced threat intelligence integration

---

# 📌 Applications
- Security Operations Centers (SOC)
- Cybersecurity monitoring
- Log management systems
- Threat analysis
- Incident investigation
- Network monitoring

---

# 📌 Conclusion
The project successfully demonstrates the implementation of a SIEM Log Dashboard using the ELK Stack. It provides centralized log collection, processing, storage, searching, and visualization for cybersecurity monitoring and analysis.

The project improved understanding of:
- SIEM systems,
- log management,
- cybersecurity monitoring,
- ELK Stack technologies.

---

# 📌 Team Members
- AGILI SAMPITHA 
- U SANJANA
- PAVITHRA D

---

# 📌 License
This project is developed for academic and educational purposes only.
