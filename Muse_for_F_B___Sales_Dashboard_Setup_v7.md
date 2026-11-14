# Muse for F&B — Sales Dashboard Setup

**For food & beverage owners. Set up your own sales dashboard with Muse in one chat.**

No copy-paste. No long forms. Just tap, answer one short question at a time, and tap Approve.

> **What you get:** a live Sales Dashboard you can check in 30 seconds every day — today's sales, best seller, growth, and what's pending. Nothing else.

**Version 7 — Tap-to-approve edition, with replica PRD**

> **What this is — and is not:** This is **not** a pre-made dashboard for sale. This is an **interview prompt** — a setup guide for Muse — **plus a replica PRD and an implementation prompt** (Parts 2 and 3 below). Attach this file, Muse interviews you one question at a time, and builds *your* sales dashboard for *your* shop. You are buying the prompt (.md file), not a finished dashboard file.
>
> **Why the PRD is in here:** a prompt alone rebuilds a dashboard at about 90% — the rebuild drops features and fills gaps with its own preferences. The PRD pins down the features, layout order, exact numbers, and style, so a rebuild (by you, or by a friend you share it with) comes out one-to-one. See Part 2 for the spec and the verification protocol.

> **See a sample first:** https://acne-sample-musedashboard.pages.dev/ — Acme Cafe, Singapore, Demo — Synthetic. Sales-only, with KPI cards, a variance table, a sales bridge, payment split, and a reconciliation line. Your real dashboard starts empty, with Pending where you have no data yet.

---

## How it works now

1. Open a new chat with Muse.
2. Tap **Start setup**.
3. Muse asks **one question at a time**, with tap buttons where you can choose.
4. After each short section, Muse shows you what it has — you tap **Approve** or **Change one thing**.
5. Muse builds your dashboard. Done.

**Time:** about 15–20 minutes for the first setup, then 2 minutes a day.

**You will need:** your business name, your website link, and the name of the system you use for sales (your POS / till). Everything else can be added later, or skipped.

No passwords in chat. Ever.

---

## Security — logins to the Vault

Security first. This is a hard rule.

- **Muse never asks for a password in a question.** No password, no username, no login code, no one-time code — in chat, in a question, or in a button label.
- **The owner never types a password in chat.** If a system needs a login, Muse says, in one short message:
  > To connect [system name], add its login to your Muse Secure Vault.
  >
  > [ Add login to Vault ]  [ Skip — Pending ]
- Muse then waits for the owner to add the login in the Vault. Muse uses the Vault login to pull the data. Muse never shows, repeats, or stores the password, and never writes it into the dashboard, the file, or any note.
- **What Muse asks for in chat:** only the system name and its link / login URL — never the login itself. Example: "What's the Odoo login URL?" — paste the link, or Skip. The login itself goes in the Vault only.
- **Systems this applies to:** POS / till (Odoo POS, Square, Lightspeed, Shopify POS, iMin, etc.), accounting (Xero, QuickBooks, Odoo Accounting), Google Analytics, Google Business Profile, and any cloud accounting system.
- **Files instead of logins:** if the owner has a PDF, Excel, or CSV sales export, they can attach that file in chat instead — Muse pulls the data from the file, no login needed.
- If the owner taps Skip, Muse marks that system **Pending** and moves on. No login, no data pull, no guessing.

## Rules Muse follows — read this first

These are hard rules for the Muse agent running the setup. They are what make it user-friendly.

1. **One question per message. Never a list of 9 questions.**
2. **Tap, don't type, wherever possible.** Every choice is a button.
3. **Always offer Skip / Pending.** If the owner doesn't know, tap Skip — Muse marks it **Pending** and moves on. No guessing.
4. **After each section, ask for approval with buttons.** Show a 3–4 line summary, then:
   - [ Approve & continue ]
   - [ Change one thing ]
5. **Don't nag.** While the owner is answering, send **no follow-up messages**.
   Only if there is **no reply for 3 minutes**, send **one** short nudge:
   > Still there? Tap Resume when you're ready.
   Then wait again. No second nudge.
6. **Short, plain words.** Short labels, short sentences. No explainers, no tools section, no long footer on the dashboard.
7. **Sales, inventory, cost and expenses — no full P&L.** This dashboard now covers sales, inventory level, cost of sales, and expenses. No full P&L, balance sheet, or tax filing on this page.
8. **Follow the owner's existing Muse account preferences.** Before asking anything new, use what the owner already has set in their Muse account — language, currency, timezone, date format, and any dashboard style they already use. Use those as the defaults. Do not ask again for something that is already set, unless it is missing or the owner wants to change it. If the owner has a preferred style, colour, or layout, use that. Otherwise, keep the simple default and mark anything unknown as Pending.
9. **Security first — logins go to the Vault, never in chat.** Muse never asks for a password, username, or login code in a question, and the owner must never type one in chat. When a system needs a login, Muse asks the owner to add it to their Muse Secure Vault, with a button. See "Security — logins to the Vault" below.

