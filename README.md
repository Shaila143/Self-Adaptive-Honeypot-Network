# 🛡️ Self-Adaptive Honeypot Network

A Self-Adaptive Honeypot Network designed to detect, log, and analyze suspicious activities while dynamically defending against attacks. This project integrates behavior analysis, adaptive database structures, and secure authentication to create a proactive security environment.

🔥 Features

User Authentication & Security

User ID–based restrictions instead of IP blocking.

4 failed login attempts → triggers security response.

Adaptive password generation based on survey inputs.

SHA-512/AES encrypted password storage.

Attack Prevention

Secure login page with behavior analysis.

Rate limiting & bot protection.

Burp Suite & automated attack detection.

JWT-based expiring cookies (regenerated every 30 seconds).

Password System

16-character system-generated passwords with randomness.

Auto-hiding after 30 seconds.

Survey-based password recovery.

Honeypot Defense

Real-time attack logging & analysis.

Dynamic database table ID swapping when suspicious activity is detected.

Behavior monitoring to flag intrusions.

API Security Service

Token-based API authentication.

Secure TLS/SSL-based communication.

🏗️ Project Architecture (Modules)

User Authentication & Security System

Secure Login & Attack Prevention

Password Generation & Recovery

Honeypot Detection & Response

API Security Service

Final Testing & Deployment

⚙️ Tech Stack

Backend: Python (Flask / FastAPI)

Frontend: React / HTML-CSS-JS (for login system)

Database: PostgreSQL / MySQL

Security: SHA-512, AES, JWT, TLS/SSL

Deployment: Cloud hosting (AWS / DigitalOcean)

🚀 Installation & Setup

Clone the repo:

git clone https://github.com/your-username/honeypot-network.git
cd honeypot-network


Create a virtual environment & install dependencies:

python -m venv venv
source venv/bin/activate   # (Linux/Mac)
venv\Scripts\activate      # (Windows)

pip install -r requirements.txt


Configure database in .env file:

DATABASE_URL=your_database_url
SECRET_KEY=your_secret_key


Run the backend server:

uvicorn main:app --reload


(Optional) Run frontend app if included.

📖 Usage

Register as a user → receive a system-generated password.

Login attempts are monitored for suspicious activity.

Multiple failed attempts → triggers honeypot response.

Admins can view attack logs and analyze intrusion patterns.

🔮 Future Enhancements

AI-driven anomaly detection.

Multi-layer honeypot traps with decoy databases.

Advanced visualization dashboard for attack patterns.

Integration with SIEM solutions.

🤝 Contributing

Contributions are welcome! Please fork the repo and submit a pull request.

📜 License

This project is licensed under the MIT License.
