# 🏥 Hospital Remote Doctor Access using VPN

## 📌 Project Overview
This project simulates a secure hospital network where doctors can remotely access patient records using a Virtual Private Network (VPN). The system focuses on demonstrating how secure communication is established over a network using SSL/TLS encryption.

It creates a realistic environment where sensitive medical data is protected from unauthorized access, while still allowing doctors to work remotely in a safe and controlled manner.

---

## 🎯 Objectives
- To simulate secure remote access in a hospital system  
- To demonstrate SSL/TLS-based encrypted communication  
- To implement authentication before accessing sensitive data  
- To show how VPN tunnels protect data transmission  
- To visualize network communication in an interactive way  

---

## 🏗️ System Architecture

The project is divided into three main components:

### 👨‍⚕️ Doctor Client (User Side)
- Runs on: `http://127.0.0.1:5011`
- Provides interface for doctors
- Handles login, registration, and patient access
- Connects to server through secure VPN tunnel

### 🏥 Hospital Server (Backend)
- Runs on: `127.0.0.1:8443`
- Handles SSL/TLS connections
- Processes requests from doctor client
- Manages authentication and patient data

### 📊 Admin Dashboard
- Runs on: `http://127.0.0.1:5000`
- Displays logs and system activity
- Monitors secure connections and events
- Shows patient database and access logs

---

## 🔐 Security Implementation

### SSL/TLS Encryption
- Secure tunnel created using Python SSL module  
- All communication is encrypted  
- Prevents data interception  

### Authentication System
- Doctors must register/login before accessing data  
- Unauthorized users are blocked  
- Invalid access attempts are logged  

### Secure Data Access
- Patient records are hidden until authentication  
- All requests pass through secure VPN channel  

---

## 💻 Key Features
- 🔒 Secure VPN-based communication  
- 🔑 Login & Registration system  
- 📡 Real-time connection simulation  
- 📊 Admin monitoring dashboard  
- 🗄️ SQLite database for storage  
- ⚡ Interactive UI showing packet flow and encryption  
- 🚫 Unauthorized access detection  

---

## 🔄 Workflow

1. User opens Doctor Portal  
2. Connects to hospital via VPN  
3. SSL handshake is established  
4. User logs in or registers  
5. Secure connection is verified  
6. Patient data is accessed through encrypted channel  
7. Admin dashboard logs all activity  

---

## 🧪 Testing & Results

- ✅ Secure connection established successfully  
- ✅ Encrypted data transmission working  
- ✅ Only authenticated users can access data  
- ❌ Unauthorized access attempts blocked  
- ✅ Real-time logs visible in admin panel  

---

## 📊 System Modules

### Doctor Portal
- VPN connection control  
- Login / Registration  
- Patient records view  
- Data update functionality  

### Admin Panel
- Live network logs  
- Patient database view  
- Activity monitoring  

---

## ⚙️ How to Run

### 1. Install Dependencies
```bash
pip install -r requirements.txt
