# Anujan Sriskantharasa

Mobile engineer in Singapore. Nine years building Android and cross-platform apps —
currently at **SPH Media**, rebuilding *The Straits Times* app in Flutter.

Most of my working life has been spent on apps that already have users, where the
interesting constraint is replacing what's there without breaking it. I led a squad
through the ST180 Android revamp in Jetpack Compose, and now work on the ground-up
Flutter rebuild that collapses two native codebases into one.

Outside work I ship my own apps end to end — design, code, backends, store release.

---

### Things I've shipped on my own

**Lanka360** — *in store review*

An all-in-one Flutter app for Sri Lanka: weather, cricket, currency, news, public
holidays, government gazettes, emergency numbers, maps, everyday calculators and an
offline NIC decoder — in English, Sinhala and Tamil throughout.

Exam results were the interesting problem. The Department of Examinations publishes
an HTML form and no API, and its host isn't reachable from my edge network, so the
app renders the department's own page in a WebView: an index number goes straight
from the phone to the department and never passes through me.

Two services behind it — a Kotlin/Spring Boot API on Postgres, containerised and
deployed to Render, and a Cloudflare Worker that KV-caches the fast-moving feeds.

Flutter · Riverpod · GoRouter · Kotlin · Spring Boot · PostgreSQL · Docker · Cloudflare Workers

**RainCheck SG** · [App Store](https://apps.apple.com/sg/app/raincheck-sg/id6796591148) · [Play Store](https://play.google.com/store/apps/details?id=com.raincheck.raincheck_sg)

A Singapore route planner for people who'd rather not get rained on. It reads live
rainfall from data.gov.sg and plans a walk that favours sheltered ground — HDB
linkways, void decks, covered walkways — rather than the shortest line. Routes are
drawn stretch by stretch so you can see where you're covered and where you're not.

Flutter · Riverpod · flutter_map · OneMap · data.gov.sg · Firebase

**SG Lottery Results** · [App Store](https://apps.apple.com/sg/app/sg-lottery-results/id6795834679) · [Play Store](https://play.google.com/store/apps/details?id=com.sg_lottery_results)

Results, ticket checking and number analytics for Singapore's 4D, TOTO and Sweep
draws. The awkward part is timing — winning numbers land at draw time, but prize
tables and jackpot figures trickle in over the following hours — so a Cloudflare
Worker re-checks every fifteen minutes through the evening on draw days and keeps
the last good copy in KV.

Flutter · Riverpod · Cloudflare Workers · Workers KV · Hive · Firebase

*An independent results utility. Not affiliated with Singapore Pools; no betting,
no ticket sales.*

---

### What I work with

**Mobile** — Flutter, Dart, Kotlin, Jetpack Compose, Java, React Native  
**Architecture** — Clean Architecture, feature-first modules, MVVM, Riverpod, Coroutines  
**Testing** — unit, widget and golden tests  
**Backend & infra** — Kotlin/Spring Boot, PostgreSQL, Docker, Cloudflare Workers & KV, Firebase

### Also

Two published papers from 2018 — one on queuing optimisation, one on gait-based
Parkinsonian detection.

Singapore · [LinkedIn](https://www.linkedin.com/in/anujansri/)
