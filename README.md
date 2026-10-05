<div align="center">

<img src="banner.png" alt="DAVE AI Office" width="100%">

### Digital&nbsp;·&nbsp;Autonomous&nbsp;·&nbsp;Virtual&nbsp;·&nbsp;Employees

**An office of AI employees that runs on your own computer.**
<br>You give one sentence. Six specialists pass the work desk to desk — and you watch.

<br>

[![Download](https://img.shields.io/badge/⤓_Download_for_Windows-3a9bf4?style=for-the-badge&logoColor=white)](../../releases/latest)
[![Guide](https://img.shields.io/badge/5_minute_guide-0c1420?style=for-the-badge)](https://YOURSITE.com/start.html)

![version](https://img.shields.io/badge/version-1.0.0-3a9bf4)
![platform](https://img.shields.io/badge/Windows-10_|_11-3a9bf4)
![free](https://img.shields.io/badge/price-free-7ee08a)
![telemetry](https://img.shields.io/badge/telemetry-none-7ee08a)
![account](https://img.shields.io/badge/account-not_required-7ee08a)

</div>

---

## The floor

```
   ┌──────────┐  ┌──────────┐  ┌──────────┐  ┌──────────┐  ┌──────────┐
   │  KARTIK  │  │ JAINISH  │  │  PRIYA   │  │   VASU   │  │   PUJA   │
   │ research │  │  build   │  │    QA    │  │  review  │  │  memory  │
   │    ▓▓▓   │  │   ▓▓▓▓   │  │    ▓▓    │  │    ▓▓    │  │    ▓     │
   └────┬─────┘  └────┬─────┘  └────┬─────┘  └────┬─────┘  └────┬─────┘
        │             │             │             │             │
        └─────────────┴──────┬──────┴─────────────┴─────────────┘
                             │
                      ┌──────┴──────┐
                      │    DAVE     │   ← one sentence in
                      │  front desk │
                      └─────────────┘
```

Ten desks in all. Hire whoever you need.

---

## One job, start to finish

```mermaid
flowchart LR
    A([your sentence]) --> B[Kartik<br/>research]
    B --> C[Jainish<br/>build]
    C --> D{Priya<br/>QA}
    D -->|pass| E{Vasu<br/>review}
    D -->|fail| C
    E -->|pass| F{your Python<br/>rule}
    E -->|fail| C
    F -->|fail| C
    F -->|pass| G([a file you can open])
    G --> H[Kajal<br/>writes the lesson down]

    style A fill:#0c1420,stroke:#3a9bf4,color:#eaf3fd
    style G fill:#0c1420,stroke:#7ee08a,color:#eaf3fd
    style D fill:#1a1608,stroke:#e8c46a,color:#eaf3fd
    style E fill:#1a1608,stroke:#e8c46a,color:#eaf3fd
    style F fill:#0c1a16,stroke:#6fd5b0,color:#eaf3fd
```

Weak work goes **back to the builder**, on its own, before it ever reaches you.
You get the second draft.

---

## What that looks like

```console
$ build a booking page for my restaurant                    effort: deep

  ●  Kartik    gathered findings                             3,712 tokens
  ●  Jainish   wrote index.html  (4.1 KB)                   11,796 tokens
  ●  Priya     checked it point by point     VERDICT: pass   9,589 tokens
  ●  Vasu      scored it 9/10 · one fix wanted               9,488 tokens
  ●  Dev       ran your Python  VERDICT: fail  no <footer>       0 tokens
  ●  Jainish   fixed it and saved again  (4.6 KB)           18,337 tokens
  ●  Puja      kept 1 note for next time                     2,084 tokens

  ✓ index.html saved  ·  7 steps  ·  3 verdicts  ·  the office is free again
```

Every number is on the record, and you can pause it mid-job.

---

## The six who clock in

| | Desk | What they do |
|---|---|---|
| ![](https://img.shields.io/badge/-5ec8d8?style=flat-square) | **Kartik** · Research | Finds out what the job needs before anyone builds |
| ![](https://img.shields.io/badge/-7ee08a?style=flat-square) | **Jainish** · Engineering | Writes the code, the page, the document |
| ![](https://img.shields.io/badge/-e8c46a?style=flat-square) | **Priya** · QA | Checks the work against the request, point by point |
| ![](https://img.shields.io/badge/-e2865f?style=flat-square) | **Vasu** · Review | Scores it out of ten and names the fix |
| ![](https://img.shields.io/badge/-a98ce0?style=flat-square) | **Puja** · Memory | Keeps what will still matter in a month |
| ![](https://img.shields.io/badge/-6fd5b0?style=flat-square) | **Kajal** · Learning | Turns finished jobs into rules for the next one |

---

## Write a rule once. It checks every build for ever.

```python
def check(request: str, work: str) -> tuple[bool, str]:
    """Every page this office builds must have a footer."""
    if "<footer" not in work.lower():
        return False, "no <footer> element in the page"
    return True, "footer present"
```

Twelve lines, no tokens, running in its own process — so a mistake in your code
is reported and skipped, never a job that hangs. Or describe the rule in plain
English and let an agent judge it. Both work.

---

## Bring your own brain

DAVE sells no tokens, so it can never mark them up.

<table>
<tr>
<td width="33%" valign="top">

**One key, everyone**

Paste a single API key and the whole floor uses it. Most people start here and
stay.

</td>
<td width="33%" valign="top">

**One brain per role**

A strong model for building, a cheap fast one for QA and memory. The bill drops;
the quality doesn't.

</td>
<td width="33%" valign="top">

**Every desk its own**

Any agent can have its own provider, model, tool or key. Mix them however you
like.

</td>
</tr>
</table>

The desk wins over the role, and the role wins over the office — so one change
never breaks the rest.

Works with an **API key** (Gemini, OpenAI, Anthropic, or any OpenAI-compatible
endpoint), a **local model** (Ollama — no key, no bill, never busy), or a
**coding tool you already pay for**. Tell DAVE where it lives and what to run;
nothing is hard-coded, so a new tool works without a new version.

---

## Private because of how it is built

```
    your machine                                     the provider you chose
  ┌───────────────────────────────┐                 ┌──────────────────────┐
  │  tasks · files · memories     │                 │                      │
  │  keys, in an encrypted vault  │ ───────────────▶│   your prompt only   │
  │  logs · lessons · the office  │                 │                      │
  └───────────────────────────────┘                 └──────────────────────┘

                        no server of ours, anywhere in that line
```

No account. No sign-in. No telemetry. No crash reporting. Deleting the data
folder deletes all of it — there is no copy to ask us for.

---

## Install

<table>
<tr><td width="50"><b>01</b></td><td>

Download **[DAVE-Setup-v1.0.0.exe](../../releases/latest)**

</td></tr>
<tr><td><b>02</b></td><td>

Run it. Windows shows a SmartScreen warning because the app is not code-signed
yet — click **More info**, then **Run anyway**

</td></tr>
<tr><td><b>03</b></td><td>

Open the app. Setup asks for a key and a folder for your agents' work

</td></tr>
<tr><td><b>04</b></td><td>

Give it a task and watch the floor

</td></tr>
</table>

About five minutes, and the first task costs nothing on a free key.

| What | Where it lives |
|---|---|
| Settings, keys, memories, logs | `%APPDATA%\DAVE AI Office` |
| What your agents produce | the folder you pick during setup |

Uninstalling removes the app. **Your work stays where you put it.**

---

<details>
<summary><b>What it does not do — and why</b></summary>

<br>

Every one of these is a choice or a date, not a surprise.

- **Windows only for now.** One platform tested properly beats three done
  badly. macOS and Linux run from source today; packaged builds are next.
- **It runs while your PC is on.** That is exactly what keeps your work on your
  own machine. A cloud office is being built for people who need it round the
  clock.
- **It reads text, code, CSV and PDF.** Word and Excel are on the list. Until
  then it says so plainly rather than half-reading them.
- **It cannot write .pptx, .docx or .xlsx directly.** It delivers a script that
  makes the file, and tells you that is what it did.
- **It says "I can't read images" instead of guessing.** A wrong description of
  your photo is worse than an honest no.
- **Ten desks, three jobs at once.** Sized for one person's real work, so your
  laptop stays usable while the office runs.
- **The model you pick decides the quality.** DAVE shows you exactly what each
  one produced and what it cost, so you can choose well.
- **English interface for now.** Every word is a plain string, so translations
  are welcome.

</details>

<details>
<summary><b>Something broken?</b></summary>

<br>

Open an issue with **what you did** and **what you saw**. That is worth hours.

The log is at `%APPDATA%\DAVE AI Office\dave.log` — the last twenty lines
usually say what happened.

</details>

<details>
<summary><b>Licence and ownership</b></summary>

<br>

Created and maintained by **Dhruvil Dave**. See [LICENSE.txt](LICENSE.txt).

Free to use for personal or commercial work, on as many of your own machines as
you like. **What it makes is yours** — we claim nothing in the output.

The artwork, the characters, the logo and the name stay with the author. The
office art was made for this project, and the characters are not images at all:
they are drawn by code, shape by shape, while the app runs.

AI providers and coding tools named here belong to their owners. DAVE works
with them; it is not affiliated with, endorsed by, or a product of any of them.

</details>

---

<div align="center">

### Open your office tonight.

Six specialists are already at their desks, waiting for a job.

[![Download](https://img.shields.io/badge/⤓_Download_free-3a9bf4?style=for-the-badge)](../../releases/latest)

<sub>© 2026 Dhruvil Dave · Runs on your computer · Your keys, your bill, your data</sub>

</div>
