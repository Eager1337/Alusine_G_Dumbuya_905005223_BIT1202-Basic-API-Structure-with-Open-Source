# Limkokwing Library API

**PROG315 — Object-Oriented Programming 2**
Limkokwing University of Creative Technology — Sierra Leone

| Field | Details |
|---|---|
| Student Name | Alusine G. Dumbuya |
| Student ID | 905005223 |
| Programme | BIT1202 |
| Examiner | Amandus Benjamin Coker |
| Semester | 04 — March 2026 to July 2026 |

---

## Description

A console-based Python simulation of a RESTful library management API for Limkokwing University. Demonstrates asynchronous programming with async/await, full type annotations, and concurrent user handling using only Python's standard library — no external packages required.

---

## How to Run

```bash
python main.py
```

Requirements: Python 3.11+ only. No pip install needed.

---

## Endpoints Simulated

| Function | Simulates | Description |
|---|---|---|
| `get_books()` | GET /books | Search by title, author, or category |
| `post_borrow()` | POST /borrow | Borrow a book — sets 14-day due date |
| `put_return()` | PUT /return | Return a book — calculates overdue fine |
| `get_overdue()` | GET /overdue | List all overdue books with fines |

---

## Key Features

- Full type annotations on all functions and variables
- `async def` and `await asyncio.sleep()` on every endpoint
- `asyncio.gather()` simulates 4 concurrent users simultaneously
- Race condition handling — two users cannot borrow the same book
- HTTP-style status codes (200, 201, 400, 403, 404) in every response
- Runs entirely in the terminal — no server, no browser needed

---

## SDG Alignment

**SDG 4 — Quality Education**: Digitising library access at Limkokwing University removes barriers for students, making academic resources accessible from any device at any time.

---

## Project Structure

```
limkokwing-library-api/
├── main.py        # All source code
├── README.md      # This file
└── .gitignore     # Excludes cache and IDE files
```

---

## License

MIT License — free to use, adapt, and distribute.
