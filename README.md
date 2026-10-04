# iproyal review: what you actually pay per GB, where the advertised price breaks down, and when per-IP billing is the cheaper call

Most people searching for an IPRoyal review are stuck on one number. They saw "residential proxies from $1.75/GB" somewhere, opened the pricing page, and now they're trying to work out whether that figure is real or bait. The second group already runs a project, has a balance sitting in an IPRoyal account, and wants to know what the per-gigabyte rate is actually going to cost them next month.

Both questions have concrete answers, and neither one is "it's a scam" or "it's the best." IPRoyal is a real mid-market provider with a real network and a genuinely useful feature — residential credit that doesn't reset every month. It also advertises a price floor that almost nobody can buy at. Sorting those two facts apart is basically what this review is for.

## IPRoyal's lineup, briefly

The company sells four proxy types plus a couple of extras:

- **Rotating residential** — pay-as-you-go traffic, 195+ countries, the product most people come for
- **ISP / static residential** — dedicated IPs from consumer ISPs, billed per IP with unlimited traffic
- **Datacenter** — cheaper, faster, more likely to get flagged on protected sites
- **Mobile** — 3G/4G/5G exit nodes, billed per proxy per month
- **Web Unblocker** — the separately priced unblocking layer, quoted at around $1.00 per 1,000 requests

There's no qualification gate to open an account, which matters more than it sounds if you've ever tried to onboard with Bright Data or Oxylabs and gotten bounced to a sales call.

## The per-gigabyte number, and why it moves

This is the part worth reading slowly. IPRoyal advertises every product with a "from" price, and on most of them that price sits at the bottom of a volume or commitment curve rather than at the checkout button.

| Product | Advertised "from" | What a new buyer pays | What unlocks the floor |
| --- | --- | --- | --- |
| Residential | $1.75/GB | $7.35/GB (pay-as-you-go, first GB) | ~10TB bulk, custom quote |
| ISP / static residential | $1.80/IP | $2.70/IP for 30 days | 60-day or 90-day term |
| Datacenter | $1.39/IP | ~$1.57/IP | 90-day commitment |
| Mobile | $117/mo | ~$130/mo | 90-day commitment |

Residential is where the gap gets wide — roughly 4x between the headline and the first gigabyte a normal person can buy. The subscription tab shaves 5% off every tier ($7.00 instead of $7.35 at the entry point), but it's a recurring charge, so you're trading flexibility for a rounding error unless your monthly consumption is genuinely predictable.

The discount curve is also front-loaded. Going from one gigabyte to two cuts the rate by around 15%, which is the biggest single step in the whole residential schedule. After that it flattens hard. At 10GB you're still paying close to three times the advertised floor. Bulk pricing crosses into the $1.75–$2.00/GB range only at volumes most individual buyers will never touch.

One more wrinkle: third-party writeups quote wildly different entry rates for the same product — $3.50/GB in one directory, $7.99 for the first gigabyte and $5.15/GB up to 50GB in PCMag's comparison. That's not necessarily error. It's what happens when the price you're shown depends on tier, commitment and whether you're on the subscription or pay-as-you-go tab. IPRoyal's own blog states residential access starts at $7.00/GB on subscription and $7.35/GB pay-as-you-go, with bulk down to $1.75/GB — which lines up with the higher figures you'll find elsewhere, not the lower ones.

## Where IPRoyal is actually strong

Three things stand out, and they're not marketing points.

**Traffic that doesn't expire.** Residential balance sits until you spend it, in pay-as-you-go mode. If your scraping schedule is lumpy — heavy in March, quiet in April — you don't lose anything by pausing. That's unusual enough in this category to be worth calling out.

**Static residential pricing is sensible.** A handful of ISP proxies at $2.70/IP on a 30-day term, dropping with a 60-day (5% off) or 90-day (10% off) commitment, comes to somewhere around $8–14 a month with unlimited traffic. If your job is "see my storefront the way a customer in Germany sees it" or "check that my ads render in Australia," that's the whole budget, and it never needs to grow.

