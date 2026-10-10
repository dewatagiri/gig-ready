# Rancang Rezeki – 3-user self-test

Automated in headless Chromium (390×844 phone viewport), driving the real UI: each user's 12 months of entries are typed
into the Log form, then the displayed numbers are compared to an independently computed expectation (22 checks per user).
Window: Oct 2025 – Sep 2026. Set-aside placeholders: EPF/i-Saraan 10%, tax 5%, buffer 10%. Debt limit 65%.

| | Low | Medium | High |
|---|---|---|---|
| Platforms | Grab (+ foodpanda every 3rd month) | Grab + foodpanda | Grab, Lalamove, Shopee, custom "Other" |
| 12-month average | RM 1,217 | RM 3,167 | RM 8,717 |
| Lean month | RM 900 (Apr 2026) | RM 2,000 (Jan 2026) | RM 7,200 (Mar 2026; Shopee RM 0) |
| Set-aside on average (EPF / tax / buffer) | RM 122 / 61 / 122 | RM 317 / 158 / 317 | RM 872 / 436 / 872 |
| Existing instalments + target | RM 250 + 300 = 550 | RM 800 + 600 = 1,400 | RM 1,500 + 1,500 = 3,000 |
| Debt % of lean month | 61.1% – within 65% | **70% – flagged (above 65%)** | 41.7% – within 65% |
| Debt % of average | 45.2% – within 65% | 44.2% – within 65% | 34.4% – within 65% |
| Checks passed | 22/22 | 22/22 | 22/22 |

The medium user shows why both views matter: fine on average, over the line in the lean month.

Also verified for every user: BM default, EN toggle, footer text, data survives reload, 5-item checklist + "one bank account" tip,
zero network requests, no page errors, no horizontal scroll, HTML in a custom platform name is shown as text (not injected).
Extra: the app still works when `localStorage` throws. Script was run from the session scratchpad (not committed).
