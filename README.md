# Prev_dot_md 📝

A tiny local web app for previewing Markdown — like StackEdit, but without the bloat, ads, or tracking. Just you, your notes, and instant preview.

🔍 What does it do?

- Edit Markdown in one panel, see the rendered preview in the other.
- Auto-saves your note to localStorage (so you don’t lose your genius).
- Toggle dark mode if you’re allergic to light.
- Syntax highlighting for code blocks (thanks to marked.js).
- No backend required for previewing — just a dumb Python server for static files.

🧠 Why?

Because you shouldn’t need an account, a cloud, or a 10MB React bundle to write Markdown. Also, privacy.

🚀 Usage

Clone this repo:

```sh
git clone https://github.com/yourname/prev-md.git
cd prev-md
```

Run the server:

```sh
python server.py
```

It’ll open your browser at [http://localhost:8000](http://localhost:8000). Start typing Markdown. That’s it.

🛠 Tech Stack

- `http.server` — no Flask/Django nonsense
- [marked.js](https://cdn.jsdelivr.net/npm/marked/marked.min.js) — for Markdown parsing
- Static files for the frontend (HTML, CSS, JS)

📁 File Structure

prev-md/
├── prev-md/
│   ├── index.html
│   ├── style.css
│   └── script.js
├── server.py
└── README.md

⚠️ Caveats

- No authentication, no user accounts, no cloud sync. It’s local only.
- If you clear your browser storage, your notes are gone. Don’t blame me.
- If marked.js CDN is down, you’re outta luck.
- No XSS protection — don’t paste evil scripts unless you want to break your own stuff.

🧪 Example Output

Type Markdown like:

```markdown
# Hello World

- This is a list
- **Bold text**
- `inline code`
```

And see it instantly rendered.

🐧 Name Origin

Because it’s a Markdown previewer, and “prev.md” is short, sweet, and not taken.

---

Made with zero analytics, zero tracking, and zero patience for
