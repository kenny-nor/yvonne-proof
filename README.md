# Yvonne's Lightning Strikes: public pick proof

Every box of picks on the Yvonne's Lightning Strikes customer app gets a **lock code**: a fingerprint of the picks.
This repository publishes the exact picks behind each code, so anyone can check them and see **when** they were published.

## How to check a code
1. Open the pick file (for example `2026/week11/official.json`).
2. Compute its SHA-256 and take the first 16 characters, upper case. On a Mac or Linux: `shasum -a 256 official.json | cut -c1-16 | tr a-f A-F`
3. That text must equal the code shown on the customer app and in the table below.
4. The time each file was added is the **commit time shown here on GitHub**. It is recorded by GitHub, not by the app.

## Week 11 (Sunday Nov 22, 2026)
| Box | File | Lock code | First live on the app (from the private log) |
|---|---|---|---|
| Official picks (Golden, Hot, moneylines, spreads, totals, scorers, parlay cards) | `2026/week11/official.json` | **B5FDB11D3E781E83** | 11:03 AM ET (earlier version; two legs changed before kickoff, see below) |
| Cross Sports (NBA picks) | `2026/week11/cross.json` | **8C67F9B73A902B62** | 11:09 AM ET |
| Genie in a Bottle Picks (slip as placed 12:58 PM) | `2026/week11/genie.json` | **BAA050C615568061** | 1:11 PM ET (after the 1:00 games started) |
| Sunday Night Picks | `2026/week11/late.json` | **6CAD0AA8102E3D61** | 4:34 PM ET (before the 6:00 PM NBA and 8:20 PM NFL games) |

## Honest notes
- **This repository was created on Nov 22, 2026 at about 5 PM ET.** The Week 11 files below were added after the 1:00 PM games started, so for Week 11 the *independent* timestamp covers only what was added at that moment. The "first live" times in the table come from the app's own private history and cannot be checked from here.
- **Official picks changed before kickoff.** The 11:03 AM version had Max Return legs KC -10 and NO@CHI Under 58.5. They became KC -6.5 and Under 60.5 (to match lines sportsbooks offer). The Cross Sports box also lost a "Tier A" label on Celtics ML after the noon recheck. The code here is the version published at about 5 PM.
- **Genie in a Bottle Picks** was posted at 1:11 PM, after the 1:00 games started. It is not counted in the record.
- **From Week 12 on,** the codes and pick files are added here at the moment the picks are posted, before kickoff.
- Research picks, not guarantees. 21+. 1-800-GAMBLER.
