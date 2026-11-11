# Password_Strenth_Checker

A lightweight desktop application built with Python and Tkinter that checks and visually displays password strength in real time.

## Features

* **Real-Time Validation:** Evaluates password strength immediately as you type.
* **Visual Progress Bar:** Updates bar fill width and color across five strength tiers.
* **5-Tier Rating System:** Categorizes passwords from **Very Weak** (Red) to **Very Strong** (Green).
* **Zero External Dependencies:** Uses only Python's built-in `tkinter` and `re` modules.

## How Scoring Works

The meter evaluates passwords based on **5 criteria**, awarding 1 point for each condition met:
1. **Length:** At least 8 characters long.
2. **Lowercase Letters:** Contains at least one lowercase letter (`a-z`).
3. **Uppercase Letters:** Contains at least one uppercase letter (`A-Z`).
4. **Numbers:** Contains at least one digit (`0-9`).
5. **Special Characters:** Contains at least one symbol (`_ @ $ ! % * ? & #`).

| Criteria Met | Strength Label | Bar Fill | Indicator Color |
| :--- | :--- | :--- | :--- |
| 0 – 1 | Very Weak | 20% | Red (`#ff4d4d`) |
| 2 | Weak | 40% | Orange (`#ff944d`) |
| 3 | Moderate | 60% | Yellow (`#ffd11a`) |
| 4 | Strong | 80% | Light Green (`#99cc33`) |
| 5 | Very Strong | 100% | Green (`#33cc33`) |

## Getting Started

### Prerequisites
* **Python 3.8 or higher** installed on your system.

### Installation & Usage
1. Save the Python code as `app.py`.
2. Open your terminal or command prompt in the project folder.
3. Run the application:
   ```bash
   python app.py
   ```
   *(On Linux, if Tkinter is missing, install it via `sudo apt-get install python3-tk`.)*

## Project Structure

```text
password-strength-meter-python/
├── app.py              # Main Tkinter GUI application
├── requirements.txt    # Dependency notes
└── README.md           # Project documentation
```
