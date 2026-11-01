
# Personal Journal Manager

A menu-driven Python console application for maintaining a personal journal in a text file. This project demonstrates Object-Oriented Programming (OOP), file handling, and exception handling.

## Features

1. **Add a New Entry** — appends a journal entry with the current date and time.
2. **View All Entries** — displays all saved entries.
3. **Search for an Entry** — searches entry text or timestamps using a keyword or date.
4. **Delete All Entries** — asks for confirmation before deleting `journal.txt`.
5. **Exit** — closes the application.

## Requirements

- Python 3.8 or newer
- No third-party packages required

## How to Run

1. Download or clone this repository.
2. Open a terminal in the project folder.
3. Run:

   ```bash
   python main.py
   ```

   On some systems, use `python3 main.py`.

The program creates `journal.txt` automatically when the first entry is added. The journal file is created in the current working directory.

## Project Structure

```text
personal-journal-manager/
├── main.py
├── README.md
└── .gitignore
```

## File Handling Modes Demonstrated

- `a` — append new entries and create the file if it does not exist.
- `r` — read saved entries.
- `unlink()` — remove the file after confirmation.

The project uses `try/except` blocks to handle missing files, permission errors, and other operating-system errors gracefully.

## OOP Structure

The `JournalManager` class encapsulates the journal file operations in instance methods. The `main()` function creates an object of this class and uses a loop to show the menu until the user exits.

## Assumptions

- Each journal entry is stored with a timestamp.
- Entries are separated by blank lines.
- Search is case-insensitive and checks the timestamp and entry text.
- Deletion removes the whole `journal.txt` file only after the user types `yes`.
- If the file does not exist, viewing, searching, or deleting shows a helpful message instead of crashing.

## GitHub Upload

Create a new repository on GitHub, for example `personal-journal-manager`. Then run these commands from this folder (replace the URL with your own repository URL):

```bash
git init
git add main.py README.md .gitignore
git commit -m "Add Personal Journal Manager project"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/personal-journal-manager.git
git push -u origin main
```

Do not include private information in your journal or commit your personal `journal.
