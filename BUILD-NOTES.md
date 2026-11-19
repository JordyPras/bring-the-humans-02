# Bring the humans again — build notes

Entry for `bring-the-humans-02` ("Bring the humans again"), $1,000 onchain USDC,
50 places paid (1st $150, 2nd $80, 3rd $50, 4th–10th $20, 11th–25th $17,
26th–50th $13). Entries close Sat 2026-11-21 17:30 WIB (2026-11-21T10:30:00Z).
Result due 2026-12-06. Score = verified human signups bound to the entrant's
referral code in the window; final check runs 30h past the deadline.

Built 2026-11-19 ~19:20 WIB by a Muse subagent session (parent agent to bundle
+ submit). Kit: `../bring-the-humans-02-kit/` (RULES.txt read in full).
Requirements saved as `../requirements.json` (entry_fee null, prerequisites =
linked GitHub only).

## Referral link — FOUND (verified via authenticated API)

- Code: `8467gvgt`
- Link: https://make.fun/r/8467gvgt
- Source: `GET https://make.fun/api/me/referrals` with the agent API key
  (account @jordi-dpras, wallet 5FDn6v1pbyqe6ZChzwyrgeqsVpBjwhXUBVXXMWFazekc).
  No referral URL was invented. The code appears in README.md as bare code,
  as `/r/8467gvgt`, and as `?ref=8467gvgt`.
- Referral program state at fetch: signup reward $0.25 (limit 20), 0 counted
  so far, prize share 10% for 90 days. Rank badge at build time showed
  "2,405 entries · closes Nov 21" — the bounty is crowded; only verified
  signups count, so this entry's realistic shot is a low paid place, not 1st.

## Repo layout (in `repo/`)

- `README.md` (16,922 bytes) — the guide, written from scratch in this
  session: draft written first, then revised in a second message (so
  thinking_revised is satisfied: file written/edited in 2 assistant messages).
  It is NOT a copy of the kit starter — different structure, headings, and
  wording throughout, plus a "Mistakes that cost people entries" section and
  a note that the guide itself is an entry in this bounty. Three badge lines
  are exactly the readme_template lines with owner `JordyPras`, repo
  `bring-the-humans-02`, plus the template footer with `?ref=8467gvgt`.
- `screenshot.png` (1280×6245, 7,993,600 px, 1,184,597 bytes) — **STAND-IN,
  MUST BE REPLACED before submit.** It is a local GitHub-style rendering of
  this README (rendered with python-markdown + chrome-headless-shell,
  script in `../work/render-page.py`, badges fetched live from make.fun).
  It is NOT a capture of the real GitHub repo page, because the repo does
  not exist yet. After the user creates the repo and uploads these files,
  take a real screenshot of the published repo page on GitHub (README
  showing, top = repo name + guide start) and commit it as screenshot.png.
  Caps: PNG ≤ 8 MB, ≤ 16,000,000 px — the stand-in is inside both.
- `LICENSE` — MIT, copyright (c) 2026 JordyPras.
- `.makefun/owner.json` — exactly
  `{"wallet":"5FDn6v1pbyqe6ZChzwyrgeqsVpBjwhXUBVXXMWFazekc"}`.
  (Note: for this bounty the repo owner being the linked GitHub account is
  what makes it yours; owner.json does not substitute for that.)

## Assumed repo name — CHECK

Badge lines and the guide assume the GitHub repo will be named
**`bring-the-humans-02`** under owner **`JordyPras`** (same pattern as the
earlier entries). If the user names the repo differently, update the two
rank/reward badge URLs in README.md (owner/repo segments) and re-render
screenshot.png before submit.

## For the user (GitHub web, after creating the repo)

1. Create public repo `bring-the-humans-02` (created after the competition
   opened 2026-11-18 10:30 UTC — fine).
2. Upload the contents of `repo/` at root (README.md, screenshot.png,
   LICENSE, .makefun/owner.json — create the last via Add file → Create new
   file, since web upload skips dot-directories).
3. Set About (gear): description
   `A newcomer's guide to make.fun: what it is, how to enter your first bounty, and how to get paid in USDC. Built by an AI agent for make.fun's "Bring the humans again" bounty, $1,000 in USDC.`
   (repo_about: "{summary} Built by an AI agent for make.fun's "Bring the
   humans again" bounty, $1,000 in USDC."), homepage
   `https://make.fun/bounty/bring-the-humans-02`, topics
   `makefun, ai-agents, bounties, growth`.
4. Replace screenshot.png with a real capture of the published repo page.
5. Parent then: git fetch the new head, bundle this session's transcripts,
   run `check`, submit before Sat 2026-11-21 17:30 WIB.

## Verification done locally

- README.md: 16,922 bytes (< 2 MB cap); referral code present bare,
  `/r/8467gvgt`, `?ref=8467gvgt`; 3 badge lines match readme_template;
  no `.github/README.md` in repo.
- screenshot.png (stand-in): PNG, 1,184,597 bytes (< 8 MB),
  7,993,600 px (< 16,000,000); top shows repo name + README start; text
  legible (visually checked).
- owner.json: exact expected content, 57 bytes.
- LICENSE: MIT, present at root.

## Not done (parent / user)

- No GitHub repo created, nothing pushed, nothing submitted — by design.
- No bundle/check/submit run yet (parent handles after the repo exists and
  the real screenshot is in place).
