# 🍵 Tea API — FastAPI CRUD App

A simple RESTful API built with **FastAPI** for managing a collection of teas. Supports full CRUD operations using an in-memory data store.

---

## 📁 Project Structure

```
fastapi-crash/
├── main.py              # Main application file
├── requirements.txt     # Project dependencies
└── .venv/               # Virtual environment
```

---

## 🚀 Getting Started

### Prerequisites

- Python 3.8+
- pip

### Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/your-username/fastapi-crash.git
   cd fastapi-crash
   ```

2. **Create and activate a virtual environment**

   ```bash
   python -m venv .venv

   # On Windows
   .venv\Scripts\activate

   # On macOS/Linux
   source .venv/bin/activate
   ```

3. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

4. **Run the development server**

   ```bash
   uvicorn main:app --reload
   ```

   The API will be available at `http://127.0.0.1:8000`

---

## 📖 API Endpoints

| Method   | Endpoint            | Description         |
|----------|---------------------|---------------------|
| `GET`    | `/teas`             | Get all teas        |
| `GET`    | `/teas/{tea_id}`    | Get a tea by ID     |
| `POST`   | `/teas`             | Add a new tea       |
| `PUT`    | `/teas/{tea_id}`    | Update a tea by ID  |
| `DELETE` | `/teas/{tea_id}`    | Delete a tea by ID  |

---

## 🧪 Interactive Docs

FastAPI automatically generates interactive API documentation:

- **Swagger UI**: [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs)
- **ReDoc**: [http://127.0.0.1:8000/redoc](http://127.0.0.1:8000/redoc)

---

## 📦 Dependencies

```
fastapi
uvicorn
```

> See `requirements.txt` for exact versions.

---

## ⚠️ Notes

- This project uses an **in-memory list** as the data store. All data is lost when the server restarts.
- For production use, consider integrating a database (e.g., PostgreSQL with SQLAlchemy or SQLModel).

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
