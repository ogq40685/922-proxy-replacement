# 922 proxy review: why it went dark, and how to replace it without burning another prepaid balance

Most people searching for a 922 Proxy review aren't comparison shopping. They're trying to log in. The client won't authenticate, the domain times out, the ticket queue is silent, and the balance sitting in the dashboard suddenly looks like money they'll never see again.

So here's the version of this review that actually helps: what happened to the service, what happens to the money you left in it, and how to pick a replacement you won't be writing another article like this about next year.

## Short answer: 922 Proxy is not working, and it isn't coming back

The service didn't go down for maintenance. It was part of the IPIDEA residential proxy infrastructure that Google's Threat Intelligence Group dismantled, and the company published a detailed report on January 28, 2026.

What that operation involved, per reporting on the takedown [4]:

- Court-ordered seizure of the domains used to control devices and sell the service
- Google Play Protect updated to detect and remove Android apps carrying the IPIDEA SDK
- Technical details shared with platforms, researchers and law enforcement
- Coordination with Cloudflare and internet providers to disrupt the command infrastructure

Google says millions of devices were removed from the pool. Dozens of brands were running on that single backend, and 922 Proxy was on the published list alongside PIA S5 Proxy, Luna Proxy, 360 Proxy, PY Proxy, IP2World, ABC Proxy, Tab Proxy and others [4]. One infrastructure, many storefronts.

Independent checks of the 922 domains found the same thing users did: no response, registration lapsing or expired, and a client that couldn't reach its authentication server. There was never a shutdown notice. The service simply stopped answering [3].

If the pattern feels familiar, it should. 911 S5 was shut down in 2022 and its operator was arrested in 2024, and PIA S5 and 922 Proxy were widely described as its successors [4].

## What 922 Proxy was, while it lasted

For context on why so many people are still searching for it: 922 Proxy (also written 922 S5 Proxy) specialised in SOCKS5 residential and ISP proxies, advertised a pool of 200 million-plus IPs across more than 190 countries, and offered rotating and sticky sessions with city-level targeting. Bandwidth was quoted at roughly 20–50 MB/s per IP [2]. Pricing was aggressive enough that it became a default pick for anti-detect browser setups, scraping pipelines and multi-account work.

The reputation had already started cracking before the shutdown. Reviews aggregated later described high failure rates on IPs that were flagged or blacklisted, inconsistent speeds and latency on residential packages, and support that responded slowly without any real-time option [1]. A proxy that's cheap but unreliable is a specific kind of expensive: you pay twice, once in the invoice and once in the retries.

## The money question nobody wants to answer

Realistically, balances are gone [3]. The console is unreachable, there's no support channel, and no legal entity to pursue. If you paid by card recently, a chargeback request is worth the phone call. If you paid in crypto, treat it as tuition.

The obvious follow-on risk is worse than the loss itself. Dead proxy brands attract impersonators. Anything calling itself a "922 official mirror", "922 v2", or a Telegram bot offering to migrate old balances is targeting orphaned accounts and deposits [3]. Before you type credentials anywhere, check the domain's registration date, and never reuse an old password on a site you haven't verified. A domain registered last month is not a relaunch.

There's a broader lesson in how 922 died, and it applies to whatever you buy next: cheap residential proxies that stay vague about where the IPs come from carry risk beyond reliability. The IPIDEA pool was built by bundling SDKs into free apps and VPN clients so that ordinary people's home connections were rented out without their knowledge [4]. That's the part that drew the takedown, and it's why the whole thing evaporated overnight rather than degrading gradually.

## How to judge the next provider before you pay

Five questions, in order of how much they'll cost you if you get them wrong:

1. **Is the IP sourcing explained?** Not the pool size claim — the sourcing. A provider that can't say where its IPs come from is one subpoena away from disappearing.
2. **What happens to unused balance if the provider dies?** If the answer is "nothing", buy in small amounts.
3. **Is there a validity window on your traffic?** A 180-day expiry on GB packages is normal and fine. A balance that expires in 30 days on a project that runs for six months is not.
4. **Does the billing model match how your workload actually consumes the network?** Per-IP and per-GB price very differently once you're at scale.
5. **Can you test before committing real money?** Refund policies on proxy services are usually narrower than people assume.

That's the frame I'd use on 9Proxy, which is the provider most 922 users are being pointed toward.

## What 9Proxy actually is

9Proxy is a residential proxy platform with a pool of 20 million-plus residential IPs across 90+ countries, HTTP and SOCKS5 support, and targeting down to country, city and state (with ZIP code and ISP-level options advertised as well). The company claims 99.95% uptime and runs 24/7 human support via Telegram, email and tickets [6][7][10].