**Payment and access are uncomplicated.** 25+ cryptocurrencies accepted, cards, no enterprise onboarding theatre, and a dashboard that reviewers consistently describe as clean. PCMag noted the interface is well-organised and easy to navigate.

## Where the review gets less flattering

Some of this is industry-normal, and some of it is worth knowing before you pay.

The ISP pricing is genuinely confusing. The homepage and the pricing index advertise ISP proxies "from $1.80/IP" with no duration attached — which reads monthly, because every competitor quotes ISP proxies monthly. Open the ISP product page and that same $1.80 is the 24-hour tier. A plain 30-day month is $2.70. The product page footer states the product starts from the 90-day rate, so two IPRoyal pages were quoting two different starting prices for the same product on the same day. It reads like a page that fell out of sync rather than a trick, but the effect on anyone comparing ISP prices across vendors is the same.

A few smaller things surface in reviews: IPRoyal charges for changes like renaming a proxy, which Decodo doesn't. Individual users don't get a free trial — the practical substitute is a one-day proxy at $1.80, and free trials are reserved for verified companies. KYC isn't mandatory for residential access, but completing it unlocks more ports, PayPal payments, and access to government and banking domains, so if you need those, verification is effectively required.

Then there's the refund policy. PCMag's head-to-head put IPRoyal behind Decodo partly on "questionable pricing and refund policies," and refund complaints are a recurring theme in community threads. It's not a scam, but it is a provider you should test at the smallest possible size before committing real budget.

One fair point that gets over-argued: IPRoyal sources a chunk of its residential pool through Pawns.app, an app that pays people to share idle bandwidth. PCMag reads that proprietary arrangement with some scepticism. In practice, nearly every large residential network is assembled this way — an SDK in someone's app or a standalone bandwidth-sharing client. IPRoyal is on the more transparent end because it runs the app under its own name. The trade-off is the same either way: real home connections that come and go.

## The billing model question nobody asks before buying

Here's the thing that actually costs people money, and it isn't IPRoyal-specific.

Residential proxies are usually sold by the gigabyte. That model is fine for high-rotation work where each request moves a small payload — scraping listings, checking geo-targeted prices, polling an API. It's terrible for the opposite workload: a small, stable set of IPs doing heavy data transfer. Long sessions, media, large downloads, account-based workflows where you hold one identity for weeks. Under per-GB billing, everything you transfer is metered, so a handful of IPs handling serious volume can run to hundreds of dollars a month.

The alternative is billing per IP with unlimited bandwidth, which caps that cost at the price of the IP. If your workload looks like five accounts that each need a consistent residential IP and move a lot of data, the per-GB model is the wrong shape entirely, no matter which provider you buy it from.

That's the honest reason to look past IPRoyal: not that its proxies are bad, but that a bandwidth-metered model is the wrong product for some jobs.

## 9Proxy, and the caveat that has to come first

9Proxy is a residential proxy platform that sells both ways — packages billed per IP with unlimited bandwidth, and packages billed per GB with rotating endpoints. It advertises 20M+ residential IPs across 90+ countries, HTTP/HTTPS and SOCKS5 support, targeting down to state, city, ZIP and ISP level, and a 60-second refund that credits you back if a proxy fails immediately after activation. Billing is balance-based rather than subscription-based, and unused balances don't get swept at the end of a month.

Now the caveat, because it's not small and burying it would be the wrong thing to do.

> 9Proxy went dark on June 28, 2026. Site, dashboard, desktop app and support all went silent. The company acknowledged "a service disruption" on June 29 and said it was prioritising "a stable and secure recovery rather than a rushed fix," without naming a cause or an ETA. Prepaid balances were inaccessible for roughly two and a half weeks. The service came back around July 15. Purchases were still officially paused into mid-July, and a status update on August 14 said GB-based plans were restored while IP-based plans remained under maintenance with no confirmed date. Uptime trackers logged another brief dip in mid-September.

So: budget accordingly. Don't park a year of spend in the dashboard, test with a small package first, and keep a funded second provider if your pipeline can't tolerate a two-week blackout. That's true of every provider in this category in 2026, but it's especially true here.

