# 📄 apa-writer — APA 7th Edition Document Generator

A Claude skill that generates complete academic documents in **APA 7th edition format** as downloadable `.docx` files. Give it a topic, upload your sources, paste links — Claude handles the rest.

**Supports:** Spanish · English · Brazilian Portuguese

---

## ✨ What it does

1. **Asks you a few questions** about your topic, work type, and sources
2. **Collects content** from PDFs, Word files, URLs, web research, or text you paste
3. **Generates a fully formatted `.docx`** — cover page, table of contents, abstract, body, and references — all in correct APA 7th edition style
4. **Verifies the output** visually before delivering the file

---

## 🗂️ Supported document types

| Type | Structure |
|---|---|
| **Student paper** | Cover page → TOC → Abstract → Body → Conclusions → References |
| **Scientific article** | Cover page → Abstract → Introduction → Method → Results → Discussion → Conclusions → References |
| **Thesis / degree project** | Extended cover page → Chapters → Theoretical framework → Methodology → Results → Conclusions → Recommendations → References → Appendices |

---

## 📥 Accepted source formats

You can give the skill content in any of these formats — or combine them:

| Format | Example |
|---|---|
| PDF file | Upload your research PDFs directly |
| Word document (.docx) | Upload notes or drafts |
| URL / link | Paste any webpage or article link |
| Plain text | Copy-paste paragraphs, notes, or quotes |
| Web research | Ask Claude to search and find sources automatically |
| Image of a document | Upload a photo or screenshot of printed material |

---

## 🌐 Language adaptations

The skill applies correct APA conventions per language:

| Rule | 🇪🇸 Spanish | 🇺🇸 English | 🇧🇷 Portuguese (BR) |
|---|---|---|---|
| 2 authors | García **y** López | García **&** López | García **e** López |
| Narrative cite | García (2020) **afirma** | García (2020) **states** | García (2020) **afirma** |
| No date | s.f. | n.d. | s.d. |
| Abstract label | Resumen | Abstract | Resumo |
| Keywords label | Palabras clave: | Keywords: | Palavras-chave: |
| Title capitalization | Primera palabra únicamente | All Major Words | Primeira palavra únicamente |
| Date format | 2020, 23 de noviembre | 2020, November 23 | 2020, 23 de novembro |
| Edition | 3.ª ed. | 3rd ed. | 3.ª ed. |

---

## 📋 APA format applied automatically

Every generated document includes:

- ✅ Times New Roman 12 pt
- ✅ 2.54 cm margins on all sides
- ✅ Double line spacing, no extra space between paragraphs
- ✅ Left alignment (not justified)
- ✅ 0.5" first-line indent on body paragraphs
- ✅ Page numbers in top-right corner from page 1
- ✅ Cover page with all required fields
- ✅ Table of contents with correct page numbers
- ✅ Abstract ≤ 250 words
- ✅ In-text citations (parenthetical and narrative)
- ✅ Reference list in alphabetical order with hanging indent

---

## 💬 How to trigger it

Just talk naturally. The skill activates on phrases like:

> *"I need to write a paper on cement in APA format"*
> *"Help me structure a research document using APA norms"*
> *"Create an APA thesis about renewable energy"*
> *"I have these PDFs — make a university assignment from them in APA"*
> *"Write an IMRD article about machine learning, APA style"*

---

## 🚀 Example workflow

```
You:    I need to write a student paper on Bitcoin for my Economics class.
        I have two PDFs and I want you to also search the web for more sources.

Claude: Got it. A few quick questions before I start:
        1. What's your name? (for the cover page)
        2. Institution and course name?
        3. Professor's name and due date?
        4. How many pages approximately?
        5. Language: Spanish, English, or Portuguese?

You:    [answers]

Claude: [reads your PDFs + searches the web for 4+ academic sources]
        [generates the .docx with cover page, TOC, abstract, body, references]
        [verifies formatting visually]
        [delivers the file]
        "Here's your document (8 pages, 6 sources). Where would you like to save it?"
```

---

## 📁 Repository structure

```
apa-writer/
├── SKILL.md      # Skill instructions for Claude
└── README.md     # This file
```

---

## 🔧 Installation

### Option A — Claude Desktop (Cowork)
1. Download `apa-writer.skill`
2. Place it in your Claude skills folder (e.g., `C:\Claude\[RULES]\`)
3. Restart Claude Desktop — the skill is ready

### Option B — Manual (SKILL.md only)
1. Copy `SKILL.md` into your local skills directory
2. Reference it from your Claude global instructions or system prompt

---

## ⚠️ Important notes

- Claude will **never fabricate citations** — only real, found sources are used
- If sources are insufficient, Claude will tell you and ask for more material
- Cover page fields left as `[placeholder]` must be filled in manually if you didn't provide them
- The file is saved locally first; Claude asks you where to put it before copying

---

## 📌 Minimum sources by document type

| Document type | Minimum sources |
|---|---|
| Student paper | 4 |
| Scientific article | 6 |
| Thesis | 10 |

---

## 🙋 FAQ

**Can I upload multiple PDFs at once?**
Yes. Upload as many as you need — Claude reads them all and consolidates the information.

**Can I mix PDFs with web research?**
Yes. You can provide files, paste links, and ask Claude to search the web — all in the same request.

**What if I don't have any sources?**
Just give Claude the topic and ask it to find sources. It will search the web for academic and reliable material automatically.

**Can I request specific sections?**
Yes. In the brief phase, mention any sections your professor requires and Claude will include them.

**What language is the document generated in?**
The language you specify during the brief (Spanish, English, or Brazilian Portuguese). APA citation rules adapt accordingly.

---

## 📜 License

MIT — free to use, modify, and share.

---

*Built on Claude's skill system. Powered by the `docx` npm library and APA 7th edition guidelines.*
