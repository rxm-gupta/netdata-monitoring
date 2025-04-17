# Monitoring With Netdata

This project demonstrates how to run **Netdata**, a real-time performance monitoring tool, in a Docker container.

## 📌 Overview

- Run Netdata in a Docker container.
- Expose the Netdata dashboard.
- Access system metrics via a web-based UI.

---

## 🚀 Getting Started

### ✅ Prerequisites

- Docker installed and running

---

### 🐳 Run Netdata Container

Use the following command to run Netdata:

```bash
docker run -d --name=netdata -p 19999:19999 netdata/netdata
```
---

### 🔍 Access Netdata Dashboard

🖥️ If running locally:

Open your browser and go to:
```bash
http://localhost:19999
```

☁️ If running on an EC2 instance:

Replace localhost with your EC2 instance’s public IP address.
```bash
http://<EC2-PUBLIC-IP>:19999
```

Make sure your EC2 security group allows inbound traffic on port 19999 (TCP).

🔐 You can do this by adding a rule in the EC2 instance's security group:

Type: Custom TCP

Port Range: 19999

Source: 0.0.0.0/0 (or a specific IP range for security)


![Image](https://github.com/user-attachments/assets/564a3e62-5e84-4698-a869-0c8e88c24b3d)

![Image](https://github.com/user-attachments/assets/ebabb662-fec0-4aee-9ed3-81d27b59f4eb)

![Image](https://github.com/user-attachments/assets/a99c5f4e-0222-454e-81e7-93c462552124)

![Image](https://github.com/user-attachments/assets/94561863-c08b-4372-971d-e231200098b1)

![Image](https://github.com/user-attachments/assets/2dc193ab-ccc0-4190-a2b9-1175b4cee973)
