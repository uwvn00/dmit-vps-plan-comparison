# dmit vps review: Is the $36.9/Year Plan Actually CN2 GIA, How Do Pro and Eyeball Differ, and Which Tier Is Worth the Premium? (Full Plan Tables + Refund Rules)

The $36.9/year plan is **LAX.AN4.T1 WEE**, and it runs on DMIT's Tier 1 international route with no China-mainland optimization whatsoever. If CN2 GIA is what you came for, the cheapest entry is **LAX.AN4.Pro TINY at $88.88/year**, which gets you the same 1TB of monthly traffic, double the RAM, and a genuine three-network GIA return path.

What follows is what that $36.9 actually buys, where the three product lines diverge once Beijing hits 8pm, the two pricing traps that make identical-looking plans cost 35% more, and every plan on the current sheet with the billing period spelled out.

> **Quick verdict**
> - **No China route needed, lowest entry cost:** LAX.AN4.T1 WEE, $36.90/year, 1TB/month, throttled to 100Mbps instead of suspended when you exceed it.
> - **China-optimized on a budget:** Eyeball AN4 TINY, $88.88/year, 1,500GB/month on a 2Gbps port, CMIN2 for mobile and 9929/CN2 for telecom and Unicom.
> - **Most stable at peak:** Premium AN4 TINY, $88.88/year for 1,000GB, or $29.90/month for STARTER once 1TB stops being enough.
> 👉 [See current DMIT plans, prices and stock](https://www.dmit.io/aff.php?aff=9081)

## What the $36.9/year LAX.AN4.T1 WEE actually is

One core on an AMD EPYC 9004, 1GB RAM, 20GB SSD, 1TB of monthly traffic counted as the larger direction of in/out, one IPv4 plus an IPv6 /64, Los Angeles. That is the whole spec sheet.

The traffic policy is the part worth reading twice. Go over 1TB and the box does not get suspended and you do not get a surprise invoice. It drops to 100Mbps and keeps running. Hong Kong and Tokyo T1 plans throttle to 50Mbps instead, according to one review's FAQ, so the Los Angeles WEE is the better of the three if you expect to blow through the quota.

T1 means NTT, Lumen and other Tier 1 carriers, with CMI for China Mobile. Telecom and Unicom connections run acceptably outside peak hours. During the evening peak, one review describes visible speed fluctuation and rates the plan as "a cheap way to try the door rather than a first-choice main machine." That matches the price.

Four scenarios where it earns its keep: a landing node you front with your own relay; a site whose audience is mostly outside mainland China; scripts, CI and dev environments that don't care about routing; and testing DMIT's hardware and stability before spending GIA money.

## Every current DMIT plan and price

Pricing below is the listed rate, not a first-year discount. **Check the `/mo` and `/yr` column before comparing anything.** GENERAL runs EPYC 9004, VOLUME runs EPYC 9005.

### Los Angeles, T1 international

| Plan | vCPU / RAM / SSD | Traffic/mo | Port | Price | Order |
| --- | --- | --- | --- | --- | --- |
| T1 GENERAL · WEE | 1 / 1GB / 20GB | 1TB | 100Mbps after overage | **$36.90/yr** | [ See plan](https://www.dmit.io/aff.php?aff=9081) |
| T1 GENERAL · TINY | 1 / 1GB / 20GB | 2TB | 10Gbps | $6.90/mo | [ See plan](https://www.dmit.io/aff.php?aff=9081) |
| T1 GENERAL · STARTER | 1 / 2GB / 40GB | 4TB | 10Gbps | $12.90/mo | [ See plan](https://www.dmit.io/aff.php?aff=9081) |
| T1 GENERAL · MINI | 2 / 2GB / 60GB | 8TB | 10Gbps | $21.90/mo | [ See plan](https://www.dmit.io/aff.php?aff=9081) |
| T1 GENERAL · MICRO | 4 / 4GB / 80GB | 16TB | 10Gbps | $32.90/mo | [ See plan](https://www.dmit.io/aff.php?aff=9081) |
| T1 VOLUME · V2C2G | 2 / 2GB / 40GB | 5TB | 10Gbps | $14.90/mo | [ See plan](https://www.dmit.io/aff.php?aff=9081) |
| T1 VOLUME · V2C4G | 2 / 4GB / 80GB | 10TB | 10Gbps | $23.90/mo | [ See plan](https://www.dmit.io/aff.php?aff=9081) |
| T1 VOLUME · V4C4G | 4 / 4GB / 120GB | 20TB | 10Gbps | $36.90/mo | [ See plan](https://www.dmit.io/aff.php?aff=9081) |
| T1 VOLUME · V4C8G | 4 / 8GB / 160GB | 40TB | 10Gbps | $52.90/mo | [ See plan](https://www.dmit.io/aff.php?aff=9081) |
| T1 VOLUME · V8C16G | 8 / 16GB / 240GB | 80TB | 10Gbps | $119.90/mo | [ See plan](https://www.dmit.io/aff.php?aff=9081) |
| T1 VOLUME · V12C24G | 12 / 24GB / 320GB | 160TB | 10Gbps | $199.90/mo | [ See plan](https://www.dmit.io/aff.php?aff=9081) |

### Los Angeles, Premium (three-network CN2 GIA)

Same plan name, two hardware generations, two different prices.

| Plan | vCPU / RAM / SSD · port | Traffic/mo | AN4 (EPYC 9004) | AN5 (EPYC 9005) | Order |
| --- | --- | --- | --- | --- | --- |
| TINY | 1 / 2GB / 20GB · 1Gbps | 1,000GB | **$88.88/yr** | $119.99/yr | [ See plan](https://www.dmit.io/aff.php?aff=9081) |
| Pocket | 2 / 2GB / 40GB · 4Gbps | 1,500GB | $159.98/yr | $203.90/yr | [ See plan](https://www.dmit.io/aff.php?aff=9081) |
| STARTER | 2 / 2GB / 80GB · 10Gbps | 3,000GB | $29.90/mo | $38.90/mo | [ See plan](https://www.dmit.io/aff.php?aff=9081) |
| MINI | 4 / 4GB / 80GB · 10Gbps | 5,000GB | $58.88/mo | $76.90/mo | [ See plan](https://www.dmit.io/aff.php?aff=9081) |
| MICRO | 4 / 4GB / 160GB · 10Gbps | 7,000GB | $74.99/mo | $99.90/mo | [ See plan](https://www.dmit.io/aff.php?aff=9081) |
| MEDIUM | 6 / 8GB / 160GB · 10Gbps | 15,000GB | $168.88/mo | $219.90/mo | [ See plan](https://www.dmit.io/aff.php?aff=9081) |
| LARGE | 8 / 16GB / 320GB · 10Gbps | 25,000GB | $338.88/mo | $459.90/mo | [ See plan](https://www.dmit.io/aff.php?aff=9081) |
| GIANT | 12 / 24GB / 640GB · 10Gbps | 50,000GB | $619.99/mo | $839.90/mo | [ See plan](https://www.dmit.io/aff.php?aff=9081) |

### Los Angeles, Eyeball (9929 / CN2 for telecom and Unicom, CMIN2 for mobile)

| Plan | vCPU / RAM / SSD · port | Traffic/mo | AN4 (EPYC 9004) | AN5 (EPYC 9005) | Order |
| --- | --- | --- | --- | --- | --- |
| TINY | 1 / 2GB / 20GB · 2Gbps | 1,500GB | **$88.88/yr** | $119.99/yr | [ See plan](https://www.dmit.io/aff.php?aff=9081) |
| Pocket | 2 / 2GB / 40GB · 4Gbps | 3,000GB | $159.98/yr | $203.90/yr | [ See plan](https://www.dmit.io/aff.php?aff=9081) |
| STARTER | 2 / 2GB / 80GB · 10Gbps | 5,000GB | $29.90/mo | $38.90/mo | [ See plan](https://www.dmit.io/aff.php?aff=9081) |
| MINI | 4 / 4GB / 80GB · 10Gbps | 10,000GB | $58.88/mo | $76.90/mo | [ See plan](https://www.dmit.io/aff.php?aff=9081) |
| MICRO | 4 / 4GB / 160GB · 10Gbps | 14,000GB | $74.99/mo | $99.90/mo | [ See plan](https://www.dmit.io/aff.php?aff=9081) |
| MEDIUM | 6 / 8GB / 160GB · 10Gbps | 30,000GB | $168.88/mo | $219.90/mo | [ See plan](https://www.dmit.io/aff.php?aff=9081) |
| LARGE | 8 / 16GB / 320GB · 10Gbps | 50,000GB | $338.88/mo | $459.90/mo | [ See plan](https://www.dmit.io/aff.php?aff=9081) |
| GIANT | 12 / 24GB / 640GB · 10Gbps | 100,000GB | $619.99/mo | $839.90/mo | [ See plan](https://www.dmit.io/aff.php?aff=9081) |

### Hong Kong and Tokyo (AS3 platform, EPYC 7003)

| Plan | vCPU / RAM / SSD | Traffic/mo | Price | Order |
| --- | --- | --- | --- | --- |
| HKG.AS3.Pro · TINY | 1 / 1GB / 10GB | 300GB | $21.90/mo | [ See plan](https://www.dmit.io/aff.php?aff=9081) |
| HKG.AS3.Pro · STARTER | 1 / 2GB / 20GB | 500GB | $32.90/mo | [ See plan](https://www.dmit.io/aff.php?aff=9081) |
| HKG.AS3.Pro · MINI | 2 / 2GB / 40GB | 1,000GB | $54.90/mo | [ See plan](https://www.dmit.io/aff.php?aff=9081) |
| HKG.AS3.T1 · WEE | 1 / 1GB / 20GB | 1TB | $36.90/yr | [ See plan](https://www.dmit.io/aff.php?aff=9081) |
| HKG.AS3.T1 · TINY | 1 / 1GB / 20GB | 2TB | $6.90/mo | [ See plan](https://www.dmit.io/aff.php?aff=9081) |
| TYO.AS3.Pro · TINY | 1 / 1GB / 10GB | 300GB | $21.90/mo | [ See plan](https://www.dmit.io/aff.php?aff=9081) |
| TYO.AS3.Pro · STARTER | 1 / 2GB / 20GB | 500GB | $32.90/mo | [ See plan](https://www.dmit.io/aff.php?aff=9081) |
| TYO.AS3.T1 · WEE | 1 / 1GB / 20GB | 1TB | $36.90/yr | [ See plan](https://www.dmit.io/aff.php?aff=9081) |
| TYO.AS3.T1 · TINY | 1 / 1GB / 20GB | 2TB | $6.90/mo | [ See plan](https://www.dmit.io/aff.php?aff=9081) |

## Pro vs Eyeball vs T1: where the extra money goes

All three lines run on the same EPYC hardware and the same KVM stack. The difference is entirely the return path.

**Premium** is three-network CN2 GIA (AS4809): GIA on the outbound for telecom and Unicom, CMI for mobile, and GIA on the return for all three. **Eyeball** keeps telecom and Unicom on CN2 or 9929 and pushes mobile over CMIN2, which is cheaper to provision and lands better for mobile-heavy audiences. **T1** is plain international transit.

The gap is small during the day and obvious at night. One long-term user review puts Premium's packet loss under 1% during the 20:00–24:00 Beijing window, with Eyeball climbing to 5%–15% over the same hours. Treat those as one reviewer's measurements rather than a spec, but the direction matches what the routing differences would predict. Reported latency: roughly 150–180ms from Los Angeles to mainland China, with Premium described as staying inside a 20ms swing at peak.

Here is the decision most people get wrong. At **$88.88/year**, Pro TINY and EB TINY cost exactly the same. Pro gives you 1,000GB and a 1Gbps port with the best return path. EB gives you 1,500GB and a 2Gbps port with a good-but-not-top return path. Same money, and the choice is routing quality against 50% more traffic. If your audience is on China Mobile and mostly daytime, EB is the better buy. If you are running anything latency-sensitive at night, pay for Pro.

👉 [Compare Premium and Eyeball at the same price point](https://www.dmit.io/aff.php?aff=9081)

## The two price traps: monthly vs annual, and EPYC 9004 vs 9005

**Same name, different generation.** AN4 Pro TINY is $88.88/year. AN5 Pro TINY is $119.99/year for an identical 1 vCPU / 2GB / 20GB / 1,000GB / 1Gbps spec. That is $31.11 more for a newer CPU generation. The EB line repeats the pattern exactly: $88.88 versus $119.99. Nothing in either spec sheet justifies the premium unless you specifically want the 9005 platform.

**Monthly looks cheap until you multiply.** T1 TINY is $6.90/month, which annualizes to $82.80. The WEE is $36.90 for a year on the same 1 core / 1GB / 20GB chassis. You pay $45.90 more per year for TINY and get 2TB instead of 1TB plus a 10Gbps port rather than 100Mbps throttling. If 1TB covers you, the WEE is less than half the annual cost of the "cheaper" monthly plan.

Watch the cliff between plan tiers, too. Pro TINY at $88.88/year is a genuine bargain; Pro STARTER at $29.90/month is $358.80 annualized for 3TB and 2 vCPU. If you need more than 1TB, EB STARTER gives you 5,000GB at the same $29.90/month, which is the cheaper way to buy headroom. Annual pricing only appears on TINY and Pocket across the current sheet. Everything from STARTER up is monthly.

## Hong Kong and Tokyo: 20–50ms, small traffic buckets

Hong Kong Premium runs CN2 GIA direct to the mainland, and three separate sources put it at 20–50ms, with one review claiming under 50ms to major Chinese cities. That is a different category of experience from Los Angeles at 150–180ms.

You pay for it in traffic. HKG.AS3.Pro TINY at $21.90/month includes only **300GB**, and the $54.90 MINI tops out at 1,000GB. A site with any real image traffic will eat 300GB before the month is out. Hong Kong is for latency-critical, low-bandwidth work: an API endpoint, a game server, a control panel, remote desktop into something that has to feel local.

Tokyo sits between the two on latency and is the pick for Japanese or wider APAC audiences. Both Hong Kong and Tokyo also carry a T1 WEE at the same $36.90/year with 1TB, which is the cheapest way to get a presence in either city if you don't need the optimized route.

## What the plan tables don't tell you

**Linux only.** No Windows templates. Basic Linux literacy is assumed.

**Upgrades only, no downgrades.** You can move up a tier; moving down means buying a new service. Start lower than you think you need.

**Stock is the real constraint.** Popular plans sell out, and restocks clear quickly. The WEE exists in all three locations at the same price, so if Los Angeles is gone, check Hong Kong and Tokyo before giving up.

**IP changes are self-service.** Blocked IPs on Premium and Eyeball get a free replacement once every 15 days; other cases and all T1 swaps cost $5. Reviews note T1 IPs get blocked less often to begin with.

**Payment.** Alipay and PayPal are the two routes that come up consistently; credit card and crypto are also cited. One review warns that checking out through a proxy or VPN can trip fraud screening and trigger an automatic refund, so turn it off before you pay.

**Native IPs, no streaming promises.** Every plan ships a native IP, and unlock reports are common, but DMIT does not guarantee which services will work on any given day.

**Overselling.** DMIT states that it does not oversell nodes, and the long-term reviews repeat that without contradicting it. Support tickets are described as answered within 30 minutes by one write-up and within a few hours by another.

## Refund policy: what you actually get back

DMIT's own documentation is specific, and it is more generous than some older reviews claim.

- **Full refund:** within 3 days of purchase, provided you have used no more than 30GB of transfer. Payment-gateway fees are deducted.
- **Partial refund:** within 30 days, calculated on the remaining service time or remaining transfer, whichever yields less. DMIT also accepts refunds without requiring a reason.
- **Processing:** typically within 48 hours, slower at peak.
- **Where it goes:** account credit (no fee) or the original payment method (gateway fee deducted). Alipay returns the handling fee, so it effectively costs nothing.
- **Data:** the instance is deleted once the refund is confirmed. Back it up first.
- **What gets denied:** more than three refunds on the same product series, being the target of a DDoS, a blocked IP for personal reasons, a payment dispute, or claiming the network isn't good enough.

That $36.90 WEE with a 3-day full-refund window is about as cheap as a real trial gets. Use it to measure your own evening peak before committing to $88.88 or $358.80 a year.

👉 [Start with the $36.90 plan and test it for three days](https://www.dmit.io/aff.php?aff=9081)

## FAQ

**Is the $36.90 plan CN2 GIA?**
No. It is LAX.AN4.T1 WEE on the Tier 1 international route, with no mainland China optimization. The cheapest GIA plan is Pro TINY at $88.88/year.

**Can I run a proxy on T1?**
Only if you front it with your own relay. Direct connections fluctuate in the evening peak. If the proxy is latency-sensitive, budget for Eyeball or Premium.

**What happens when I exceed the traffic quota?**
The port is throttled and the server keeps running. 100Mbps in Los Angeles, 50Mbps on the Hong Kong and Tokyo WEE plans.

**Does it support Windows?**
No. Linux only.

**Will it unlock Netflix or other streaming?**
IPs are native and unlock reports are frequent, but availability changes and DMIT makes no written guarantee.

**What if the plan I want is out of stock?**
The T1 WEE is sold in all three locations at $36.90/year. If one is empty, try the other two, and check back after restocks.

## How to pick

Match the plan to the job, not to the price tag:

- **No China route needed, just a stable cheap box:** T1 WEE, $36.90/year, Los Angeles for the 100Mbps overage throttle.
- **China access, tight budget:** Eyeball AN4 TINY, $88.88/year, 1,500GB, best for mobile-heavy audiences.
- **China access, stable evenings:** Premium AN4 TINY, $88.88/year. Move to Pro STARTER at $29.90/month only when 1TB is genuinely tight.
- **Under 50ms to the mainland:** Hong Kong Pro from $21.90/month, and plan your traffic around that 300GB cap.
- **Japanese or APAC audience:** Tokyo, Pro if latency matters, T1 WEE if it doesn't.

Two things to confirm at checkout before you pay: that the plan is actually in stock in the location you picked, and the final total shown on the order page, since the tables above reflect listed rates and add-ons or payment fees can move the number.

👉 [Check live stock and current pricing on all DMIT plans](https://www.dmit.io/aff.php?aff=9081)
