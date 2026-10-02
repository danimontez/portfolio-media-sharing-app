# 📸 Photo & Video Sharing App 

A photo and video sharing app built with **FastAPI** (backend) and **Streamlit** (frontend).

---

## 📖 Overview

This project is a full-stack media sharing application that allows users to upload, view, and interact with photos and videos. The backend is powered by **FastAPI** for fast, async API endpoints, while the frontend is built with **Streamlit** for a simple, interactive UI.

---

## ✨ Features

- 🔐 User authentication (signup / login)
- 📤 Upload photos and videos
- 🖼️ View a feed of shared media
- 🗑️ Delete your own posts

---

## 🛠️ Tech Stack

| Layer      | Technology              |
|------------|--------------------------|
| Backend    | FastAPI, Uvicorn         |
| Frontend   | Streamlit                |
| Database   | SQLite       |
| ORM        | SQLAlchemy               |
| Auth       | JWT (python-jose)        |
| File Store | Imagekit         |

---

## 📂 Project Structure

```
portfolio-media-sharing-app/
├── src/
│   └── media_sharing_app/
│       ├── app.py
│       ├── db.py
│       ├── schemas.py
│       ├── users.py
│       └── images.py/
├── frontend.py/
├── main.py/
├── pyproject.toml/
├── uv.lock/
├── .gitignore
└── README.md
```

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/danimontez/portfolio-media-sharing-app.git
cd portfolio-media-sharing-app.git
```

### 2. Install dependencies

```bash
uv sync
```

Create a `.env` file (see `.env.example`):

```env
IMAGEKIT_PRIVATE_KEY=
IMAGEKIT_URL_ENDPOINT=
```
### 3. Run the project

Run the backend:

```bash
uv run ./main.py 
```

The API will be available at `http://127.0.0.1:8000`.
Interactive docs: `http://127.0.0.1:8000/docs`

Run the frontend:

```bash
streamlit run frontend.py
```

---

## 🔌 API Endpoints (Example)

| Method | Endpoint              | Description               |
|--------|-----------------------|---------------------------|
| POST   | `/auth/register`      | Register a new user       |
| POST   | `/auth/jwt/login`         | Login and get JWT token   |
| GET    | `/users/me`           | Get current user          |
| POST   | `/upload`       | Upload a photo or video   |
| GET    | `/feed`             | Get media feed            |
| DELETE | `/posts/{id}`         | Delete a post             |

---


## 🙏 Acknowledgements

- [FastAPI](https://fastapi.tiangolo.com/)
- [Streamlit](https://streamlit.io/)
- [SQLAlchemy](https://www.sqlalchemy.org/)

---

