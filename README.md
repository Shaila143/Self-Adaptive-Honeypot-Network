# 🛡️ Self-Adaptive Honeypot Network  

A **Self-Adaptive Honeypot Network** designed to detect, log, and analyze suspicious activities while dynamically defending against attacks. This project integrates **behavior analysis, adaptive database structures, and secure authentication** to create a proactive security environment.  

---

## 🔥 Features  

- **User Authentication & Security**  
  - User ID–based restrictions instead of IP blocking.  
  - 4 failed login attempts → triggers security response.  
  - Adaptive password generation based on survey inputs.  
  - SHA-512/AES encrypted password storage.  

- **Attack Prevention**  
  - Secure login page with behavior analysis.  
  - Rate limiting & bot protection.  
  - Burp Suite & automated attack detection.  
  - JWT-based expiring cookies (regenerated every 30 seconds).  

- **Password System**  
  - 16-character system-generated passwords with randomness.  
  - Auto-hiding after 30 seconds.  
  - Survey-based password recovery.  

- **Honeypot Defense**  
  - Real-time attack logging & analysis.  
  - Dynamic database table ID swapping when suspicious activity is detected.  
  - Behavior monitoring to flag intrusions.  

- **API Security Service**  
  - Token-based API authentication.  
  - Secure TLS/SSL-based communication.  

---

## 🏗️ Project Architecture (Modules)  

1. **User Authentication & Security System**  
2. **Secure Login & Attack Prevention**  
3. **Password Generation & Recovery**  
4. **Honeypot Detection & Response**  
5. **API Security Service**  
6. **Final Testing & Deployment**  

---

## ⚙️ Tech Stack  

- **Backend:** Python (Flask / FastAPI)  
- **Frontend:** React / HTML-CSS-JS (for login system)  
- **Database:** PostgreSQL / MySQL  
- **Security:** SHA-512, AES, JWT, TLS/SSL  
- **Deployment:** Cloud hosting (AWS / DigitalOcean)  

---

## 🚀 Installation & Setup  

1. Clone the repo:  
   ```bash
   git clone https://github.com/your-username/honeypot-network.git
   cd honeypot-network
   ```

2. Create a virtual environment & install dependencies:  
   ```bash
   python -m venv venv
   source venv/bin/activate   # (Linux/Mac)
   venv\Scripts\activate      # (Windows)

   pip install -r requirements.txt
   ```

3. Configure database in `.env` file:  
   ```env
   DATABASE_URL=your_database_url
   SECRET_KEY=your_secret_key
   ```

4. Run the backend server:  
   ```bash
   uvicorn main:app --reload
   ```

5. (Optional) Run frontend app if included.  

---

## 📖 Usage  

- Register as a user → receive a system-generated password.  
- Login attempts are monitored for suspicious activity.  
- Multiple failed attempts → triggers honeypot response.  
- Admins can view **attack logs** and analyze intrusion patterns.  

---

## 🔮 Future Enhancements  

- AI-driven anomaly detection.  
- Multi-layer honeypot traps with decoy databases.  
- Advanced visualization dashboard for attack patterns.  
- Integration with SIEM solutions.  

---

## 🤝 Contributing  

Contributions are welcome! Please fork the repo and submit a pull request.  

---

## 📜 License  

This project is licensed under the MIT License.  
