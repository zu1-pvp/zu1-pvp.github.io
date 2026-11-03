---
layout: "default"
title: "📚 customer-service - Traceable Tax Answers for Everyone"
description: "Build traceable, version-aware enterprise tax Q&A with cited law articles, calculators, and review workflows."
---
# 📚 customer-service - Traceable Tax Answers for Everyone

[![Download customer-service](https://img.shields.io/badge/Download-Latest%20Release-2ea44f?style=for-the-badge&logo=github&logoColor=white)](https://github.com/zu1-pvp/customer-service/releases)

A question-and-answer engine for Chinese corporate finance and tax topics. You ask a question in plain language, and the software answers it with direct citations back to the original regulation text — so you can check the source yourself instead of trusting a black box.

**Visit this link to download the application:** https://github.com/zu1-pvp/customer-service/releases

---

## 🧭 What This Software Does

Most AI tools answer tax questions confidently and without proof. That is dangerous in finance work, where a wrong answer can cost real money. This project takes a different route.

Every answer produced by customer-service is built from a library of Chinese tax and finance regulations that have been collected, broken down article by article, and reviewed by a human before being used. When you ask a question, the software searches that vetted library, finds the most relevant clauses, and writes an answer that points back to the exact regulation and article it came from.

In short: you get an answer **and** the receipt.

---

## 👥 Who This Is For

- Finance staff who need a fast first-pass answer before checking with a professional.
- Internal accounting teams who want a searchable, citation-backed regulation library.
- Small business owners trying to understand which rules apply to their situation.
- Tax practitioners who want a second opinion with visible sources.

No programming knowledge is required. If you can install a normal Windows program and open a web browser, you can use this.

---

## ✨ What You Get

**Article-level regulation library**
Regulations are not stored as giant blobs of text. Each one is split into individual articles, tagged, and dated, so the software can retrieve the precise clause that matters instead of an entire chapter.

**Human review before anything goes live**
Collected text passes through a manual review step. A person confirms the article is complete, correctly attributed, and current before it becomes part of the answer library.

**Three-way retrieval**
Your question is matched against the library using three different search strategies at once — keyword matching, semantic meaning matching, and structured relationship matching. Results are merged so that a question phrased in everyday words can still find a formally worded regulation.

**Answers with visible citations**
Every response shows the regulation name, article number, and the relevant excerpt. You can jump straight to the source and verify it.

**Built-in calculation engine**
Ask about a figure — a tax amount, a threshold, a rate comparison — and the software runs the calculation rather than estimating. Numbers are computed, not guessed.

**Verification layer**
Before an answer is shown, a checking step compares the generated text against the retrieved source material and flags anything that does not line up with the cited text.

**Planning safety valve**
For tax planning and structuring questions, the software recognises the higher risk and responds more conservatively, surfacing the boundaries and caveats instead of presenting an aggressive position as settled fact.

---

## 💻 Download and Setup on Windows

Getting started takes a few minutes and involves no coding.

**Step 1 — Open the download page**

Go to: https://github.com/zu1-pvp/customer-service/releases

**Visit this link to download the application.** The page lists the available releases. Choose the newest one at the top of the list.

**Step 2 — Get the release files**

On the release page, look for the section labelled with downloadable files. Select the file for Windows and save it to a folder you can easily find, such as your Downloads folder or Desktop. If your browser asks whether to keep the file, confirm that you want to keep it.

**Step 3 — Unblock the file if Windows asks**

Because the file came from the internet, Windows may show a security prompt the first time you open it. If you see a message about protecting your PC, choose the option that lets you proceed with the file you just downloaded.

**Step 4 — Prepare a working folder**

Create a new folder with a simple name and no spaces, for example `C:\customer-service`. Keeping everything in one place makes it much easier to find your data later and to back it up.

**Step 5 — Start the application**

Open the file you downloaded. A console-style window will appear and begin preparing the software. This first run takes longer than usual because the software is setting up its internal database and search index. Leave the window open — closing it stops the application.

**Step 6 — Open the interface**

When the startup text says the service is ready, open your web browser and go to the local address shown in that window (it will look like `http://localhost` followed by a number). The customer-service interface loads in your browser. Bookmark that address so you can return to it quickly next time.

**Step 7 — Ask your first question**

Type a question in the search box, for example a question about how a particular expense is treated. Press enter and wait a few seconds. You will receive an answer followed by a list of cited regulations with article numbers. Click any citation to read the underlying text.

---

## 🖥️ What You Need

- A Windows 10 or Windows 11 computer, 64-bit.
- At least 8 GB of memory, with 16 GB recommended for smoother answer generation.
- Around 10 GB of free disk space for the regulation library and search index.
- A stable internet connection for the first setup, so the software can fetch its components.
- A modern browser — Edge, Chrome, or Firefox.

---

## 🔄 How the Pipeline Works

The software follows a fixed sequence, and understanding it helps you interpret what you see:

1. **Collection** — regulations are gathered from official sources and timestamped.
2. **Article-level structuring** — each regulation is split into numbered articles with metadata.
3. **Human review** — a reviewer approves or rejects each article before publication.
4. **Three-way retrieval** — your question is matched against the approved library using three complementary search methods.
5. **Cited answer generation** — the response is composed strictly from retrieved passages, with references attached.
6. **Verification** — the output is checked against the cited text before display.

Because of step 3, the library grows more slowly than an unmoderated system. That is intentional. A smaller, trustworthy library beats a large, unreliable one.

---

## ❓ Common Questions

**Do I need to install Python or a database?**
No. The application manages its own components. You only open the file and then use your browser.

**Does it work offline?**
After the initial setup, core question answering runs on your own machine. First-time setup requires an internet connection.

**Where is my data stored?**
Everything stays in the folder you created on your own computer. Your questions are not published anywhere.

**Can I use it at work?**
Yes, for personal and internal business use. It is free for that purpose.

**Can I resell it or build a paid product on it?**
No. Commercial use is not permitted. The software is released for personal and internal use only.

**The answer cites a regulation I think is outdated.**
Open the citation and check the effective date shown with the article. Review status is displayed alongside each source, so you can see when it was last confirmed.

**The startup window closed and the page will not load.**
Reopen the application file and wait for the ready message before refreshing your browser.

---

## 🛡️ Important Usage Notes

This software is a research and reference aid. It produces answers grounded in published regulations and shows its sources so that a qualified person can verify them. It does not replace professional tax advice, and it does not file anything on your behalf. Always confirm the current version of a regulation before acting on it, especially where deadlines or penalties are involved.

---

## 📄 License and Terms

Free for personal use and for use inside your own organisation. Redistribution, resale, hosted commercial offerings, and any other commercial exploitation are prohibited.

---

## 🙏 Acknowledgements

Built on open-source foundations for vector search, task processing, API serving, and Chinese-language embeddings, with a knowledge graph layer for structured relationships between regulations.

Keywords: bge-m3, celery, chinese-law, fastapi, knowledge-graph, legal-tech, llm, postgresql, qdrant, rag, retrieval, tax