One point that matters given why you're reading this: 9Proxy does not appear in the list of brands Google tied to the IPIDEA infrastructure [4]. That's an observation about the published list, not a certification — but it's the first thing worth checking after 922, and it checks out.

The platform splits into two genuinely different billing models, plus bundles that mix them [5]:

**IP-based.** You buy a fixed number of residential IPs and get unlimited bandwidth through them. Unused IPs don't expire, so a package bought this month is still sitting there in three months. The trade-off is lifespan: once an IP is in use it typically stays alive for a few hours up to around 24 hours, and there's no natural rotation — you rotate through the Auto Rotation Proxy feature at intervals you set on selected ports. Authentication requires the desktop app for local port forwarding, with optional proxy authentication [5].

**GB-based.** You buy traffic instead of addresses, and generate unlimited endpoints. IPs rotate per request or per session (sticky mode switches when the configured session time ends), and auth is the simple stuff: username/password or IP whitelist, straight from the dashboard with no app required [5]. Validity is 180 days, unlimited on enterprise tiers.

Access routes cover the usual spread: a Windows client, Proxy2Web for zero-install browser use, ProxyHub for mobile device management, a public API for pipelines, and native SOCKS5 for anti-detect browsers and Python scripts [6].

Payments accepted include credit cards, crypto (USDT, BTC, ETH, LTC, DOGE and others), Alipay, Apple Pay and Google Pay [9].

On performance, one independent review measured a 97.7% success rate against Cloudflare-protected targets, and noted the pool stays reasonably clean — a low hard block rate, which is the part that actually determines whether your scraper works or spends its day solving challenges [6].

