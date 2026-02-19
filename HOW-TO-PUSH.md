# How to put your new website on the internet (step-by-step)

Your new website lives in the **docs** folder. To make it show up at **catfong.github.io**, you need to "push" your changes to GitHub. Pushing means: *send the files from your computer to GitHub so the internet can see them.*

---

## Before you start

- You need **Git** on your computer (you might already have it).
- You need to be **logged in to GitHub** (in a browser is fine).
- Your project folder **catfong.github.io** should already be connected to GitHub (it’s a clone or you created the repo there).

---

## Step 1: Open Terminal

- On **Mac**: Open **Terminal** (search for “Terminal” in Spotlight, or find it in Applications → Utilities).
- You’ll see a window with a line of text and a blinking cursor. That’s where you type commands.

---

## Step 2: Go to your website folder

Type this and press **Enter**:

```bash
cd ~/Desktop/github/catfong.github.io
```

That means: “Go into the folder where my website lives.”

---

## Step 3: See what changed

Type:

```bash
git status
```

You’ll see a list of files that changed (things in **docs** and maybe **HOW-TO-PUSH.md**). That’s normal.

---

## Step 4: Tell Git to include the new stuff

Type:

```bash
git add docs/
```

Then:

```bash
git add HOW-TO-PUSH.md
```

(Or, to add everything that changed in one go, you can type: `git add .`)

---

## Step 5: Save a “snapshot” with a message

Type:

```bash
git commit -m "New simple HTML website"
```

That saves this version of the site on your computer and labels it with that message.

---

## Step 6: Send it to GitHub (push)

Type:

```bash
git push
```

- If it asks for your **username**, type your GitHub username and press Enter.
- If it asks for a **password**, use a **Personal Access Token** from GitHub (not your normal password). To get one: GitHub.com → your profile (top right) → **Settings** → **Developer settings** → **Personal access tokens** → create a token, then paste it when Git asks for a password.

When you see something like “Everything up-to-date” or “branch main -> main”, you’re done.

---

## Step 7: Make sure GitHub is showing the right folder

1. On GitHub.com, open your **catfong.github.io** repo.
2. Go to **Settings** → **Pages** (left side).
3. Under **Build and deployment**, **Source** should be **Deploy from a branch**.
4. Under **Branch**, choose **main** (or **master**) and the folder **/docs**, then **Save**.

Now GitHub will show the world whatever is in your **docs** folder. After you push, wait a minute or two, then open **https://catfong.github.io** in your browser to see your new site.

---

## If something goes wrong

- **“git: command not found”**  
  You need to install Git: https://git-scm.com/downloads

- **“Permission denied” or “Authentication failed”**  
  GitHub doesn’t accept account passwords anymore. Use a **Personal Access Token** (see Step 6).

- **“remote: Repository not found”**  
  The folder might not be linked to the right GitHub repo. Tell me the exact message and we can fix it.

---

**Short version:** Open Terminal → `cd ~/Desktop/github/catfong.github.io` → `git add .` → `git commit -m "New website"` → `git push` → set Pages to use the **docs** folder → wait a minute → visit **https://catfong.github.io**.
