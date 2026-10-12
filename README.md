# Cascade Lab

A single-page trainer for the **pneumatic cascade method** (sequential control with 2 or 3 double-acting cylinders).

1. **Sequence** – pick 2 or 3 cylinders and type a sequence such as `A+ B+ B- A-`.
2. **Cascade table** – click `⋮` between actions to split them into groups, then fill in each ack signal (`a1`, `b0`…) and where it goes. **Check table** marks every cell.
3. **Wire it, then run it** – click a port, then another port or a group line, to connect them. Hold **START** (or press Space) to run the simulation. Coloured lines show which group line the air comes from; signal conflicts flash red.
4. **Test circuit** runs one full cycle automatically and explains what's wrong if it fails.

Answers: **Show answer** (table) and **Show wiring** (circuit).

## Sessions

- Your work autosaves in the browser.
- **Copy link** – a link that opens your exact session (table + wiring).
- **Copy exercise link** – same sequence, but a blank table, no wiring, and the answer buttons hidden. Send this one to a friend.
- **Save file / Open file** – keep sessions as `.json` files.

Everything runs in the browser; there is no server and nothing is uploaded.

## Put it on GitHub Pages

1. Create a new public repository on GitHub, e.g. `cascade-lab`.
2. Upload `index.html` (and this README) to the repository root and commit.
3. Go to **Settings → Pages**. Under *Build and deployment*, set **Source** to *Deploy from a branch*, choose `main` and `/ (root)`, then **Save**.
4. After a minute the site is live at `https://<your-username>.github.io/cascade-lab/`.

From a terminal instead:

```bash
git init cascade-lab && cd cascade-lab
cp /path/to/index.html /path/to/README.md .
git add . && git commit -m "Cascade Lab"
git branch -M main
git remote add origin https://github.com/<your-username>/cascade-lab.git
git push -u origin main
```

Then turn on Pages as in step 3.
