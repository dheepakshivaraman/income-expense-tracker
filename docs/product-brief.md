# Income & Expense Tracker — Product Brief

## Core value proposition

Most people do not know where they stand financially *right now*. Bank apps show
transactions but bury the answer; spreadsheets demand discipline nobody sustains.

**The promise:** record a single amount against a category in under ten seconds,
and always see one honest number — what you have left.

The product wins on *speed of capture* and *clarity of answer*. Everything that
does not serve those two things is not the product.

## Primary persona

**"Priya, the self-managed earner."**

- Earns from more than one place (salary, freelance work, the occasional refund).
- Spends across a handful of predictable buckets — rent, food, travel, bills.
- Has abandoned at least two budgeting apps because onboarding took longer than
  the problem was worth.
- Wants an answer to one question at the end of each month: *did I come out ahead?*

Priya is not an accountant. She will not categorise into forty buckets, she will
not reconcile, and she will not link a bank account to a product she does not yet
trust. She will type a number if it takes one screen.

## MVP definition

The minimum version that delivers the promise is a **single-user ledger with a
live balance.**

A user must be able to:

1. Record an amount as either income or expense.
2. Attach it to a category.
3. See total income, total expense, and the resulting balance update immediately.
4. Review what has been recorded, and remove a mistake.
5. Add a category when the seeded ones do not fit.

That is the entire launchable product. If a user can do those five things, the
value proposition holds.

### Ruthlessly excluded from the MVP

Each of these is a reasonable feature. None of them is needed to prove the
core promise, and each one delays it.

| Deferred | Why it waits |
| --- | --- |
| Accounts, login, multi-user | The insight is valuable before it is shared. Local single-user first. |
| Bank / UPI sync | Enormous integration cost, and trust we have not yet earned. |
| Budgets and limits | Meaningless until a user has history to budget against. |
| Recurring transactions | A convenience on top of capture, not capture itself. |
| Editing a transaction | Delete-and-re-add covers the same need at a fraction of the cost. |
| Charts and trends | Three totals answer the question. Charts decorate it. |
| CSV import / export | An escape hatch for users we do not have yet. |
| Multi-currency | One currency proves the model. |
| Mobile app | The web form is the fastest thing to ship and to change. |

## Epic roadmap

**Epic 1 — Capture (MVP).** Record income and expense against a category.
*Outcome: the ledger exists and is trustworthy.*

**Epic 2 — Understand (MVP).** Live totals, balance, and a per-category
breakdown. *Outcome: the user gets the answer without doing arithmetic.*

**Epic 3 — Organise (MVP, thin slice).** Seeded categories plus the ability to
add one. *Outcome: the ledger fits the user's actual life.*

**Epic 4 — Retain (post-MVP).** Accounts and sync, so the ledger survives a
device change.

**Epic 5 — Guide (post-MVP).** Budgets, trends, and recurring entries — advice
layered on top of a ledger that already works.

## Prioritized backlog

Ordered by the sequence in which they deliver value. Stories 1–7 constitute the
MVP; the rest are explicitly not being built yet.

### MVP

**US-1 — Record an expense**
As a self-managed earner, I want to record an expense with an amount, category
and date, so that my spending is captured the moment it happens.
*Priority: P0 · Epic 1*

**US-2 — Record an income**
As a self-managed earner, I want to record income the same way I record an
expense, so that the ledger reflects money in as well as money out.
*Priority: P0 · Epic 1*

**US-3 — See my current totals**
As a self-managed earner, I want to see total income, total expense and my
balance, so that I know where I stand without doing any arithmetic.
*Priority: P0 · Epic 2*

**US-4 — Review my transactions**
As a self-managed earner, I want to see the entries I have recorded, most recent
first, so that I can confirm the ledger matches reality.
*Priority: P1 · Epic 1*

**US-5 — Delete a transaction**
As a self-managed earner, I want to remove an entry I recorded by mistake, so
that my balance stays trustworthy.
*Priority: P1 · Epic 1*

**US-6 — Break spending down by category**
As a self-managed earner, I want to see totals grouped by category, so that I
can tell which bucket is consuming my money.
*Priority: P1 · Epic 2*

**US-7 — Add a category**
As a self-managed earner, I want to add a category of my own, so that the
tracker matches how I actually think about my money.
*Priority: P2 · Epic 3*

### Deferred

- **US-8** — Filter the ledger by date range. *Post-MVP · Epic 2*
- **US-9** — Sign in so my data follows me across devices. *Post-MVP · Epic 4*
- **US-10** — Set a monthly budget per category and be warned when I approach it. *Post-MVP · Epic 5*
- **US-11** — Mark a transaction as recurring. *Post-MVP · Epic 5*
- **US-12** — Export my ledger as CSV. *Post-MVP · Epic 5*

## Success criteria for the MVP

- A first-time user records their first transaction in under 30 seconds, with no
  setup beyond opening the app.
- Recording or deleting a transaction updates the displayed balance with no
  manual refresh.
- The three headline numbers are always internally consistent:
  `balance = total income − total expense`.
