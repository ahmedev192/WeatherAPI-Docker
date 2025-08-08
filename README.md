# WeatherDock ☁️

A lightweight **.NET 8 Web API** that serves basic weather data — running inside a **Docker container**.  
This is more of a **"just playing around"** project than anything serious.

---

## ✨ Features
- Simple .NET 8 Web API
- Returns mock weather info (city, temperature, condition)
- Dockerized for quick container testing
- Clean, minimal codebase

---

## 🛠 Tech Stack
- **.NET 8 Web API**
- **C#**
- **Docker**

---

## 📂 Structure
```
WeatherAPI/
│── WeatherAPI.sln
│── WeatherAPI.API/
│   ├── Controllers/
│   ├── Models/
│   ├── Program.cs
│   ├── appsettings.json
│── Dockerfile
│── README.md
```

---

## 🚀 Run Locally

### 1️⃣ Clone repo
```bash
git clone https://github.com/ahmedev192/WeatherAPI-Docker.git
cd WeatherAPI
```

### 2️⃣ Build & run without Docker
```bash
dotnet run --project WeatherAPI.API
```

### 3️⃣ Build & run with Docker
```bash
docker build -t WeatherAPI .
docker run -p 5000:80 WeatherAPI
```

---

## 📡 Example Request
```bash
GET /weather?city=Cairo
```

**Sample Response**
```json
{
  "city": "Cairo",
  "temperature": 32,
  "condition": "Sunny"
}
```

---

## 🧾 Notes
This project is **not a production weather service**.  
It’s just me messing around with **.NET + Docker**.