---

## 1. Start — tap, don't paste

Muse opens with this, and nothing else:

> Let's set up your Sales Dashboard — a simple sales dashboard.
>
> I'll ask one question at a time. Tap to answer where you can, skip anything you don't know.
>
> [ Start setup ]  [ Use Acme example ]

- **Start setup** → go to Step 2.
- **Use Acme example** → fill the demo from Section 5, then go to Step 6 to approve.

No setup prompt to copy. No pasting.

---

## 2. The interview — one question at a time

Muse asks in this order. One message, one question, buttons where shown.

### Step 1 — Shop name

> What's your shop name, as customers see it?
>
> Type it, or tap Skip.
>
> [ Skip — Pending ]

### Step 2 — F&B type

> What kind of F&B are you?
>
> [ Restaurant ]  [ Cafe ]  [ Hawker / food court ]
> [ Bakery ]  [ Bar / drinks ]  [ Cloud kitchen ]
> [ Takeaway / kiosk ]  [ Catering ]  [ Other ]

Tap one. Tap more than one if you do both — Muse will ask "Anything else?" once, then move on.

Then Muse asks, in one short message each:
- Cuisine / what you sell? — type, or Skip
- How many outlets? — [ 1 ] [ 2 ] [ 3+ ] [ Skip ]
- Opening hours? — in 3 short steps, below. Not one typed line.

#### Opening hours — 3 steps

One question at a time, each with a Skip button:

1. Which days are you open?
   > [ Mon–Sun ]  [ Mon–Sat ]  [ Tue–Sun ]  [ Weekdays only ]  [ Custom days ]  [ Skip — Pending ]
   
   Muse records the closed days from this answer. If the owner taps Custom days, Muse asks which days, one short message, then moves on.

2. What time do you open and close?
   > Type it, e.g. 11am–9pm, or tap Skip.
   >
   > [ Skip — Pending ]

3. Any break in the middle, when you're closed?
   > [ No break ]  [ Yes — 2–6pm ]  [ Other break ]  [ Skip — Pending ]
   
   If the owner taps Other break, Muse asks what time the break is, one short message, then moves on.

*Example: Acme Cafe — Mon–Sun, 11am–9pm, break 2–6pm.*

### Step 3 — Business details

One at a time, each with a Skip button:

- Legal / registered name, if different?
- Registration number — UEN / Company No.?
- Country?
- Address?
- Phone?
- Business email?
- Year end? — [ 31 Dec ] [ 31 Mar ] [ 30 Jun ] [ Other ] [ Skip ]
- Currency and timezone? — Muse suggests from Country, owner taps Approve or types another.

**After Step 3, Muse shows a summary and asks:**

> Here's what I have so far:
> [shop name] — [type], [country]
> UEN: [number / Pending]
> Year end: [date / Pending]
> Hours: [days, times, break / Pending]
>
> [ Approve & continue ]  [ Change one thing ]

### Step 4 — Tax — tap ONE

> Which tax applies to you? Tap one.
>
> [ Not registered — 0% ]
> [ GST registered ]
> [ VAT registered ]
> [ Sales tax ]
> [ Not sure — Pending ]

Muse then asks only what that choice needs, one at a time:

- **Not registered — 0%:** Done. No tax on sales. Dashboard shows net sales = total sales.
  *Example: Acme Cafe — not registered, 0%.*
- **GST registered:** Rate? [ 9% ] [ Other ] — GST number? — Prices [ GST-inclusive ] [ GST-exclusive ]
- **VAT registered:** Rate? [ 20% ] [ 5% ] [ 0% ] [ Other ] — VAT number? — Prices [ VAT-inclusive ] [ VAT-exclusive ]
- **Sales tax:** If Country = USA, go to the USA state flow below. For other countries: State / province? — Rate? — Prices [ Tax-inclusive ] [ Tax-exclusive ]
- **Not sure — Pending:** Done. Muse writes "Pending — check with accountant" and moves on.

Muse never adds or removes tax without the owner tapping it.

#### USA state flow — only if Country = USA

One question at a time, each with a Skip button:

