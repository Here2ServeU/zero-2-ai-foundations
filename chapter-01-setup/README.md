# Chapter 01 — Set up your computer and say hello

> Matches **Chapter 01** of the Foundations course video. This is the very first step of the whole journey.
> The runnable scripts for this chapter are in this folder.

**Labels:** 💻 Runs free on your laptop

---

## The big idea (in plain words)

Think of the computer as a friend who only does *exactly* what you tell it — no more, no
less. To give it instructions, you need three things:

1. **A language to speak** — we use **Python**, which reads almost like English.
2. **A place to write** — an editor called **VS Code**.
3. **A way to save your work safely** — a tool called **Git**.

In this chapter you'll install those three, then write your very first program: one that makes
the computer say hello to you. That's it. Small on purpose.

## New words (look up anything unfamiliar in the [GLOSSARY](../GLOSSARY.md))

- **Python** — the language we write programs in.
- **VS Code** — the app where we write our code.
- **Terminal** — a text window where you type commands instead of clicking buttons.
- **Run** — to make the computer actually *do* what your program says.

## What you will build

A program called `hello.py` that prints two friendly lines:

```
Hello, Sam!
Let's build something real.
```

(You'll use your own name instead of Sam.)

---

## Let's do it, one small step at a time

### Step 1 — Install Python

1. Go to **python.org/downloads** in your web browser.
2. Click the big yellow **Download Python** button.
3. Open the file you downloaded.
   - **Windows:** **Tick the box that says "Add Python to PATH"** at the *bottom* of the very
     first installer screen, *before* clicking **Install Now**. This one tick saves you many
     headaches later. If the last screen offers **"Disable path length limit,"** click it too.
   - **Mac:** just click through Install.
4. **Check it worked.** Open your **Terminal** (see Step 3 if you don't know how) and type:

   ```bash
   python3 --version     # Mac / Linux
   python --version      # Windows
   ```

   **What you should see:** something like `Python 3.11.5`. Any `3.something` is fine.

> **Windows note:** on Windows the command is usually `python`, not `python3`. Throughout this
> course, whenever you see `python3`, type `python` instead. If neither works, see
> [If something breaks](#if-something-breaks) below — it's almost always the PATH tick.

### Step 2 — Install VS Code (your writing app)

1. Go to **code.visualstudio.com** and click **Download**.
2. Install it like any normal app.
   - **Windows:** take the **User Installer** (the default). It installs just for you and never
     asks for an administrator password. On the "Select Additional Tasks" screen, tick
     **"Add to PATH"** — that's what lets you type `code .` in a terminal later.
   - **Mac:** the download is a zipped app. Unzip it, then **drag `Visual Studio Code` into your
     Applications folder** before opening it. (If you open it straight from Downloads, macOS
     nags you every time.)
3. Open VS Code. When it asks to install the **Python extension**, say **yes** — it makes
   writing Python much friendlier.

### Step 3 — Find your Terminal

The terminal is where you'll tell the computer to *run* your programs.

- **The easy way:** inside VS Code, click the top menu **Terminal → New Terminal**. A text
  panel opens at the bottom. That's it.
- Mac also has a separate **Terminal** app; Windows has **PowerShell**. Either works, but the
  VS Code one is simplest because it sits right next to your code.

### Step 4 — Install Git (saves your work safely)

1. Go to **git-scm.com/downloads**, pick your system, and install.
2. Check it worked — in the terminal type:

   ```bash
   git --version
   ```

   **What you should see:** something like `git version 2.42.0`.

> **Windows: the Git installer asks a *lot* of questions.** That's normal, and the defaults are
> fine except for one. Here's what to pick — click **Next** on anything not listed:
>
> | Screen | What to choose | Why |
> |---|---|---|
> | "Choosing the default editor used by Git" | **Use Visual Studio Code as Git's default editor** | The default is **Vim**, which beginners cannot exit. Change this one. |
> | "Adjusting the name of the initial branch" | **Override... `main`** | Modern default; matches what everyone else uses. |
> | "Adjusting your PATH environment" | **Git from the command line and also from 3rd-party software** (the middle, recommended option) | Lets VS Code and your terminal both find Git. |
> | "Configuring the line ending conversions" | **Checkout Windows-style, commit Unix-style** (the default) | Keeps your files readable to Mac and Linux people. |
>
> If you already installed Git and picked Vim by mistake, you don't have to reinstall — just run
> `git config --global core.editor "code --wait"` in your terminal.

**Mac:** typing `git --version` may pop up a box saying *"The 'git' command requires the command
line developer tools."* Click **Install** and wait a few minutes. That box *is* the installer —
you don't need anything from git-scm.com.

> Don't worry about *using* Git yet. We just want it installed. You'll learn to save and share
> your work in a later chapter.

### Step 5 — Make a folder for this chapter

In the terminal, type these one at a time:

```bash
mkdir hello-project
cd hello-project
```

- `mkdir hello-project` makes a new **folder** called `hello-project`.
- `cd hello-project` moves you *into* that folder, so your work lands there.

### Step 6 — Write your first program

1. In VS Code, open the `hello-project` folder (**File → Open Folder**).
2. Make a new file called **`hello.py`** (File → New File, then save it with that name).
3. Type these three lines exactly (use **your** name):

   ```python
   name = "Sam"
   print(f"Hello, {name}!")
   print("Let's build something real.")
   ```

**What each line says, in plain words:**

1. `name = "Sam"` — Put the word *Sam* into a labeled box called `name`. (A labeled box is a
   **variable**. You can put anything in it.)
2. `print(f"Hello, {name}!")` — `print` means "say this on the screen." The `{name}` part
   means "look inside the box and use what's there," so it says **Hello, Sam!**
3. `print("Let's build something real.")` — Say one more line on the screen.

4. **Save the file** (Ctrl+S, or Cmd+S on Mac). Saving matters — the computer runs the *saved*
   version.

### Step 7 — Run it

In the terminal (make sure you're inside `hello-project`), type:

```bash
python3 hello.py     # Mac / Linux
python hello.py      # Windows
```

**What you should see:**

```
Hello, Sam!
Let's build something real.
```

You just wrote and ran a real program. Every giant system later in this course is built from
small steps exactly like this one: make a file, write code, save, run it.

---

## Try it yourself (mini challenges)

- 🔧 **Change the name.** Put your best friend's name in the box and run it again.
- 🔧 **Add a third line.** Make it print your favorite food. (Hint: copy a `print(...)` line.)
- 🔧 **Break it on purpose.** Delete one of the quotation marks and run it. Read the error.
  Then put the mark back. Seeing errors — and fixing them — is a normal part of coding.

## If something breaks

Installing three tools is the fiddliest part of the whole course. Nothing below means you did
anything wrong — every one of these happens to working developers too.

> ### Try this first, before anything else
>
> **Close your terminal completely and open a new one.** (In VS Code: click the 🗑 trash icon on
> the terminal panel, then **Terminal → New Terminal**. Better still, quit VS Code and reopen
> it.)
>
> A terminal only learns where your tools live *at the moment it opens*. Install something while
> a terminal is already open, and that terminal will keep insisting the tool doesn't exist. This
> single step fixes most "command not found" problems, and people lose hours to it.

### Python problems

- **`python3: command not found` (Mac/Linux)** → Python isn't installed, or the installer didn't
  finish. Redo Step 1, then open a fresh terminal.
- **`'python' is not recognized as an internal or external command` (Windows)** → Almost always
  the **"Add Python to PATH"** tick from Step 1. You don't need to uninstall anything: run the
  same installer again, choose **Modify** (or **Repair**), and make sure PATH is selected. Then
  open a *new* terminal.
- **Windows: `python3` doesn't work but `python` does** → That's correct and expected. On
  Windows the command is `python`. Wherever this course writes `python3`, type `python`.
- **Windows: typing `python` opens the Microsoft Store**, or says *"Python was not found; run
  without arguments to install from the Microsoft Store"* → Windows ships a fake `python` that
  only advertises the Store. Turn it off: **Settings → Apps → Advanced app settings → App
  execution aliases**, then switch **off** both `python.exe` and `python3.exe`. Open a new
  terminal and try again.
- **Windows: `py --version` works but `python` doesn't** → PATH again. Either fix it with
  Modify/Repair above, or simply use `py` in place of `python` for the rest of the course.
- **Windows: "Windows protected your PC" blue box when you open the installer** → Click **More
  info → Run anyway**. It appears because the file is newly downloaded, not because it's unsafe;
  just make sure you downloaded it from **python.org**.
- **Mac: `pip install` later fails with an SSL / certificate error** → Open your Applications
  folder, go into the **Python 3.x** folder, and double-click **Install Certificates.command**.
  It takes a few seconds and fixes it permanently.
- **Two different Python versions answer in two different terminals** → You have more than one
  Python installed (common on Mac with Homebrew, or on Windows with a Store copy). It's not
  harmful. Pick one and stay consistent; in VS Code use **Ctrl+Shift+P → Python: Select
  Interpreter** and choose the one from python.org.

### VS Code problems

- **Windows: "Windows protected your PC" when installing** → Same as above: **More info → Run
  anyway**.
- **Windows: it asks for an administrator password you don't have** → You downloaded the
  *System* installer. Get the **User Installer** from code.visualstudio.com instead; it installs
  for just you and needs no password.
- **Mac: "VS Code can't be opened because Apple cannot check it for malicious software"** →
  Right-click (or Control-click) the app icon and choose **Open**, then **Open** again in the
  box. You only do this once.
- **`code .` says "command not found"** → **Mac:** open VS Code, press **Cmd+Shift+P**, type
  `shell command`, and pick **"Shell Command: Install 'code' command in PATH."** **Windows:**
  reinstall and tick **"Add to PATH."** (You never actually need `code .` in this course — it's
  just convenient.)
- **VS Code doesn't offer the Python extension, or your code has no colors** → Click the
  **Extensions** icon in the left bar (four little squares), search **Python**, and install the
  one from **Microsoft**.
- **VS Code says "Select a Python interpreter" or can't find Python** → Press
  **Ctrl+Shift+P** (**Cmd+Shift+P** on Mac), type `Python: Select Interpreter`, and pick the
  version you installed in Step 1. If the list is empty, Python isn't on your PATH — see the
  Python section above.
- **Windows: the VS Code terminal isn't the one you expected** → Click the **∨** arrow next to
  the **+** on the terminal panel and choose **PowerShell**, **Command Prompt**, or **Git Bash**.
  Any of them works for this course. PowerShell is the normal choice.
- **Windows: PowerShell says "running scripts is disabled on this system"** → Windows blocks
  script files by default. Fix it once, in PowerShell:

  ```powershell
  Set-ExecutionPolicy -Scope CurrentUser RemoteSigned
  ```

  Answer **Y** when it asks. You won't hit this in Chapter 01, but you will in Chapter 05 when
  you switch on a virtual environment — so it's worth doing now.

### Git problems

- **`git: command not found` / `'git' is not recognized`** → Open a brand-new terminal first
  (see the box at the top). If it still fails on **Windows**, reinstall from git-scm.com and, on
  the PATH screen, choose **"Git from the command line and also from 3rd-party software."**
- **Mac: a box appears asking to install "command line developer tools"** → Click **Install**
  and wait. That box *is* how Git gets installed on a Mac; nothing is wrong.
- **The Git installer asked a dozen questions and I clicked through them (Windows)** → The only
  answer that really matters is the editor, and you can change it afterwards:

  ```bash
  git config --global core.editor "code --wait"
  ```

- **You're stuck inside a strange full-screen editor you can't quit (Vim)** → Press **Esc**,
  then type `:q!` and press **Enter**. Then run the `core.editor` command above so it never
  happens again.
- **Git asks "who are you?" later on** → Tell it once, with your own name and email:

  ```bash
  git config --global user.name "Your Name"
  git config --global user.email "you@example.com"
  ```

### Running `hello.py` problems

- **`can't open file 'hello.py'`** → You're not in the right folder. Type `cd hello-project`
  first. Type `ls` (Mac/Linux) or `dir` (Windows) to see whether `hello.py` is really there.
- **Windows: the file is actually named `hello.py.txt`** → File Explorer hides extensions, so
  Notepad quietly adds `.txt`. Turn the hiding off: in File Explorer, **View → Show → File name
  extensions**, then rename the file to `hello.py`. Saving from **VS Code** avoids this
  completely.
- **`SyntaxError`** → A typo. Most often a missing quote `"` or parenthesis `)`. Compare your
  three lines to the example, character by character. Watch out for **curly quotes** (`"` `"`)
  if you copied the code out of a document — Python only accepts straight ones (`"`).
- **`IndentationError: unexpected indent`** → One of your lines starts with a stray space. All
  three lines should start hard against the left edge.
- **Nothing prints** → Make sure you *saved* the file (Ctrl+S / Cmd+S) before running it.
- **The terminal shows a path like `PS C:\Users\You>` and nothing you type works** → You may be
  in the middle of a command that's waiting for you. Press **Ctrl+C** to cancel and get a fresh
  prompt back.

## What you just learned

- You installed the three core tools every developer uses: **Python**, **VS Code**, and
  **Git**.
- You found and used the **terminal**.
- You created a folder, wrote a Python file, and **ran** your first program.
- You learned that **variables** are labeled boxes and `print` shows things on screen.
- You learned that **errors are normal** and tell you what to fix.

## Where to next

➡ [Chapter 02 — Your very first tiny AI experiment](../chapter-02-data). You'll make the
computer *learn from examples* for the first time.
