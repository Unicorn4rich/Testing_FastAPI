# 🚀 FastAPI CRUD API

This is a simple CRUD (Create, Read, Update, Delete) API built using [FastAPI](https://fastapi.tiangolo.com/). It is deployed on Vercel and is publicly accessible for use and testing.

🔗 **Base URL**: [https://testing-api-fast.vercel.app/](https://testing-api-fast.vercel.app/)

---

## 📌 Features

- ✅ `GET`: Retrieve all names
- ➕ `POST`: Add a new name
- ❌ `DELETE`: Remove a name
- 🔄 `PUT`: Update an existing name

---

## 📂 API Endpoints

### 1. `GET /`

**Description**: Returns a list of all names.

**URL**:  
`https://testing-api-fast.vercel.app/`

**Response Example**:

```json
["Shoaib", "Ali", "Ahmed"]
```

---

### 2. `POST /`

**Description**: Adds a new name to the list.

**URL**:  
`https://testing-api-fast.vercel.app/`

**Request Body**:

```json
{
  "name": "Zain"
}
```

**Response Example**:

```json
["Shoaib", "Ali", "Ahmed", "Zain"]
```

---

### 3. `DELETE /data/{name}`

**Description**: Deletes the specified name from the list.

**URL Format**:  
`https://testing-api-fast.vercel.app/data/Ahmed`

**Response Example**:

```json
["Shoaib", "Ali"]
```

---

### 4. `PUT /{name}`

**Description**: Updates an existing name with a new one.

**URL Format**:  
`https://testing-api-fast.vercel.app/Ali`

**Request Body**:

```json
{
  "name": "Bilal"
}
```

**Response Example**:

```json
["Shoaib", "Bilal", "Ahmed"]
```

---

## 🛠 Tech Stack

- Python 3.x 🐍
- FastAPI ⚡
- Deployed on Vercel 🚀

---

## 📎 Notes

- This API uses an in-memory list (`names`) as its data source.
- The data resets to default whenever the server restarts.
- Intended for learning/demo purposes only.

---

## 📬 Contact

Feel free to raise an issue or reach out if you have any questions or suggestions.

---