If that risk profile works for you, the entry prices are low enough that testing is cheap: 👉 [check the current 9Proxy packages and rates](https://bit.ly/9-Proxy).

## 9Proxy's full plan line-up

Prices below reflect the adjustment 9Proxy applied to IP-based and bundle packages on June 1, 2026. GB-based pricing was left unchanged.

**Residential by IP — fixed package price, unlimited bandwidth**

| Package | Cost per IP | Total | Buy |
| --- | --- | --- | --- |
| 100 IPs | $0.24 | $24 | [Get 100 IPs](https://bit.ly/9-Proxy) |
| 500 IPs | $0.144 | $72 | [Get 500 IPs](https://bit.ly/9-Proxy) |
| 1,000 IPs + 500 bonus | $0.084 | $126 | [Get 1,500 IPs](https://bit.ly/9-Proxy) |
| 2,500 IPs | $0.084 | $210 | [Get 2,500 IPs](https://bit.ly/9-Proxy) |
| 5,000 IPs | $0.072 | $360 | [Get 5,000 IPs](https://bit.ly/9-Proxy) |
| 15,000 IPs | $0.048 | $720 | [Get 15,000 IPs](https://bit.ly/9-Proxy) |
| 25,000 IPs | $0.035 | $863 | [Get 25,000 IPs](https://bit.ly/9-Proxy) |
| 50,000 IPs | $0.029 | $1,438 | [Get 50,000 IPs](https://bit.ly/9-Proxy) |

**Business IP packages**

| Package | Cost per IP | Total | Buy |
| --- | --- | --- | --- |
| 100,000 IPs | $0.023 | $2,300 | [Get 100,000 IPs](https://bit.ly/9-Proxy) |
| 200,000 IPs | $0.021 | $4,140 | [Get 200,000 IPs](https://bit.ly/9-Proxy) |
| 500,000 IPs | $0.018 | $8,625 | [Get 500,000 IPs](https://bit.ly/9-Proxy) |

**Residential by GB — 180-day validity, rotating endpoints**

| Package | Cost per GB | Total | Buy |
| --- | --- | --- | --- |
| 5 GB | $3.00 | $15 | [Get 5 GB](https://bit.ly/9-Proxy) |
| 50 GB + 5 GB bonus | $2.10 | $105 | [Get 55 GB](https://bit.ly/9-Proxy) |
| 100 GB | $1.50 | $150 | [Get 100 GB](https://bit.ly/9-Proxy) |
| 200 GB | $1.00 | $200 | [Get 200 GB](https://bit.ly/9-Proxy) |
| 1,000 GB | $0.80 | $800 | [Get 1,000 GB](https://bit.ly/9-Proxy) |
| 2,000 GB | $0.75 | $1,500 | [Get 2,000 GB](https://bit.ly/9-Proxy) |

Enterprise GB packages with unlimited validity run at custom pricing through sales.

**Bundles — IPs plus traffic in one package**

| Bundle | Contents | Price | Buy |
| --- | --- | --- | --- |
| Starter | 100 IPs + 5 GB | $30 | [Get the Starter bundle](https://bit.ly/9-Proxy) |
| Popular | 1,500 IPs + 50 GB | $180 | [Get the Popular bundle](https://bit.ly/9-Proxy) |
| Pro | 5,000 IPs + 500 GB | $720 | [Get the Pro bundle](https://bit.ly/9-Proxy) |

Two things to know before you buy. The IP-based model requires the desktop app, because it works through local port forwarding rather than a plain username-and-password endpoint — that's a real difference if you're deploying to a headless server. The GB-based model works straight from the dashboard with username/password or IP whitelist authentication, no app needed. IP-based proxies also have natural session lifetimes of a few hours up to about 24 hours, so they suit account-based work rather than rapid rotation.

If you're testing, start where the money is smallest: 👉 [grab the 5 GB package](https://bit.ly/9-Proxy) if your job rotates IPs, or 👉 [take 100 IPs](https://bit.ly/9-Proxy) if it holds them. A test balance is also available on request, which is the cheapest possible way to find out whether the pool survives contact with your actual targets.

## IPRoyal vs 9Proxy, without the sales voice

|  | IPRoyal | 9Proxy |
| --- | --- | --- |
| Entry residential price | $7.00–$7.35/GB | $3.00/GB, or $0.24/IP with unlimited traffic |
| Billing models | Per GB (residential), per IP (ISP/datacenter) | Per GB and per IP |
| Traffic validity | Doesn't expire in pay-as-you-go mode | 180 days on GB packages; IPs don't expire |
| Proxy types | Residential, ISP, datacenter, mobile | Residential (IP-based and GB-based) |
| Targeting | Country, state, city on residential | Country, state, city, ZIP, ISP |
| Free trial | None for individuals; paid 1-day proxy | Test balance on request |
| Crypto | 25+ currencies | USDT, BTC, ETH, LTC, DOGE and others |
| Support | 24/7 chat and email, ~58s average response claim | 24/7 via Telegram, email, tickets |
| Track record | Years of operation, no major outages reported | Two 2026 outages, purchases paused in July |
| Get started | — | [Create a 9Proxy account](https://bit.ly/9-Proxy) |

The pattern here isn't "one is better." IPRoyal is the more established operation with broader product coverage and a longer track record. 9Proxy is cheaper per gigabyte and offers an unlimited-bandwidth-per-IP option IPRoyal only really matches in its ISP line. Neither difference matters until you know which billing model your workload needs.

## Which one to actually pick

Answer one question first: how much data do you move per IP?

If a small set of IPs carries most of your volume — account management, long authenticated sessions, media, anything where you'd rather not watch a meter — you want per-IP pricing, and IPRoyal's residential product is the wrong shape for that job. Its ISP line works, at $2.70/IP for 30 days. 9Proxy's IP packages work too, at $0.24/IP for the first hundred, and the fact that unused IPs don't expire means a failed test isn't money torched.

If you rotate through thousands of IPs and each request moves little data, buy gigabytes, and the honest comparison is $7.35/GB at IPRoyal's entry point against $3.00/GB at 9Proxy's. Both have volume curves; IPRoyal's is steeper at the top end, 9Proxy's starts lower.

And if you're not sure yet, spend $15 or $24 rather than $200. A GB package or a hundred IPs will tell you more about success rates against your specific targets than any review will.

## FAQ

**Is IPRoyal legit, or a scam?**

Legitimate, and it's been operating for years with a real residential, ISP, datacenter and mobile network. The complaints that recur are about pricing transparency and refund handling, not about proxies that never work.

**Does IPRoyal's traffic expire?**

Residential traffic bought pay-as-you-go sits in your account until you use it — no monthly reset. Confirm the current terms on the site before you budget around it, because this is exactly the kind of policy providers revise.

**Does IPRoyal have a free trial?**

Not for individuals. The closest thing is a one-day proxy at $1.80. Free trials are offered to verified companies.

**Why is IPRoyal's advertised price so much lower than what I'm charged?**

The "from" prices sit at the bottom of volume or commitment curves. Residential hits $1.75/GB around 10TB by custom quote. ISP hits $1.80/IP on a 24-hour term, not a month.

**What's a cheaper alternative if my budget is small?**

If your workload is bandwidth-heavy on a few IPs, an unlimited-bandwidth per-IP package will usually beat any per-gigabyte provider. 9Proxy's smallest IP package is $24 for 100 IPs, and the smallest GB package is $15 — but weigh that against its 2026 outage record, and keep a fallback funded.

## Bottom line

IPRoyal earned its place. Non-expiring residential traffic, sensible static IP pricing, no qualification gate, and a product range that covers most jobs a small team runs into. What it doesn't do is sell a small buyer a cheap gigabyte, and the advertised floor is not a price anyone reading this will pay. Budget $7–$8 per gigabyte unless you're committing to volumes that make a custom quote worthwhile.

9Proxy is the sharper deal on paper for bandwidth-heavy and per-IP work, at a real and documented reliability cost — two 2026 outages, a two-week blackout, prepaid balances frozen, and IP-based plans still working through maintenance as of the last public status update. Cheap and unproven beats expensive and unproven only if you keep a second provider on standby. 👉 [Compare both options starting from $15](https://bit.ly/9-Proxy) and test against your own targets before you scale either one.
