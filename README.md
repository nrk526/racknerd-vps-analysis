# vps under $5: what the current market actually offers, and how RackNerd's $21.99/year specials change the math

Five dollars a month buys very different things depending on who you buy from. As of the latest tracking data, six providers list eleven VPS plans under $5/month, ranging from $2.50 to $5.00 — and most of them are monthly clouds with half a gig of RAM and 10 GB of storage. There's a second route, though: yearly KVM specials that work out to less per month than any monthly plan on that list. RackNerd's entry special is $21.99 for a full year — about $1.83/month — with 1 GB RAM, 20 GB SSD and 3 TB of monthly traffic, and the price doesn't jump when you renew.

This article covers both routes: what the monthly market looks like right now, RackNerd's complete current specials lineup, the multi-year cost math most comparisons skip, the hidden limitations buried in the terms of service, and the refund and renewal rules you should know before committing to a yearly plan.

> **Quick take:** for most people searching for a vps under $5, the deciding factor is how long the server needs to live. Running something for months or years? RackNerd's 1 GB KVM VPS special at **$21.99/year** (renewal at the same price) is cheaper than every monthly option on the market, with double the RAM and six times the traffic of the $4 DigitalOcean plan. Need a box for a week or two, then gone? A monthly cloud plan fits that better. 👉 [Check RackNerd's current VPS specials and prices](https://bit.ly/RacKnerd)

## What $5 a month actually buys right now

The monthly market under $5 is a set of small, honest compromises. Here's what trackers recorded as of late October:

| Provider | Plan | Price/mo | RAM | Storage | Traffic & notes |
| --- | --- | --- | --- | --- | --- |
| Vultr | vc2-1c-0.5gb-v6 | $2.50 | 0.5 GB | 10 GB SSD | 0.5 TB; IPv6-focused variant |
| InterServer | KVM VPS 1 Slice | $3.00 ($1.50 first month) | 2 GB | 40 GB SSD | 2 TB, 10 Gbps port |
| InterServer | KVM Storage VPS 1 Slice | $3.00 ($1.50 first month) | 2 GB | 1 TB HDD | 2 TB, 10 Gbps; storage-oriented |
| Database Mart | Lite Linux VPS | $3.49 | 1 GB | 30 GB SSD | "Unlimited" traffic at 50 Mbps port |
| DigitalOcean | s-1vcpu-512mb-10gb | $4.00 | 0.5 GB | 10 GB SSD | 0.5 TB, 2 Gbps port |
| Database Mart | Express Linux VPS | $4.07 | 4 GB | 60 GB SSD | "Unlimited" traffic at 100 Mbps port |
| Clouvider | VPS.2 | €3.95/mo (5% off, ~$4.67) | 2 GB | 50 GB NVMe | 5 TB, 10 Gbps port |

A few things worth reading out of that table before you pick anything.

The headline-cheapest plan — Vultr at $2.50 — is the IPv6-focused sandbox variant. The regular IPv4 version of the same shape runs $3.50. If your project needs to be reachable over IPv4 (most do), the real floor is higher than the headline number.

InterServer's 2 GB slice at $3/month is the strongest spec sheet among monthly plans, helped by a first-month promo that cuts the initial bill to $1.50. And the "unlimited bandwidth" plans from Database Mart offset the word unlimited with heavily capped port speeds — 50 Mbps is fine for a blog, painful for anything serving files or running a proxy for daily use.

The real catch is what happens at month twelve. InterServer's slice costs $34.50 over the first year once the first-month discount is factored in, then $36.00 a year after that. DigitalOcean's half-gig plan costs $48 a year, every year. Neither price ever goes down.

## RackNerd's approach: yearly specials from $21.99

RackNerd doesn't sell a monthly plan under $5. Its standard monthly KVM line starts around $17.99/month for larger configurations, and the "$2.24/mo" figure you'll see on its homepage is the monthly equivalent of the cheapest annual tier — a 512 MB plan at $26.99/year (1 vCPU, 30 GB SSD, 500 GB traffic), which works out to roughly $2.25/month. That 512 MB tier is worth a mention for absolute minimum budgets, though half a gig of RAM and 500 GB of traffic limit it to very light duties: a tiny static site, a status page, maybe a lightweight proxy.

The main sub-$5 lineup is a set of five annual KVM VPS specials, all currently listed on the official specials page:

| Plan | vCPU | RAM | SSD | Traffic/mo | Price | Order |
| --- | --- | --- | --- | --- | --- | --- |
| 1 GB KVM VPS | 1 | 1 GB | 20 GB | 3 TB | **$21.99/yr** | [ Order the 1 GB plan](https://bit.ly/RacKnerd) |
| 2 GB KVM VPS | 2 | 2 GB | 35 GB | 5 TB | **$35.99/yr** | [ Order the 2 GB plan](https://bit.ly/RacKnerd) |
| 4 GB KVM VPS | 3 | 4 GB | 60 GB | 7 TB | **$59.99/yr** | [ Order the 4 GB plan](https://bit.ly/RacKnerd) |
| 6 GB KVM VPS | 6 | 6 GB | 100 GB | 12 TB | **$89.99/yr** | [ Order the 6 GB plan](https://bit.ly/RacKnerd) |
| 8 GB KVM VPS | 7 | 8 GB | 150 GB | 20 TB | **$119.99/yr** | [ Order the 8 GB plan](https://bit.ly/RacKnerd) |

Every plan ships with the same base: KVM virtualization, full root SSH access, one dedicated IPv4, a 1Gbps port, and the ctrl control panel for reboots, OS reinstalls, an HTML5 VNC console, bandwidth graphs, and firewall management. OS choices cover Ubuntu, Debian, AlmaLinux, Rocky Linux, CentOS, and Fedora; custom ISO installs are possible if you ask support first, and you can reinstall the OS yourself anytime later.

Only the 1 GB and 2 GB plans clear the under-$5 bar outright at $1.83 and $3.00 per month equivalent. The 4 GB plan lands exactly at $5.00/month if you divide by twelve — close enough to count, and it matters for reasons the next section explains. The 6 GB and 8 GB plans are listed for completeness since they sit on the same page and often make more sense per dollar once a project grows, but nobody would call them sub-$5 plans.

## The renewal math: where these plans actually separate from monthly clouds

Most comparison articles stop at the first bill. The more useful number is the second year.

RackNerd marks these specials as **lifetime recurring** — the price you sign up at is the price you renew at. That's the unusual part. Plenty of budget hosts lead with a cheap first term and reset to a much higher renewal rate; monthly clouds just keep billing full price forever.

Run the two-year comparison against the monthly options:

- **RackNerd 1 GB special:** $21.99 year one, $21.99 year two — $43.98 total
- **InterServer 2 GB slice:** $34.50 year one (with the first-month discount), $36.00 year two — $70.50 total, for 2 GB RAM but only two-thirds of the traffic
- **DigitalOcean 0.5 GB:** $48.00 per year, every year — $96.00 over two years, for half the RAM and a sixth of the traffic

By year two you're paying roughly 60% more (InterServer) to more than double (DigitalOcean) what the RackNerd special costs, for comparable or worse hardware in the DigitalOcean case. Over three years the gap widens further, because the special stays at $21.99.

The flip side is commitment. Yearly means paying upfront, and — this is the part to read carefully — there's no safety net the way there is with a monthly plan you can cancel tomorrow. More on that below.

## What you can actually run — and two restrictions hiding in the terms

RackNerd's ctrl panel includes one-click installs for self-hosted and AI applications, and the official specials page is unusually specific about what fits where. These minimums are the honest deciding factor between plans:

- **n8n, Coolify** — comfortable from 2 GB RAM
- **Ollama, AnythingLLM, LibreChat, Hermes Agent** — need at least 4 GB RAM
- **OpenClaw** — needs at least 8 GB RAM
- **CyberPanel, CloudPanel, Docker + Portainer, AdminBolt** — fine on 1 GB

The practical takeaway: if your sub-$5 search is really about self-hosting an automation stack or running a local LLM frontend, the 1 GB plan will disappoint you immediately. Ollama and friends require the 4 GB special at $59.99/year — right at the $5/month line, and the last plan in the lineup that fits this budget. Meanwhile the classic use cases for a cheap box (WordPress blog, WireGuard node, reverse proxy, Discord bot, Git server, uptime monitoring) run fine on 1 GB, and 3 TB of monthly traffic is genuinely hard to exhaust with any of them.

Two restrictions from RackNerd's terms of service that most roundups never mention:

**Nested virtualization is off by default.** You can't run VMs inside your KVM VPS — no hypervisors, VPS resale platforms, or emulators that need hardware virtualization — without written approval, and RackNerd doesn't guarantee the VT-x/AMD-V CPU flags are exposed. Containers are explicitly fine: Docker, Docker Compose, LXC/LXD, Kubernetes, K3s all work. If your plan involves running virtual machines inside the VM, you'd need a dedicated server instead.

**Crypto mining is banned outright**, along with bulk mailing, brute-forcing, outbound DDoS, and traffic exchange. Cheap bandwidth attracts mining attempts, and getting suspended for abuse also forfeits any shot at a refund.

One limitation to state plainly while we're here: these are **unmanaged** VPS. RackNerd's 24/7 support covers the platform — network, hardware, the panel — but if your OS breaks or your web server config is broken, that's yours to fix. At this price point that's standard across the market, not a RackNerd quirk.

## Refunds, cancellation, and renewal: read this before paying yearly

This is the section most budget VPS roundups skip, and it's the one that most often surprises yearly buyers. RackNerd's terms do **not** include a money-back guarantee: once payment is received, refunds are handled case-by-case, with no automatic refund window. Account credit you've prepaid is explicitly non-refundable and non-withdrawable.

What that means in practice:

- **Just paid and haven't really used the server?** Opening a billing ticket promptly is worth a shot — refunds at this stage get handled case-by-case, and reporting a genuine problem (server won't boot, IP unreachable) is the scenario where requests have a chance.
- **Mid-cycle change of mind?** Realistically no refund. Your option is cancelling at the end of the billing period and letting the term run out.
- **Renewal you didn't want?** Cancellation requests go through the client area before the renewal date — third-party write-ups of the policy put the notice window at around five days for standard services. Miss it, the card gets charged, and the default-no-refund rule applies to that charge too. If you buy yearly, a calendar reminder a week before renewal is cheap insurance.
- **Instant cancellation** terminates the service within about 24 hours and deletes all data immediately and permanently — so back up before cancelling, and if you click it by accident, open a ticket right away to ask for restoration.
- **Chargebacks** are the worst path: the official terms state that disputes filed after an abuse-related penalty trigger an administrative fee of **$125–$250**, plus possible account suspension. Always go through a ticket first.

None of this makes the 1 GB special a bad deal — $21.99 is a small enough amount that many buyers treat the risk as part of the price — but it does mean you should pick the datacenter deliberately rather than treating the purchase as refundable experimentation. RackNerd lists around 20 locations across North America, Europe and Asia (Los Angeles, Dallas, New York, Chicago, Seattle, San Jose, Atlanta, Ashburn, Tampa, Toronto, Amsterdam, London, Dublin, Strasbourg and Utah among them), and per its own documentation each location has test download files and looking glass tools so you can check latency before ordering. One caveat worth knowing: the cheapest tiers in popular locations go in and out of stock, so if your first-choice location is unavailable, check what else is open rather than assuming the plan is gone.

## Ordering: what happens after you click

The order flow is short: pick a plan, choose your datacenter location and OS on the configuration page, check out, and pay — RackNerd accepts PayPal, credit cards, cryptocurrency, and bank wire. Provisioning is automatic and, per the company's own blog, most VPS come online within 5–15 minutes.

Two details worth knowing ahead of time, both straight from that official ordering guide. First, your login credentials arrive in two separate emails: an order confirmation, then a dedicated "KVM VPS Login Information" email with the IP, root SSH password, and ctrl panel address. Second, the ctrl panel login is distinct from your client area account — a common stumbling block for first-time buyers. If either email goes missing, check spam first; the "View Email Log" option in the client area can recover them. 👉 [Start the order process for a RackNerd special](https://bit.ly/RacKnerd)

If something looks wrong right after deployment, the company's advice is to open a support ticket immediately rather than noting it in the order comments — and given the case-by-case refund policy above, that early ticket doubles as your paper trail if you end up needing one.

## Monthly or yearly: picking the right billing shape

The honest answer to "vps under $5" depends on server lifespan, and it's worth being direct about where each option wins.

Monthly clouds — Vultr, DigitalOcean, InterServer and the rest — win when the server is disposable. Spinning a machine up for a two-week test, a migration, or a burst project and then destroying it is exactly what hourly/monthly billing exists for. On that timeline, nobody's yearly special makes sense.

RackNerd's specials win when the server has a pulse beyond a couple of months. A blog, a proxy node, a bot, a home lab box, a small production app — anything you'd still be paying for in month six is cheaper on a $21.99–$35.99/year special than on any monthly plan, and the lifetime renewal pricing protects the second and third year. The trade is upfront payment plus a no-refund policy, which is a reasonable exchange at these amounts if you've checked the location and specs first.

If you want to de-risk the decision without paying for a monthly plan elsewhere, one workable sequence: check the location's looking glass before ordering, start with the smallest plan that meets your RAM floor, and scale up next year rather than overbuying now.

## FAQ

**Is a VPS under $5/month good enough for a real website?**
For a small blog or lightweight app, yes — 1–2 GB of RAM covers most simple stacks. RackNerd's 2 GB special at $35.99/year is a sensible production-budget pick with 5 TB of traffic. High-traffic sites or database-heavy apps outgrow this bracket quickly; the 4 GB tier is the realistic ceiling of the sub-$5 budget.

**Does RackNerd raise the price when you renew a special?**
No — the specials are marked as lifetime recurring, meaning renewal happens at the same annual price you signed up at. This is the main structural difference from hosts that use first-term discounts.

**Can I get a refund if I change my mind?**
There's no money-back guarantee; refunds are handled case-by-case through billing tickets, and prepaid account credit is not refundable. Fresh orders with a genuine technical problem have the best case. Cancelling stops future renewals but doesn't reclaim payments already made.

**Can I run Docker or VMs on a RackNerd special?**
Docker, LXC/LXD and Kubernetes work normally. Running virtual machines inside the VPS is prohibited by default unless you get written approval, since nested hardware virtualization isn't guaranteed on these plans.

**Does RackNerd have a monthly plan under $5?**
No. Its standard monthly KVM plans start around $17.99/month, and the homepage's "$2.24/mo" is the monthly equivalent of the $26.99/year 512 MB tier. The sub-$5 pricing on the main specials only comes from dividing the annual price by twelve — which is why the billing shape matters as much as the price.

**Which payment methods does RackNerd take?**
PayPal, credit cards, cryptocurrency, and bank wire. Crypto is a practical option if PayPal or card payments are awkward in your region — just remember that platform tickets are essentially your only recourse on non-card payments, since there's no chargeback mechanism.

## Which plan to actually get

- **Blog, bot, proxy, small self-hosted tools** → 1 GB special, $21.99/year. $1.83/month for 3 TB of traffic is the cheapest credible way to keep a small server alive long-term.
- **n8n, Coolify, or a small app with a database** → 2 GB special, $35.99/year. Two cores and 5 TB at $3/month equivalent is the sweet spot.
- **Anything LLM-related** → 4 GB special, $59.99/year. It's the minimum for Ollama, AnythingLLM, LibreChat and friends, and the last plan that fits $5/month.
- **A server you need for days, not months** → a monthly plan from Vultr or DigitalOcean fits that workflow better than any yearly commitment; RackNerd's economics only kick in when the box stays up.
- **Absolute rock-bottom budget, very light usage** → the 512 MB tier at $26.99/year exists, but half a gig of RAM is unforgiving; the 1 GB special is only $5 more per year and is the better buy for almost everyone.

Before you click order on any of them, three last checks: confirm your preferred datacenter has stock, verify the plan meets the RAM floor for whatever you're installing, and set a renewal reminder for next year so the auto-billing never surprises you. 👉 [Order the RackNerd 1 GB KVM VPS special at $21.99/year](https://bit.ly/RacKnerd)
