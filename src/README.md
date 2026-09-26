# CaseFlow — Backend (Auth Module)

A legal case-management platform built to centralize case information, hearing tracking, and lawyer collaboration for law firms — replacing physical files, spreadsheets, and individual memory as the source of truth.

This repo currently implements the **authentication module** (register/login), the foundation the rest of the platform builds on.

## Problem it solves

Law firms often have no central system for case status, upcoming hearings, or continuity when a lawyer is unavailable. CaseFlow addresses this by giving lawyers and admin staff a shared, role-based system for case data — with future support for controlled client visibility.

## Tech stack

- Node.js + Express
- MongoDB (Mongoose)
- JWT authentication
- bcrypt password hashing

## Features (current)

- User registration with hashed passwords
- Login with JWT issuance
- Role field (`lawyer` / `admin`) on every user, foundation for role-based access control

## API Endpoints

| Method | Endpoint             | Description         |
|--------|-----------------------|----------------------|
| POST   | `/api/auth/register`  | Create a new user   |
| POST   | `/api/auth/login`     | Log in, receive JWT |

## Setup

```bash
git clone https://github.com/Crownuka/caseflow-backend.git
cd caseflow-backend
npm install
```

Create a `.env` file:
Run locally:
```bash
npm run dev
```

## Roadmap

Full product scope is documented in [`PRD.md`](./PRD.md). Planned next: case management (CRUD), hearing tracking, internal notes, and role-based access control.

## Author

Ezenwanyi Iromba Uka — [GitHub](https://github.com/Crownuka) · [LinkedIn](https://www.linkedin.com/in/ezenwanyi-uka-046a29a7) 
[Medium] (https://medium.com/@queenuka30)