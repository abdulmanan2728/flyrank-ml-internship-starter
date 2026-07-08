# Capstone Project: Research Question Framing
**Lane Choice:** Search & Discoverability

## 1. The Core Question
How strongly does a page's average ranking position (`avg_position`) correlate with its actual click-through rate (`ctr`), and can we detect systematic drops in engagement before traffic completely falls off?

## 2. Unit of Analysis
The unit of analysis is an individual indexed URL (page) tracked over a 90-day window.

## 3. The Output
The model will output a probability score indicating whether a page is likely to experience a declining trend in search click-through performance.

## 4. The Action
A content marketing manager or SEO specialist will use this list to prioritize content refreshes, updates, or technical audits on pages that show signs of dropping engagement but still retain keyword visibility.

## 5. Cost of a Wrong Recommendation
* **False Positive (Type I Error):** Recommending an update for a healthy page. *Cost:* Wasted human hours rewriting content that didn't need fixing.
* **False Negative (Type II Error):** Missing a page that is actively declining. *Cost:* Lost search visibility and organic traffic to competitors, which directly impacts business revenue.

## 6. Why ML Helps (Instead of Simple Rules)
While basic rules can easily flag pages that have already crashed, they miss early, multi-variable signals. An ML approach can look at interactions between `avg_position`, `content_age_days`, and historical `ctr` to spot declining performance early, before the traffic loss becomes severe.
