<a href="https://github.com/KelvinCode1234/ai-chatbot">
  <img alt="FastAPI-powered AI chatbot with staff approval and knowledge base" src="assets/opengraph-image.png">
  <h1 align="center">AIChatbot</h1>
</a>

<p align="center">
  AIChatbot is a blazing-fast, open-source chatbot template powered by FastAPI, React, and a custom knowledge base with staff approval functionality.
</p>

<p align="center">
  <a href="#features"><strong>Features</strong></a> ·
  <a href="#tech-stack"><strong>Tech Stack</strong></a> ·
  <a href="#deploy-your-own"><strong>Deploy Your Own</strong></a> ·
  <a href="#running-locally"><strong>Running Locally</strong></a> ·
  <a href="#license"><strong>License</strong></a>
</p>

<br/>

## 🧠 Features

- **FastAPI backend** – Ultra-fast API built in Python
- **React frontend** – Clean UI with Tailwind CSS
- **Knowledge base system** – Pulls responses from pre-fed data
- **Staff approval** – Human-in-the-loop moderation for quality control
- **Fully modular** – Easily extend with new features or APIs

---

## 🧱 Tech Stack

- ⚙️ **Backend**: FastAPI (Python)
- 💻 **Frontend**: React, TypeScript, Tailwind CSS
- 💾 **Database**: SQLite / Postgres
- 🐳 **Deployment**: Docker & Docker Compose ready
- 🔐 **Security**: .env configuration & API Key handling

---

## 🚀 Deploy Your Own

You can deploy your own AIChatbot with **Docker**:

```bash
docker-compose up --build
```

Or deploy manually via Vercel, Railway, Render, or any backend hosting of your choice. Be sure to set the proper environment variables as seen in `.env.example`.

---

## 🛠 Running Locally

### 1. Clone the project

```bash
git clone https://github.com/KelvinCode1234/ai-chatbot
cd ai-chatbot
```

### 2. Backend setup

```bash
cd backend
python -m venv venv
source venv/bin/activate  # For Windows: venv\Scripts\activate
pip install -r requirements.txt
```

Set up your `.env` file:

```env
DATABASE_URL=sqlite:///./bot.db
API_KEY=your_api_key_here
```

Start the backend:

```bash
uvicorn main:app --reload
```

---

### 3. Frontend setup

```bash
cd frontend
npm install
npm run dev
```

Visit `http://localhost:3000` to access the chatbot.

---

## 📁 Project Structure

```
ai-chatbot/
│
├── backend/          # FastAPI app
│   ├── main.py
│   ├── models/
│   ├── routes/
│   └── utils/
│
├── frontend/         # React app
│   ├── src/
│   └── public/
│
├── docker-compose.yml
└── README.md
```

---

## 📜 License

This project is licensed under the **MIT License**. See [`LICENSE`](./LICENSE) for details.

---

## 🙏 Acknowledgements

- Inspired by [`pkaramagi/aichatbot`](https://github.com/pkaramagi/aichatbot)
- Built by [KelvinCode1234](https://github.com/KelvinCode1234) with ❤️