👉 [See 9Proxy's IP-based, GB-based and bundle packages](https://bit.ly/9-Proxy)

## Full plan and price comparison

One thing to know before you read the table: 9Proxy ran its first pricing adjustment effective June 1, 2026, which changed IP-based and bundle pricing. GB-based pricing was left untouched and remains as it was [5][6]. That's why older reviews and coupon pages show different IP-tier numbers — they're pre-adjustment.

| Plan | Billing model | What you get | Price (USD) | Validity | Purchase |
| --- | --- | --- | --- | --- | --- |
| 100 IPs | IP-based, unlimited bandwidth | 100 residential IPs | $24 | IPs don't expire until used | [Get 100 IPs](https://bit.ly/9-Proxy) |
| 500 IPs | IP-based, unlimited bandwidth | 500 residential IPs | $72 | IPs don't expire until used | [Get 500 IPs](https://bit.ly/9-Proxy) |
| 1,000 IPs + 500 bonus | IP-based, unlimited bandwidth | 1,500 usable IPs | $126 | IPs don't expire until used | [Get the 1,000 IP package](https://bit.ly/9-Proxy) |
| 2,500 IPs | IP-based, unlimited bandwidth | 2,500 residential IPs | $210 | IPs don't expire until used | [Get 2,500 IPs](https://bit.ly/9-Proxy) |
| 5,000 IPs | IP-based, unlimited bandwidth | 5,000 residential IPs | $360 | IPs don't expire until used | [Get 5,000 IPs](https://bit.ly/9-Proxy) |
| 15,000 IPs | IP-based, unlimited bandwidth | 15,000 residential IPs | $720 | IPs don't expire until used | [Get 15,000 IPs](https://bit.ly/9-Proxy) |
| 25,000 IPs | IP-based, unlimited bandwidth | 25,000 residential IPs | $863 | IPs don't expire until used | [Get 25,000 IPs](https://bit.ly/9-Proxy) |
| 50,000 IPs | IP-based, unlimited bandwidth | 50,000 residential IPs | $1,438 | IPs don't expire until used | [Get 50,000 IPs](https://bit.ly/9-Proxy) |
| Business 100,000 IPs | IP-based, high volume | 100,000 residential IPs | $2,300 | IPs don't expire until used | [Get the 100,000 IP business package](https://bit.ly/9-Proxy) |
| Business 200,000 IPs | IP-based, high volume | 200,000 residential IPs | $4,140 | IPs don't expire until used | [Get the 200,000 IP business package](https://bit.ly/9-Proxy) |
| Business 500,000 IPs | IP-based, high volume | 500,000 residential IPs | $8,625 | IPs don't expire until used | [Get the 500,000 IP business package](https://bit.ly/9-Proxy) |
| 5 GB | GB-based | 5 GB of residential traffic | $15 | 180 days | [Get 5 GB](https://bit.ly/9-Proxy) |
| 50 GB + 5 GB bonus | GB-based | 55 GB of residential traffic | $105 | 180 days | [Get the 50 GB package](https://bit.ly/9-Proxy) |
| 100 GB | GB-based | 100 GB of residential traffic | $150 | 180 days | [Get 100 GB](https://bit.ly/9-Proxy) |
| 200 GB | GB-based | 200 GB of residential traffic | $200 | 180 days | [Get 200 GB](https://bit.ly/9-Proxy) |
| 1,000 GB | GB-based | 1,000 GB of residential traffic | $800 | 180 days | [Get 1,000 GB](https://bit.ly/9-Proxy) |
| 2,000 GB | GB-based | 2,000 GB of residential traffic | $1,500 | 180 days | [Get 2,000 GB](https://bit.ly/9-Proxy) |
| Enterprise 3,000 GB | GB-based, enterprise | 3,000 GB of residential traffic | $2,160 | No expiry | [Get the 3,000 GB enterprise package](https://bit.ly/9-Proxy) |
| Enterprise 6,000 GB | GB-based, enterprise | 6,000 GB of residential traffic | $4,200 | No expiry | [Get the 6,000 GB enterprise package](https://bit.ly/9-Proxy) |
| Enterprise 10,000 GB | GB-based, enterprise | 10,000 GB of residential traffic | $6,800 | No expiry | [Get the 10,000 GB enterprise package](https://bit.ly/9-Proxy) |
| Bundle: 100 IPs + 5 GB | Mixed | 100 IPs plus 5 GB traffic | $30 | IPs don't expire; GB 180 days | [Get the starter bundle](https://bit.ly/9-Proxy) |
| Bundle: 1,500 IPs + 50 GB | Mixed | 1,500 IPs plus 50 GB traffic | $180 | IPs don't expire; GB 180 days | [Get the popular bundle](https://bit.ly/9-Proxy) |
| Bundle: 5,000 IPs + 500 GB | Mixed | 5,000 IPs plus 500 GB traffic | $720 | IPs don't expire; GB 180 days | [Get the pro bundle](https://bit.ly/9-Proxy) |

Prices above reflect the post-June-1-2026 structure for IP-based and bundle plans, and unchanged GB-based rates [5][6]. Confirm the total in your dashboard before paying — packages and bonuses do get revised.

## Which package actually fits your job

The two models aren't a ladder from cheap to expensive. They're built for different workloads, and picking wrong is the most common way people waste money here.

**If your sessions need to persist** — account logins, carts, anything where the same address has to stay put — you want IP-based. Bandwidth is unlimited, so a heavy 4K-ish asset pipeline through 500 IPs costs the same as a text-only one. The 1,000 IP package with the 500 bonus IPs is the best value on the board: $126 for 1,500 usable addresses works out to about $0.084 per IP, versus $0.24 per IP at the 100-IP entry tier. Start at 100 IPs only if you're testing the platform; if you already know your workflow, skipping to the 1,000+500 tier is a straight 65% cut in unit cost.

**If you rotate constantly and each request is small** — SERP checks, ad verification, geo-checking, API polling — GB-based wins, because you're paying for a few hundred kilobytes per request rather than reserving addresses you won't reuse. The 200 GB tier is where GB pricing stops being expensive: $1.00 per GB versus $3.00 per GB on the 5 GB entry pack. The 10,000 GB enterprise tier at $0.68 per GB is only worth it if you're running continuous infrastructure, but that one has no expiry at all, which the 180-day tiers don't.

**If you're not sure yet**, the $30 bundle is the honest recommendation. It gets you 100 IPs and 5 GB in one account, enough to test both behaviour patterns against your actual targets before you commit to a four-figure package.

One caveat on the 180-day window: it applies to the 5, 50, 100, 200, 1,000 and 2,000 GB packages. If your project runs slower than that, you're buying traffic you may not consume in time. Enterprise GB tiers remove the deadline entirely.

## Discounts: what exists and what's expired

This is where most proxy "review" pages quietly lie to you, so here's the current state.

9Proxy ran a GB promotion in April 2026: after your first paid GB order of the month, a personal 9% coupon appeared in your dashboard under My Coupons, single-use, GB orders only, not stackable, and it expired June 30, 2026 [8]. That window has closed. Lunar New Year codes like LNY2026 offered 8% off regular IP and GB packages between January 23 and February 23, 2026, and those are dead too [9]. Coupon-aggregator pages still list both. That doesn't make them usable at checkout.

What's live is the invite mechanism itself. 9Proxy's affiliate program terms describe commissions up to 15% and a 5% discount for users who arrive through a referral invite [9]. The link in this article carries an invite code, so if that term is honoured at checkout you'll see the discount in the order summary — check it before you confirm payment rather than assuming, and don't expect it to stack with anything else.

👉 [Set up a 9Proxy account and check what the invite rate applies to](https://bit.ly/9-Proxy)

## Where 9Proxy is weaker than its marketing suggests

Worth knowing before you pay, especially coming off a bad experience:

**No self-serve free trial.** There's nothing on the site that lets you validate IP quality against your own targets without buying first [6]. Trial access has been offered on request through 9Proxy's own community reps, who've described limited trials and 10 free IPs depending on availability [9] — that's a conversation with support, not a button.

**The refund terms are narrow.** The published credit-refund policy essentially covers IPs that die within about 60 seconds [7]. Framing matters here: if you buy a package that doesn't suit your use case, the money isn't coming back.

**Coverage is 90+ countries, not 195.** US, UK, Europe and Southeast Asia are well covered. If you need an unusual geography, verify it before committing rather than inferring it from the pool-size number [6].

**Trustpilot friction exists**, though the reviews cluster around refund-policy disputes rather than the proxy infrastructure itself [6]. Read it as a billing-expectations problem, not necessarily an IP-quality one.

**Streaming is not a use case on IP-based plans.** 9Proxy signalled in an updated Acceptable Use Policy that media streaming such as YouTube won't be supported on those plans — worth confirming current terms if that's anywhere near your workload [7].

**The pool is smaller than enterprise providers.** Around 20 million residential IPs, against 125M+ for Decodo or 150M+ for Bright Data [6]. For most individual practitioners and small teams that gap is theoretical; for very large distributed scraping it isn't.

## Migrating off 922 without repeating the mistake

Six steps, in this order:

1. **Write down the countries and cities you actually used on 922.** That list is your real requirement, not the number of IPs you had.
2. **Buy the smallest package that covers a real test.** The $30 bundle or the 200 GB tier, not the 50,000 IP tier.
3. **Run your real workflow, not a ping test.** Log into the accounts that matter, load the target sites, bind the proxy into your anti-detect browser, and push a payment page through it. A user review on AlternativeTo specifically calls out stable IPs and working setups with Dolphin Anty and AdsPower [10] — verify that on your own stack.
4. **Move accounts in small batches.** A handful at a time, and put fixed IPs behind anything you'd hate to lose.
5. **Never prepay more than a week or two of usage.** This is the entire 922 lesson. A provider going dark should cost you a week, not a quarter.
6. **Check the region, protocol and rotation mode your task needs before scaling.** IP-based plans require the desktop app for port forwarding; GB-based plans work straight from the dashboard with username/password or an IP whitelist [5]. Pick based on which one your tooling can actually consume.

## FAQ

**Is 922 Proxy coming back?**
No credible indication of it. Any site claiming to be a 922 relaunch, mirror, or balance-migration service should be treated as a scam until independently verified [3].

**Does 9Proxy offer a free trial?**
Not self-serve. Limited trial access has been discussed by 9Proxy's own representatives on community forums, subject to availability [9]. Plan on buying a small package to test.

**Should I buy IP-based or GB-based?**
IP-based when the same address has to survive multiple requests and bandwidth is heavy or unpredictable. GB-based when you rotate per request and each request is small. If you can't decide, the $30 bundle lets you test both.

**How many IPs do I need?**
Fewer than you think. Work out peaks of concurrent sessions rather than total requests. Most individual workflows fit well under 500 concurrent IPs; the 1,000+500 bonus tier is the value sweet spot if you're past that.

**Can I use 9Proxy with anti-detect browsers and scraping frameworks?**
Native SOCKS5 support means it drops into anti-detect browsers, proxychains and Python scripts without protocol conversion, and Scrapeless documents a working one-line endpoint swap [6][7].

## Bottom line

922 Proxy isn't a product you can review any more, because it isn't a product any more. It was one storefront on a shared residential infrastructure that Google dismantled in January 2026, and every balance on it died with the domains [3][4].

If you're replacing it, the useful criteria aren't pool size or per-IP headline price. They're whether the provider explains where its IPs come from, whether unused balance has an expiry, and whether you can test with a small package instead of a large one. 9Proxy scores well on the parts that are checkable: transparent published pricing across 23 packages, two billing models that map to genuinely different workloads, IPs that don't expire until used, and a 97.7% success rate against Cloudflare-protected targets in independent testing [5][6]. It scores less well on flexibility — no self-serve trial, and a refund window narrow enough that the trial you run is the one you bought.

Buy the small package first. Test your own targets. Scale when the numbers say so, not when the discount banner does.

👉 [Start with a 9Proxy package and test it on your own targets](https://bit.ly/9-Proxy)
