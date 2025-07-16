# 📨 Python Publisher-Subscriber Messaging System

This is a simple Publisher-Subscriber (Pub/Sub) messaging system implemented in Python using sockets and threading. Clients can connect as **publishers** or **subscribers** to topics and send or receive messages in real time.

---

## Features

- Publisher and Subscriber roles
- Multiple topics support
- Real-time message broadcast to subscribers of a topic
- Thread-safe using Python threading locks
- Handles client disconnects gracefully

---

## Files

- `server.py` — Runs the Pub/Sub server
- `client.py` — Client that can be a publisher or subscriber

---

## How to Run

### 1. Run the Server

```bash
python server.py <port>
```

Example:
```bash
python server.py 5000
```

This starts the server on localhost at the specified port.

### 2. Run a Client

```bash
python client.py <host> <port> <role> <topic>
```

- `<host>` — Server address (usually `127.0.0.1` for local)
- `<port>` — Server port (e.g., `5000`)
- `<role>` — Either `publisher` or `subscriber`
- `<topic>` — The topic name to send or receive messages from (e.g., `news`)

---

## Example Usage

### Start the server:
```bash
python server.py 5000
```

### Open a terminal and start a subscriber:
```bash
python client.py 127.0.0.1 5000 subscriber sports
```

### Open another terminal and start a publisher:
```bash
python client.py 127.0.0.1 5000 publisher sports
```

### In the publisher terminal, type a message and press Enter:
```
-> Goal scored by Team A!
```

### The subscriber terminal will show:
```
[sports] Goal scored by Team A!
```

---

## Terminate Publisher Client

Type `terminate` (case-insensitive) in the publisher terminal to disconnect.

---

## Requirements

- Python 3.x

No additional packages needed — uses Python's standard library.

---

## License

This project is licensed under the MIT License.

---

## Author

**Randila** — Computer Science Undergraduate at UCSC

---

## Notes

- If you add a README.md file, add and commit it with:
```bash
git add README.md
git commit -m "Add README"
git push
```

- If your GitHub repo already has commits, pull first before pushing:
```bash
git pull origin main --allow-unrelated-histories
```

Feel free to open issues or contribute via pull requests!
