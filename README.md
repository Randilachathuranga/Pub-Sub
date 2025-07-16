# 📨 Python Publisher-Subscriber Messaging System

This is a simple Publisher-Subscriber (Pub/Sub) messaging system implemented using Python sockets and threading. It allows multiple clients to connect as **publishers** or **subscribers** for specific topics and communicate in real-time.

---

## 🚀 Features

- Clients can choose to be either **Publisher** or **Subscriber**
- Support for multiple **topics** (e.g., `news`, `weather`, `sports`)
- Real-time broadcasting from publishers to all subscribers of a topic
- Thread-safe communication using `threading.Lock`
- Graceful handling of client disconnections

---

## 🛠️ Tech Stack

- **Language**: Python 3.x
- **Concepts**: Socket Programming, Multi-threading

---

## 📁 Project Structure