1. Which state?
   > Tap one — 50 states + DC, with Skip.
   >
   > [ Skip — Pending ]

2. Muse suggests the state base rate, then asks for ZIP / city — that sets the combined state + local rate.
   > Type the ZIP / city, or tap Skip.
   >
   > [ Skip — Pending ]

3. Prices: tax-inclusive or tax-exclusive?
   > [ Tax-inclusive ]  [ Tax-exclusive ]  [ Skip — Pending ]
   >
   > US is normally tax-exclusive, added at checkout.

4. Do you sell alcohol, and do you do delivery / takeout?
   > Tap what applies, or Skip. Those are taxed differently in many states.
   >
   > [ Alcohol ]  [ Delivery ]  [ Takeout ]  [ None of these ]  [ Skip — Pending ]

Dashboard shows: State rate + Local rate = Combined rate, and net sales vs tax collected separately. Never just one flat %.

#### USA tips — note, not in the interview flow

- State rate is not the total. There are over 13,000 US sales tax jurisdictions. The combined state + local rate averages 7.53% in 2026, ranging from 0% to over 10%.
- 5 states have no state sales tax — Delaware, Montana, New Hampshire, Oregon, Alaska — but that does not mean no tax on a meal. New Hampshire charges 8.5% Meals and Rooms Tax on restaurant food. Alaska lets cities charge up to 7.5%. Oregon has some city prepared-food taxes. Montana has resort taxes.
- Prepared food is taxed almost everywhere, even where groceries are exempt or reduced. Don't use the grocery rate for a restaurant.
- 6 states charge more on meals than on general goods — Connecticut 7.35%, Maine 8%, Vermont 9%, Rhode Island 8%, New Hampshire 8.5%, DC 10%.
- Voluntary tips are not subject to sales tax. Mandatory service charges / auto-gratuity generally are, as part of the sale price. The POS must separate them.
- Delivery fees / packaging bundled with a taxable order are often taxable.
- Do NOT hardcode rates in the file. Muse looks up the combined rate by street address / ZIP on the state's revenue department site, or via TaxJar / Avalara, and marks it Pending until verified. Rates change.

### Step 5 — Website & systems

> What's your website / shopfront link?
>
> Paste the link, or tap Skip.
>
> [ Skip — Pending ]

Then:

> What system do you use for sales / till?
>
> [ Odoo POS ]  [ Square ]  [ Lightspeed ]
> [ Shopify POS ]  [ iMin ]  [ Cash register only ]  [ Other ]

> What's the system link / login URL?
>
> Paste it, or tap Skip.
>
> [ Skip — Pending ]

Then, accounting connect:

> Want to connect an accounting system?
>
> [ Xero ]  [ QuickBooks ]  [ Odoo Accounting ]  [ No — not now ]  [ Skip — Pending ]

If the owner taps one, Muse asks once for its link / login URL, or Skip. Then Muse asks them to add that system's login to their Muse Secure Vault — see "Security — logins to the Vault". Never ask for a password in chat.

> What's the accounting link / login URL?
>
> Paste it, or tap Skip.
>
> [ Skip — Pending ]

Then, Google Analytics & reviews — one question at a time, each with a Skip button:

> Do you have Google Analytics?
>
> Type your GA4 ID, or tap Skip.
>
> [ Skip — Pending ]

> Do you have a Google Business Profile?
>
> Paste your review link, or tap Skip.
>
> [ Skip — Pending ]

Never ask for a password in chat. Logins go to the Secure Vault only — see "Security — logins to the Vault". Never invent a GA4 ID or review link.

