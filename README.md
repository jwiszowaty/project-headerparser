# 🌐 Request Header Parser Microservice

A Node.js + Express API that returns the client's IP address, preferred language, and software info by parsing request headers. This project fulfills the FreeCodeCamp “Request Header Parser Microservice” project requirements. :contentReference[oaicite:0]{index=0}

---

## 📚 Table of Contents

- [Features](#features)  
- [API Endpoints](#api-endpoints)  

---

## Features

- **CORS** enabled for FreeCodeCamp test compatibility.
- Responds with:
  - `ipaddress` – user's IP address (from `req.ip` or `x-forwarded-for`)
  - `language` – preferred language (from `Accept-Language` header)
  - `software` – user agent string (from `User-Agent` header)
- Serves a static homepage (`index.html`) with usage instructions.
- Architected with Node.js and Express for clarity and simplicity.

---

## API Endpoints

| Method | Endpoint         | Description                       |
|--------|------------------|-----------------------------------|
| GET    | `/`              | Serves static homepage (UI/demo) |
| GET    | `/api/whoami`    | Returns client’s IP, language, and software info |
