# Scraping API free trial: what ScraperAPI's 7 days and 5,000 credits actually cover, what happens on day 8, and which plan you'd need after (full pricing table)

ScraperAPI's free trial runs 7 days and gives you 5,000 API credits, no credit card required. When it ends, the account settles onto a permanent free plan of 1,000 credits per month with 5 concurrent connections.

The part sign-up pages tend to skip is that a credit is not a request. A standard HTML page costs 1 credit, Amazon costs 5, Google and Bing cost 25, LinkedIn costs 30, and a page behind Cloudflare or DataDome costs 11 once the bypass is added. So 5,000 trial credits buy 5,000 ordinary pages, or 1,000 Amazon products, or 200 Google result pages. That ratio decides whether one week is enough to test your target. Below is every plan and price on the pricing page, the full credit table, what happens when the trial runs out, and how the trial terms compare with the two other free trials developers usually shortlist.

> **Quick verdict:** if your target is a plain HTML site, stay on the free plan. It costs nothing and 1,000 credits a month covers a small daily job. If your target is Amazon, a search engine, or anything behind bot protection, spend the 7 days on a concentrated test, because the free tier only buys 200 or 40 requests a month there. 👉 [Start the 7-day trial with 5,000 credits](https://www.scraperapi.com/signup?fp_ref=coupons)

## Every ScraperAPI plan and price

All seven paid tiers carry the same features: JS rendering, premium residential and mobile IPs, advanced bypassing, structured data endpoints, DataPipeline, full crawler access, automatic retries, unlimited bandwidth and a 99.9% uptime guarantee. What changes between tiers is volume, concurrency, geotargeting and how much analytics history you keep. Analytics covers the last 30 days on Hobby and Startup, and is unlimited from Business upward. Annual billing takes 10% off automatically, with no code.

| Plan | Credits per month | Concurrent threads | Geotargeting | Monthly / annual (per month) |  |
| --- | --- | --- | --- | --- | --- |
| Free | 1,000 | 5 | Not included | $0 | [Create a free account](https://www.scraperapi.com/signup?fp_ref=coupons) |
| Hobby | 100,000 | 20 | US & EU | See pricing page | [View Hobby](https://www.scraperapi.com/pricing?fp_ref=coupons) |
| Startup | 1,000,000 | 50 | US & EU | $149 / $134.10 | [View Startup](https://www.scraperapi.com/pricing?fp_ref=coupons) |
| Business | 3,000,000 | 100 | Country-level | $299 / $269.10 | [View Business](https://www.scraperapi.com/pricing?fp_ref=coupons) |
| Scaling (most popular) | 5,000,000 | 200 | Country-level | $475 / $427.50 | [View Scaling](https://www.scraperapi.com/pricing?fp_ref=coupons) |
| Professional | 10,500,000 | 300 | Country-level | $975 / $877.50 | [View Professional](https://www.scraperapi.com/pricing?fp_ref=coupons) |
| Advanced | 21,500,000 | 500 | Country-level | $1,975 / $1,777.50 | [View Advanced](https://www.scraperapi.com/pricing?fp_ref=coupons) |
| Enterprise | 22,000,000+ | 500+ | Country-level | Custom quote | [Ask for Enterprise pricing](https://www.scraperapi.com/pricing?fp_ref=coupons) |

Hobby is the entry paid tier and its current monthly rate is shown on the pricing page alongside the six tiers above. Country-level geotargeting starts at Business, which is also where the analytics window stops being capped at 30 days.

## What 5,000 credits actually buy

ScraperAPI bills per request, and the request price depends on the domain you hit and the parameters you send. The multipliers below are the ones the pricing page publishes.

| Request type | Credits per request |
| --- | --- |
| Standard HTML page | 1 |
| E-commerce (Amazon, Walmart, eBay) | 5 |
| Search engines (Google, Bing, including subdomains) | 25 |
| LinkedIn | 30 |
| Bot-protection bypass (Cloudflare, DataDome, PerimeterX, Akamai) | +10 |
| JS rendering (`render=true`) | +10 |
| Premium proxies (`premium=true`) | +10 |
| Screenshot | +10 |
| Ultra Premium (paid plans only) | 30 |
| Ultra Premium with rendering | 75 |

Geotargeting, sessions, device type, output format and auto-parsing add nothing. Every response reports its own cost in the `sa-credit-cost` header, the dashboard's Domain Cost Estimator prices any URL before you scrape it, and `max_cost` caps a single request so one expensive page can't eat a chunk of your allowance.

Here is the same 5,000 credits expressed as real requests, next to what the free plan covers each month:

| Target | Credits each | 7-day trial (5,000) | Free plan (1,000/month) |
| --- | --- | --- | --- |
| Plain HTML page | 1 | 5,000 | 1,000 |
| Amazon / Walmart / eBay | 5 | 1,000 | 200 |
| Google or Bing | 25 | 200 | 40 |
| LinkedIn | 30 | ~166 | ~33 |
| Cloudflare-protected page | 11 | ~450 | ~90 |

Two things follow. A weekly SERP tracking job across 40 keywords, one pull each, burns the entire free month in a single run. And a 1,000-product Amazon price check fits inside the trial with room to spare, but needs a paid plan for anything recurring. On Startup, a standard page works out to roughly $0.15 per 1,000, which is cheap enough that the multiplier, not the plan, is what decides your bill.

## Day 8: what happens when the trial ends

Nothing is charged. The trial requires no card, and when the 7 days are up the account simply reverts to 1,000 credits a month at 5 threads. If you do upgrade and burn through a month's credits, the default is that scraping pauses until renewal, and unused credits do not roll over.

How you get out of that pause depends entirely on the tier:

- **Hobby, Startup, Business:** auto-upgrade only. When credits run out, the account moves to the next plan if you've opted in; otherwise it stays paused until renewal. There is no overage billing on these three.
- **Scaling, Professional:** auto-upgrade or pay-as-you-go, with a monthly spending cap you set.
- **Advanced, Enterprise:** pay-as-you-go only, and Enterprise limit changes go through sales.

Pay-as-you-go is a spending limit rather than a prepayment, so leaving it on won't produce a surprise invoice beyond the cap you configured. But the cheapest plan that offers it at all is Scaling at $475 a month, which makes $475 the real floor for "keep scraping at a fixed per-credit rate." If you're on Startup at $149 and your volume creeps past a million credits, the next step is $299 Business, not a small overage charge. Size the plan with headroom, or trim rendering to the pages that need it.

Concurrency works differently from credits. Exceed your thread limit and the API returns a 429 asking you to come back within the limit. The request is turned away rather than queued, and you aren't charged for it.

Cancellation is free at any time from the dashboard or through support, and paid plans carry a 7-day no-questions-asked refund. 👉 [Compare the plans and current rates on the pricing page](https://www.scraperapi.com/pricing?fp_ref=coupons)

## How the free trials compare

Three trials come up repeatedly when developers are picking a scraping API, and they're built on different models. ScraperAPI front-loads a large allowance into one week. Import.io spreads a similar allowance across a month. Decodo gives a small recurring free tier instead of a countdown.

|  | ScraperAPI | Decodo | Import.io |
| --- | --- | --- | --- |
| Trial length | 7 days | Ongoing free credit | 30 days |
| Allowance | 5,000 credits, then 1,000/month free | $5 credit, up to 10K requests; free starter plan up to 10K requests/month | 5,000 successful queries |
| Card required | No | No | No, nothing auto-charged |
| Failed requests billed | Charged per request with domain multipliers; no success-only promise published | Only successful responses billed | Blocked, failed, timed-out and empty requests not counted |
| Cheapest paid plan | Hobby (rate on pricing page) | $19/mo at 10 req/s | $9/mo annual or $11 month-to-month for 5,000 queries |

The absence of domain multipliers on Decodo and Import.io is a genuine difference, not a marketing line. On a mixed workload that includes search engines or protected sites, their flat per-request pricing is easier to forecast than a credit system where the same plan covers 25x fewer Google pages than HTML pages.

Each model fits a different validation job. Import.io's 30 days suit a slow check against a scheduled workflow, since one page of data equals one query and a paginated category of 12 pages counts as 12. Decodo's recurring free tier suits a small long-running job you want to keep alive indefinitely. ScraperAPI's single week suits hammering one real target hard enough to see whether it gets blocked, which is the question a trial is actually there to answer.

## Who shouldn't pick ScraperAPI

**You need country-level geotargeting on a small budget.** Hobby and Startup are pinned to US and EU proxies. Any other country means Business at $299 a month, which is a steep entry price if geo is the only reason you're upgrading.

**You want pay-as-you-go but can't commit $475.** Overage billing starts at Scaling. Below that, a busy month forces a plan jump instead of a metered top-up.

**Your targets are social platforms or heavily protected travel sites.** Independent testing circulated by third parties has reported very low success rates on several of these, and LinkedIn, which does work, costs 30 credits per request. Test your exact domain during the trial rather than assuming the bypass handles it.

**Your target sits behind a login.** Session support keeps cookies alive, but third-party write-ups of ScraperAPI's documentation state that scraping content behind authentication walls violates its terms. Confirm before you build a workflow around it.

**You care about 404s or fresh pricing data.** The same third-party summaries note that 404 responses still consume credits, and that difficult targets can be served from a cache for up to 10 minutes. Neither appears in the pricing FAQ, so verify against current docs if either affects your job.

## Picking a plan without wasting the trial

Match the plan to the target, not to the credit number:

- **One or two plain HTML sources, checked daily:** the free plan, indefinitely. 1,000 credits a month is 1,000 pages, and no card is needed to keep it.
- **Amazon, a search engine, or a protected site you haven't tested yet:** the 7-day trial, and divide 5,000 by the per-request cost before you start so you know whether you can afford 200 requests or 5,000.
- **Production traffic with a plain-HTML workload:** Startup at $149 monthly or $134.10 on annual, unless you need country-level geo (Business, $299) or the ability to overflow (Scaling, $475).
- **Anything above a few million credits a month:** compare Scaling against Professional on a per-credit basis, and check whether Enterprise's volume discount applies to your mix. Ultra Premium requests keep their own minimum rate even under Enterprise pricing.

Three checks before you enter card details. Run your actual target URL through the Domain Cost Estimator, because a plan sized on sticker credits can shrink by 25x on a Google SERP job. Decide whether you need country-level geotargeting now rather than later, since it moves your entry plan from Hobby to Business. And buy to your monthly burn, because credits reset at renewal and anything unused is gone.

👉 [Start the 7-day trial and price your own target before choosing a plan](https://www.scraperapi.com/signup?fp_ref=coupons)
