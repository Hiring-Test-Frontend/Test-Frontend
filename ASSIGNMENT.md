# VeriFi AI — 10–15 minute exercise

Add search and a category filter to an existing transactions list.

## Setup

```bash
npm install
npm run dev
```

http://localhost:5173 — `demo@verifi.test` / `demo1234`

Open **Activity**. The list already loads. Work in `src/pages/Transactions.tsx`.

## Task (10–15 min)

1. **Search** — filter rows by merchant or name as the user types.
2. **Category** — let them filter by category (chips or a select). Categories are on each transaction; you can also call `GET /transactions/categories`.
3. **Empty state** — when filters match nothing, say so. Don’t show a blank page.

Client-side filtering is fine. Match the existing UI (`Input`, `Card`, `DataState`).

Amounts: **negative = out**, **positive = in**.

## If you finish early

- Debounce search
- Combine search + category
- A “Clear filters” control
- Keyboard-friendly labels

## Submit

Work on your own branch. Do not commit to `main`.

```bash
git checkout -b your-name
git add src/pages/Transactions.tsx
git commit -m "Add transaction search and category filter"
git push -u origin HEAD
```

Use your real name (or GitHub username) as the branch name, for example `jane-doe`. Push that branch to `origin` and send the branch name when you are done. Leave `main` unchanged.

## Do not

- Rewrite the app or `src/mocks/`
- Add a new page
- Push commits to `main`
