# 📘 SQL Sales Analysis Helper Guide

A simple SQL project to help AltSchoolers and beginner analysts learn how to write and **understand SQL queries**, not just copy them. This repo covers five foundational SQL challenges and explains each one in clear, beginner-friendly language.

---

## 💡 Why I Built This

During my SQL assessment at AltSchool Africa, I ran into a few challenges. One of them was a frustrating bug with the `prettytable` package. I had to figure out the fix all thanks to our instructor who gave us some hints to resolve the issue.

After solving it, I thought:

> “What if I made this easier for someone else?”

So I created this repo to **share the queries, the fixes, and the logic behind each answer**. It’s my way of learning in public and helping others grow with me.

---

## 🛠️ Before You Begin

To run this project in Google Colab or Jupyter Notebook:

- Use this magic command before every SQL query:
  %%sql result <<
- Don’t modify, add, or remove cells in restricted assessment notebooks.
- Always run all initialization/setup cells **before** attempting the questions.

### ⚠️ PrettyTable Bug Fix

If you run into this error: 
KeyError: 'PLAIN_COLUMNS'

Here’s how to fix it:

1. Open a **new notebook** (not the assessment one).
2. Run this:
   ```python
   !pip install prettytable==3.10.0 --force-reinstall

Restart the runtime (Runtime > Restart runtime)

Return to your main notebook, and run everything again.

Worked like magic 💫


📁 Files
queries_and_solutions.ipynb – Contains Questions 1–5 with working SQL code.

EXPLANATION.md – Human-readable explanation for each query and why it works.

README.md – What you're reading now 🙂


📬 How To Use
Run the notebook in Colab.

Refer to EXPLANATION.md as a learning companion.

Fork this repo and try your own tweaks.

Share with someone else who's learning!


🙌 Acknowledgments
Shoutout to AltSchool Africa, the SQL bugs that nearly had me giving up 😂, and the amazing data community learning and sharing every day.


🌍 Let’s Connect
GitHub: Gana Joshua Danlami

X (Twitter): @JoshofTP

“You don’t need to know everything to start, just enough to help someone behind you.”

#SQL #AltSchoolAfrica #LearningInPublic #GanaJoshuaDanlami





