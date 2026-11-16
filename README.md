# 28 Analysis — made by kitaryo28

A chess.com-style chess analysis website: game review with a voice coach (Kuro the cat), Stockfish 19 NNUE engine, weakness report from many games, puzzles with endless levels, opening trainer and explorer, tablebase, library with notes, spaced-repetition mistake review, bots with faces/voices/clocks, Learn lessons (basics to pro), themes (dark / light / midnight blue).

---
## START FROM ZERO (step by step)

### Step 1 - Make a GitHub account
Go to https://github.com/signup and create a free account. Remember your **username**.

### Step 2 - Download the 2 engine files (this makes Stockfish strong)
Open each link; the file downloads:
1. https://github.com/nmrugg/stockfish.js/releases/download/v19.0.1/stockfish-19-lite-single.js
2. https://github.com/nmrugg/stockfish.js/releases/download/v19.0.1/stockfish-19-lite-single.wasm

**Do NOT rename them.** Keep the names exactly as they are.
(If you skip this step the site still works with a weaker engine.)

### Step 3 - Create the repository
1. Open https://github.com/new
2. Repository name: `28-analysis`
3. Choose **Public**
4. Tap **Create repository**

### Step 4 - Upload everything (all in the same place, no folders)
1. On the new empty repo page tap **uploading an existing file**. (On a phone: open github.com in Chrome -> menu -> **Desktop site**.)
2. Upload ALL of these:
   - index.html
   - manifest.webmanifest
   - sw.js
   - icon.svg
   - icon-192.png
   - icon-512.png
   - README.md
   - stockfish-19-lite-single.js   (from Step 2)
   - stockfish-19-lite-single.wasm (from Step 2)
3. Wait until all files are listed, then tap **Commit changes**.

### Step 5 - Turn the website on
1. Open the repo -> **Settings** -> **Pages**.
2. Under *Build and deployment* choose **Deploy from a branch**.
3. Branch: **main**, folder: **/ (root)** -> **Save**.
4. Wait 1-2 minutes. Your site: `https://YOUR-USERNAME.github.io/28-analysis/`

### Step 6 - Check it works
Open your site. Top-right shows **Stockfish 19 NNUE** when the new engine is running.
(**Stockfish engine** = older engine, **Built-in engine (lite)** = weak fallback: re-check that both engine files were uploaded with the exact names.)

### Step 7 - Install like an app (optional)
Phone browser menu -> **Add to Home screen / Install app**.

### Updating later
Repo -> **Add file -> Upload files** -> upload the new `index.html` -> **Commit changes** -> wait 1-2 minutes -> hard-refresh the site.

---
## Features and notes
- **Analyze:** paste any PGN, import from Lichess / Chess.com (works on your GitHub site), "Find my weaknesses" over 5-15 games, library with notes, opening name, phase accuracy and rough rating, tablebase for 7 pieces or fewer.
- **Opening explorer:** needs a free Lichess token (https://lichess.org/account/oauth/token, no scopes). Paste it in Settings -> Coach & engine.
- **Puzzles:** endless levels per difficulty (generated with Stockfish), Online Lichess puzzles, daily puzzle, "Review my mistakes" (spaced repetition).
- **Voice:** uses your phone's text-to-speech. Settings -> Coach & engine -> Voice (Test / Test bot).
- Data (library, progress, settings) is saved only in your own browser.