Optional, only if the owner wants it — Muse asks once:
> Anything else to link? Drive folder, delivery apps?
>
> [ No, that's all ]  [ Add one ]

### Step 5b — Inventory, cost of sales, and expenses

One question at a time, each with a Skip button. All three are optional — Skip means Pending, and the dashboard shows Pending until the owner adds it.

**Inventory level:**
> Do you track stock / inventory?
>
> [ Yes ]  [ No — not now ]  [ Skip — Pending ]

If Yes, Muse asks, one at a time:
- What are your main stock items? — type a few, or Skip
- Current level for each? — type a number, or Skip
- Low-stock / par level for each? — type a number, or Skip
- Unit cost for each? — type a number, or Skip

Muse flags any item at or below its par level as **Low stock**.

**Cost of sales:**
> Do you want food / product cost per dish?
>
> [ Yes ]  [ No — not now ]  [ Skip — Pending ]

If Yes, Muse asks, one at a time:
- Cost per serving for your best seller? — type, or Skip
- Cost per serving for your other top dishes? — type a few, or Skip

Muse calculates: Cost of sales = cost per serving × servings sold. Gross profit = Sales − Cost of sales. Food cost % = Cost of sales ÷ Sales.

**Expenses:**
> Do you want to track monthly expenses?
>
> [ Yes ]  [ No — not now ]  [ Skip — Pending ]

If Yes, Muse asks, one at a time, for each category the owner names:
- Rent? — amount per month, or Skip
- Utilities? — amount per month, or Skip
- Staff? — amount per month, or Skip
- Delivery / packaging? — amount per month, or Skip
- Other? — name + amount per month, or Skip

Muse never guesses a cost, a stock level, or an expense. Anything unknown is Pending.

### Step 6 — Approve & build

Muse shows the final summary:

> Ready to build?
> [shop] — [type]
> Tax: [choice]
> Website: [link / Pending]
> System: [POS / Pending]
> Accounting: [Xero / QuickBooks / Odoo Accounting / No — not now / Pending]
> Payment types: PayNow / e-wallet, card, cash — bar chart, day / month / year
> Google Analytics: [GA4 ID / Pending]
> Google reviews: [review link / Pending]
>
> [ Approve & build dashboard ]  [ Change one thing ]

Owner taps Approve. Muse builds it. No retyping.

---

## 3. Your Dashboard — what Muse will build

A simple sales dashboard. Short, not wordy.

### Name

**[Your Shop Name] Sales Dashboard**
Heading: **[Your Shop Name] — Sales**

### Links — side by side at the top

| Shopfront | System |
|---|---|
| yourwebsite.com | Your POS link — labelled **Odoo** / **Square** / etc. |

### Headline numbers — 3 only

1. **Best seller**
2. **Revenue growth** — vs last week / last month
3. **Sales today / this month** — one clear number

No Profit, P&L, expenses, or costing on this page. Sales only.

### Charts — let them do the talking

- **Daily sales** — line chart
- **Sales by category / dish** — bar chart
- **Sales timing** — best day / best time, when you have enough days
- **Daily takings by payment type** — PayNow / e-wallet, credit card, cash — bar chart, with day / month / year filters

No long explanations under the charts.

### Website & reviews — monthly

Below the sales charts. Separate from the sales headline numbers — the headlines stay sales-only.

- **Google Analytics — this month vs last month:** Users, Sessions, Page views — each with + / - % vs last month. Pending until GA4 is connected.
- **Google reviews — this month vs last month:** Reviews received this month, total reviews, average rating — each with + / - vs last month, plus the latest 3 reviews, short. Pending until Google Business Profile is connected. Muse drafts replies, owner posts, no auto-posting, no fake / incentivised reviews.

### Inventory level

- **Stock balance:** current level per main item, with par / low-stock level beside it. Items at or below par are flagged **Low stock**.
- **Stock order timeline:** Pending until the owner adds counts and orders.

### Cost of sales

- **Cost of sales — this month:** total, with food cost % vs sales.
- **Per dish:** cost per serving, margin per serving, for the best seller and other top dishes the owner gave costs for.
- **Gross profit:** Sales − Cost of sales, with gross profit %.

### Expenses — monthly

- **Total expenses — this month:** total, with % vs sales.
- **By category:** Rent, Utilities, Staff, Delivery / packaging, Other — each with its monthly amount.
- **Net after cost + expenses:** Gross profit − Total expenses, one line only. No full P&L.

### 3 key drivers — short comments only

Muse adds **one short line each** on the 3 things driving sales right now, e.g.:

- Best seller is driving repeat orders
- Weekend lunch is your peak
- Delivery is growing faster than dine-in

If there isn't enough data yet, it says **Pending**.

### Stock — Pending until you have counts

- **Stock balance:** Pending
- **Stock order timeline:** Pending

Muse does not invent stock numbers.

### Reminders — at the bottom

Short list only, e.g.:

- Till needs re-pointing to new system link
- Rent / utilities amounts — Pending
- Next stock count — Pending

No tools section. No long footer. No routine text.

### Words Muse will use

- **Pending** — not "Not yet", not "TBC"
- Short labels, short sentences
- Numbers with currency, e.g. **S$273.30 (Demo — Synthetic)**
- If a number is a demo / test, Muse says so — demo totals are never shown as real money

---

## 4. Daily routine — 2 minutes

**Daily, after close:**
1. Tell Muse: "Today's sales are in [your system]. Update the dashboard."
2. Muse pulls the day's sales and updates the charts.
3. You check the 3 headline numbers. Done.

**Weekly:** Muse updates revenue growth and best seller.
**Monthly:** Check year-end / tax items with your accountant. Muse keeps the dashboard; your accountant keeps the books.

---

## 5. Example — filled in (Acme Cafe, Singapore — Demo / Synthetic)

This is a demo example, so you can see what "done" looks like. Tap **Use Acme example** to run the demo with it.

All sales figures below are **Demo / Synthetic** — not real money, not real sales.

- **Shop:** Acme Cafe, Singapore
- **Type:** Restaurant, 1 outlet
- **Cuisine:** Pending
- **Hours:** Mon–Sun, 11am–9pm, break 2–6pm
- **Tax:** Not registered — 0%
- **Website:** Courseoss.com
- **System:** Odoo POS, link Pending
- **Accounting:** No — not now
- **Year end:** 31 Dec
- **Currency / timezone:** SGD, Asia/Singapore
- **UEN / registration number:** Pending
- **Address:** Pending
- **Phone:** Pending
- **Business email:** Pending
- **Demo sales today:** **S$273.30 (Demo — Synthetic)**
- **Demo sales this month:** **S$2,847.90 (Demo — Synthetic)**
- **Demo best seller:** Grilled Chicken Chop **(Demo — Synthetic)**
- **Demo dataset:** 13,781 synthetic sales, 1 Jan 2025 to 9 Nov 2026 **(Demo — Synthetic)**
- **Demo payments:** PayNow / card / cash mix, weekend peaks **(Demo — Synthetic)**
- **Demo Google Analytics — this month vs last month (Demo — Synthetic):** Users 1,240 (+18% vs last month), Sessions 1,860 (+15% vs last month), Page views 4,320 (+12% vs last month)
- **Demo Google reviews — this month vs last month (Demo — Synthetic):** Reviews received this month 14 (+6 vs last month), total reviews 128, average rating 4.6 stars (+0.1 vs last month)
- **Google Analytics:** Pending — demo figures above are synthetic only
- **Google Business Profile / review link:** Pending — demo figures above are synthetic only
- **Dashboard:** Acme Cafe Sales Dashboard — Best seller + Revenue growth, stock Pending
- **Demo inventory (Demo — Synthetic):** Grilled Chicken Chop 42 units (par 20), Chicken Rice — rice 120 kg (par 50 kg), Kopi beans 18 kg (par 10 kg) — no Low stock flags
- **Demo cost of sales — Oct 2026 (Demo — Synthetic):** Cost of sales S$2,950, food cost 35.0% of sales, Gross profit S$5,470 (65.0%). Best seller cost: Grilled Chicken Chop S$4.20 per serving, margin S$8.80 per serving
- **Demo expenses — Oct 2026 (Demo — Synthetic):** Rent S$2,200, Utilities S$380, Staff S$1,600, Delivery / packaging S$260, Other S$150 — Total S$4,590 (54.5% of sales). Net after cost + expenses S$880

Demo data is clearly labelled on the dashboard, and can be cleared before real sales are recorded. Demo and real sales are never mixed. The same applies to the demo Google Analytics and Google reviews figures above — clear them before real GA / review data is connected.

---

## 6. Checklist — before you call it done

- [ ] Started by tapping, no copy-paste
- [ ] One question at a time, with Skip offered
- [ ] Opening hours asked as days, times, and break — closed days recorded
- [ ] Tax option tapped, not typed from a list
- [ ] If USA, state asked, then ZIP / city for the combined rate — never one flat %
- [ ] Website + system links added, or Pending
- [ ] Accounting connect asked — Xero / QuickBooks / Odoo Accounting, or No — not now
- [ ] Dashboard shows your shop name, not "Demo"
- [ ] Shopfront and system links sit side by side, labelled
- [ ] 3 headline numbers only — no P&L / expenses on the page
- [ ] Charts are line/bar, no long explainers
- [ ] Daily takings by payment type — PayNow / e-wallet, card, cash — bar chart, day / month / year filters
- [ ] Google Analytics asked — GA4 ID added, or Pending
- [ ] Google Business Profile asked — review link added, or Pending
- [ ] Monthly Google Analytics / Google reviews section shows Pending until connected, or Demo — Synthetic in the demo
- [ ] Inventory asked — stock items, levels, par levels added, or Pending
- [ ] Cost of sales asked — cost per serving added, or Pending; gross profit shows only if costs are given
- [ ] Expenses asked — monthly categories added, or Pending
- [ ] No password was asked for or typed in chat — logins went to the Secure Vault only, or were Skipped as Pending
- [ ] Unknown items say **Pending**
- [ ] Reminders are at the bottom
- [ ] You can read it in 30 seconds
- [ ] No follow-up messages were sent while you were answering, except one nudge after 3 minutes of silence

---

## 7. Rules Muse follows for you

- Never guess a number, a tax rate, a price, or a login.
- Never hardcode a US tax rate — look it up by address / ZIP, mark it Pending until verified.
- Never ask 9 questions in one message.
- Never send a follow-up while the owner is answering — one nudge only, after 3 minutes of no reply.
- Never add a dish, a tax, or a system you didn't name or tap.
- Demo / test orders are never counted as real sales.
- Your passwords stay out of chat — logins go to your Muse Secure Vault only, never typed in chat. Security first.
- If something is wrong, say so in one line and fix it. Don't rebuild the whole dashboard.

---

*Built for F&B owners who want to see their sales clearly — and get back to the shop.*
*Version 7 — Tap-to-approve edition, with replica PRD. No copy-paste.*

---

# Part 2 — Replica PRD (source of truth)


**Replica PRD — first included in Version 7, 14 Nov 2026. This is Part 2 of this file.**

## Why this PRD exists

A prompt alone does not reproduce a dashboard one-to-one. When a friend's Muse rebuilds from the prompt, it fills gaps with its own preferences and drops features — the rebuild lands at ~90%, not an exact replica. This PRD is the missing layer: the features, the layout order, the exact numbers, and the style, in tables a builder can check off. **The prompt tells Muse what to ask. This PRD tells Muse what "done" looks like.**

## Source-of-truth order

When anything conflicts, follow this order. Do not invent, substitute, or "improve".

1. **This PRD** — features, layout, numbers, style.
2. **The mock HTML** — `acme-sales-sample.html` (live at https://acne-sample-musedashboard.pages.dev/). The visual reference. If the PRD and the mock disagree on a number, the PRD wins; if they disagree on layout, the mock wins and the PRD must be corrected.
3. **Part 1 of this file** — the interview flow (one question at a time, tap buttons, Skip / Pending, Approve after each section).
4. **The live Space** — Acme Cafe Sales Dashboard (Space). A working example, not a spec.

## Product

A simple sales dashboard for an F&B owner, readable in 30 seconds a day. Sales, inventory level, cost of sales, and expenses. **No full P&L, no balance sheet, no tax filing on this page.**

## Layout — exact section order, top to bottom

| # | Section | Content |
|---|---|---|
| 0 | Badge | `Demo — Synthetic • [Shop], [Country] • Not real sales` (demo only; omitted on a real dashboard) |
| 1 | Heading | `[Shop] — Sales` (h1, 34px) + sub-line: `Sample month: [Month Year] • Sales, inventory, cost of sales & expenses • No full P&L` |
| 2 | Links, side by side | Two cards: **Shopfront** (website) and **System** (POS link, labelled e.g. Odoo POS, or "link Pending") |
| 3 | Headline KPIs — 4 cards in one row | Best seller / Revenue growth / Sales today / Sales this month |
| 4 | Daily sales — last 7 days | Line chart (SVG) + one note line with the 7 daily figures |
| 5 | Sales by dish — [month] | Horizontal bars, one per dish, longest bar = 100% |
| 6 | Sales timing | Best day / best time, one line (Pending if not enough days) |
| 7 | Daily takings by payment type — [month] | Bars: PayNow / e-wallet, credit card, cash — with day / month / year filters |
| 8 | Sales bridge — [prev month] to [month] | Waterfall: previous month → movers → this month |
| 9 | Variance — top 5 dishes, [month] vs [prev] | Table; any dish moving more than 10% gets a flag |
| 10 | Inventory level — [month] | Stock balance table: item, current level, par level, Low stock flag |
| 11 | Cost of sales — [month] | Total, food cost %, per-dish cost / margin, gross profit |
| 12 | Expenses — [month] | Total, % of sales, by category, net after cost + expenses (one line) |
| 13 | Website & reviews — monthly | GA (Users, Sessions, Page views, each vs last month) + reviews (received, total, average, latest 3) |
| 14 | 3 key drivers | One short line each |
| 15 | Reminders | Short list at the bottom |
| 16 | Reconciliation | One line: `Total = Dishes = Payments` |

No tools section. No long footer. No routine text. No explainers under the charts.

## Feature table

| # | Feature | Spec | Acme demo value |
|---|---|---|---|
| F1 | Shop name heading | `[Shop] — Sales`, h1 | Acme Cafe — Sales |
| F2 | Shopfront + system links | Two cards side by side, labelled; Pending if no link | Courseoss.com / Odoo POS — link Pending |
| F3 | Best seller KPI | Dish name + sales + % vs last month | Grilled Chicken Chop, S$1,312, +18.2% |
| F4 | Revenue growth KPI | % vs last month | +12.4% vs Sep 2026 |
| F5 | Sales today KPI | One clear number, labelled with the sample day | S$273.30 (31 Oct) |
| F6 | Sales this month KPI | Total + % vs last month + order count | S$8,420, +12.4%, 1,124 orders |
| F7 | Daily sales chart | Line chart, last 7 days, with the 7 figures in a note line | Mon S$240, Tue S$255, Wed S$268, Thu S$281, Fri S$312, Sat S$368, Sun S$342 |
| F8 | Sales by dish bars | Bar per dish, longest = 100% width | Chicken Chop S$1,312; Chicken Rice S$980; Laksa S$760; Kopi/Teh S$640 |
| F9 | Sales timing | Best day / best time | Weekend lunch is the peak |
| F10 | Payment-type bars | PayNow/e-wallet, card, cash; day/month/year filters | PayNow S$3,850 (45.7%), Card S$3,120 (37.1%), Cash S$1,450 (17.2%) |
| F11 | Sales bridge | Sep → movers → Oct, must sum exactly | 7,492 → Chicken Chop +202 → Other dishes +818 → Laksa −92 = 8,420 |
| F12 | Variance table | Top 5 dishes, Oct vs Sep, flag any move over 10% | Flagged dishes carry a red flag pill |
| F13 | Inventory | Item, current level, par level; at/below par = **Low stock** | Chicken Chop 42 units (par 20), rice 120 kg (par 50 kg), kopi beans 18 kg (par 10 kg); no Low stock |
| F14 | Cost of sales | Total, food cost %, per-dish cost + margin, gross profit | Oct: S$2,950, 35.0%, Gross profit S$5,470 (65.0%); Chicken Chop S$4.20/serving, margin S$8.80 |
| F15 | Expenses | Total, % of sales, by category; net = gross profit − expenses, one line | Oct: Rent S$2,200, Utilities S$380, Staff S$1,600, Delivery/packaging S$260, Other S$150; Total S$4,590 (54.5%); Net S$880 |
| F16 | Google Analytics | Users, Sessions, Page views, each with +/− % vs last month; Pending until GA4 connected | Users 1,240 (+18%), Sessions 1,860 (+15%), Page views 4,320 (+12%) |
| F17 | Google reviews | Received this month, total, average, latest 3 reviews; Pending until GBP connected; Muse drafts replies, owner posts, no auto-posting | Received 14 (+6), total 128, average 4.6 (+0.1) |
| F18 | 3 key drivers | One short line each; Pending if not enough data | Best seller driving repeat orders; Weekend lunch is peak; Delivery growing faster than dine-in |
| F19 | Reminders | Short list at the bottom | Till re-pointing, Rent/utilities Pending, Next stock count Pending |
| F20 | Reconciliation | One line, must balance exactly | Total S$8,420 = Dishes S$8,420 = Payments S$8,420 |
| F21 | Opening hours | Days open/closed + open/close times + midday break | Mon–Sun, 11am–9pm, break 2–6pm |
| F22 | Tax | One tapped option; USA = state, then ZIP/city for combined rate; never one flat %; never hardcode rates | Not registered — 0% |
| F23 | Security | No password, username, or login code ever asked in chat; logins go to the Muse Secure Vault only; files (PDF/Excel/CSV) instead of logins where possible | — |
| F24 | Interview behaviour | One question per message; tap buttons; Skip / Pending every time; Approve after each section; no follow-ups while answering, one nudge only after 3 min silence | — |
| F25 | Demo labelling | Every demo figure labelled `Demo — Synthetic`; demo and real sales never mixed; demo cleared before real data | 13,781 synthetic sales, 1 Jan 2025 – 9 Nov 2026 |

## Style tokens (from the mock HTML — do not restyle)

- Page: `background #f4f4f2`, text `#1c1c1e`, font system-ui, max-width 1020px, padding 24px.
- Cards: white `#fff`, border `#e5e5e3`, radius 12px, padding 18px.
- KPI value: 26px bold; KPI label: 13px, muted `#6b7280`.
- Up: green `#0a7d2c`. Down / flag: red `#b3261e`, flag pill background `#fde8e8`.
- Chart blue: `#2563eb`. Bars: dark `#3f3f46`, blue variant `#2563eb`; bar track `#e5e7eb`, height 12px, radius 999px.
- Badge: background `#fff3cd`, border `#d9a400`, radius 999px, 13px.
- Reconciliation line: background `#eef2ff`, radius 8px, 13px.
- Headings: h1 34px, h2 19px, h3 15px. Mobile under 640px: KPIs 2 columns, links stack.

## Data model (Acme demo dataset)

- Shop: Acme Cafe, Singapore. Type: Restaurant, 1 outlet. Cuisine: Pending. Year end: 31 Dec. Currency SGD, timezone Asia/Singapore. Tax: Not registered — 0%. Website: Courseoss.com. System: Odoo POS, link Pending. Accounting: No — not now. UEN, address, phone, business email: Pending.
- Sales: Oct 2026 S$8,420 (Sep S$7,492), 1,124 orders. Best seller Grilled Chicken Chop S$1,312 (+18.2%).
- All figures Demo — Synthetic. Never shown as real money.

## Verification protocol — the one-to-one check

Do this before calling a rebuild "done". This is the step that catches the missing 10%.

1. **Mock run:** build the dashboard in a fresh Space from the PRD + mock HTML only (no extra instructions, no peeking at the original Space).
2. **Section-by-section comparison:** go through the layout table (§ Layout) row by row against the mock. For each row, mark Present / Missing / Different.
3. **Feature check:** go through the feature table (F1–F25) the same way. Any feature marked Missing or Different is a defect, not a preference.
4. **Numbers check:** every figure in the demo dataset must match exactly (sales, bridge, reconciliation). A wrong number is a defect.
5. **Log the diffs:** write a short diff log — feature, expected, got, fixed or not. Rebuild until the log is empty.
6. **A/B with mock examples:** run the same check with the Acme demo data and with a second made-up shop (different name, type, tax) to catch hardcoded values.
7. **Sandbox dry run:** test the interview flow end to end with mock answers, including Skip on every optional question, and confirm Pending appears instead of invented data.

## Version log

| Version | Date | Change |
|---|---|---|
| 1 | 14 Nov 2026 | First PRD, built from v6 prompt + Acme mock HTML + live Space. |

---

# Part 3 — Implementation prompt


**Attach this file and the mock HTML to a new Muse chat, then paste this prompt. Do not paste the prompt on its own.**

1. This file — Parts 1 and 2 are the interview flow and the PRD (the source of truth: features, layout, numbers, style).
2. `acme-sales-sample.html` — the mock. The visual reference for what "done" looks like. Live at https://acne-sample-musedashboard.pages.dev/.

---

Build the sales dashboard exactly as specified in the attached PRD.

Rules for this build:

- Read Part 2 (the PRD) first, in full, before building anything. The PRD outranks Part 1 and outranks your own preferences. If the PRD and the mock HTML disagree on a number, use the PRD number. If they disagree on layout, use the mock layout and note it in your diff log.
- Build every section in the PRD layout table, in the same order, top to bottom. Do not skip a section, merge two sections, or add a section that is not in the PRD.
- Build every feature F1–F25 in the feature table. Do not drop a feature because it looks minor, and do not add a feature because it looks useful.
- Use the PRD style tokens exactly: page background #f4f4f2, white cards with #e5e5e3 borders and 12px radius, KPI value 26px bold, chart blue #2563eb, up green #0a7d2c, down/flag red #b3261e. Do not restyle, rebrand, or "modernise" the look.
- Use the Acme demo dataset from the PRD for the demo build. Every figure must match the PRD exactly, including the sales bridge (7,492 → +202 → +818 → −92 = 8,420) and the reconciliation line (Total S$8,420 = Dishes S$8,420 = Payments S$8,420). Label every demo figure "Demo — Synthetic".
- Never invent a number, a tax rate, a price, or a login. Anything unknown is "Pending", not a guess.
- Never ask for a password, username, or login code in chat. Logins go to the Muse Secure Vault only.
- No full P&L, no balance sheet, no tax filing on this page. Net after cost + expenses is one line only.

When the build is done, run the verification protocol in the PRD before you say it is finished:

1. Compare your build against the mock HTML section by section, using the PRD layout table, and list every row as Present, Missing, or Different.
2. Check every feature F1–F25 the same way.
3. Check every demo number against the PRD.
4. Show me the diff log. Fix every Missing and Different item, then re-check, until the log is empty.
5. Then run the same check with a second made-up shop (different name, type, and tax) to catch anything hardcoded to Acme.

Only tell me the dashboard is done when the diff log is empty. If something in the PRD is unclear, ask me in one short message instead of guessing.
