# 🌐 Request Header Parser Microservice

A Node.js and Express.js API that returns your IP address, preferred language, and software (user-agent) info using the HTTP request headers. This project fulfills the FreeCodeCamp “Request Header Parser Microservice” requirement from the Back End Development and APIs certification.

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
