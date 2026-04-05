# Meta-Ad-Performance-Dashboard
This is a **Meta Ad Performance Dashboard** built in Power BI that tracks the effectiveness  of ad campaigns across Facebook and Instagram. It provides a complete funnel view —  from awareness to engagement to purchases — along with demographic, geographic,  and time-based insights.


# 📊 Meta Ad Performance Dashboard (Facebook & Instagram)

![Meta Ad Performance Dashboard](Meta_dashboard.png)

---

## 🗂️ Data Model

![Data Model](Data_Modelling.png)

---

## 📌 Project Overview

This is a **Meta Ad Performance Dashboard** built in Power BI that tracks the effectiveness 
of ad campaigns across Facebook and Instagram. It provides a complete funnel view — 
from awareness to engagement to purchases — along with demographic, geographic, 
and time-based insights.

---

## 🎯 Business Objective

The marketing team needed a performance tracking report for ad campaigns running on 
**Facebook and Instagram** to:
- Identify the most effective platform (Facebook vs Instagram)
- Track campaign ROI and optimize budget allocation
- Understand audience engagement patterns

**Scope:** Only paid ads on Facebook & Instagram (Messenger and Audience Network excluded)

---

## 📐 Data Model Tables

| Table | Description |
|-------|-------------|
| `ad_events` | Contains event-level data — impressions, clicks, shares, comments, purchases |
| `ads` | Ad-level info — ad type, platform, campaign_id, target age/gender/interests |
| `campaigns` | Campaign details — name, budget, start/end date, duration |
| `users` | User demographics — age, gender, country, interests, location |
| `Calender Table` | Date table for time intelligence — Date, Day, Week, Month |
| `Dynamic measure` | Parameter table for dynamic KPI switching on visuals |

---

## 📊 KPIs & Definitions

| KPI | Definition | Formula |
|-----|-----------|---------|
| Impressions | Times ads were displayed | COUNT(event_type = Impression) |
| Clicks | Times users clicked ads | COUNT(event_type = Click) |
| Shares | Times ads were shared | COUNT(event_type = Share) |
| Comments | User comments on ads | COUNT(event_type = Comment) |
| Purchases | Purchases made after seeing ads | COUNT(event_type = Purchase) |
| Engagements | Total interactions | Clicks + Shares + Comments |
| CTR | % impressions that led to clicks | (Clicks ÷ Impressions) × 100 |
| Engagement Rate | % impressions that led to engagements | (Engagements ÷ Impressions) × 100 |
| Conversion Rate | % clicks that led to purchases | (Purchases ÷ Clicks) × 100 |
| Purchase Rate | % impressions that led to purchases | (Purchases ÷ Impressions) × 100 |
| Total Budget | Total ad spend | SUM(campaigns.total_budget) |
| Avg Budget/Campaign | Average budget per campaign | Total Budget ÷ Campaign Count |

---

## 📈 Dashboard KPI Summary

| Metric | Value |
|--------|-------|
| Total Impressions | 339.8K |
| Total Clicks | 40.1K |
| Total Shares | 2.0K |
| Total Comments | 4.1K |
| Total Purchases | 2.0K |
| Total Engagements | 46.1K |
| Total Campaigns | 50 |
| CPC | $63.27 |
| CTR | 11.79% |
| Engagement Rate | 13.58% |
| Conversion Rate | 5.07% |
| Purchase Rate | 0.60% |
| Total Budget | $2.54M |
| Avg Budget/Campaign | $50.72K |
| Total Users | 9.841K |
| Total Ads | 200 |

---

## 💡 Dashboard Insights

### 🔺 Funnel Analysis
- **High CTR (11.79%) and Engagement Rate (13.58%)** → Ad creatives and targeting 
at the top of the funnel are very effective
- **Low Purchase Rate (0.60%)** → Sharp drop-off in the lower funnel. Classic case of 
strong awareness but weak action/purchase
- **Key Takeaway:** Optimize landing pages, retargeting strategies, and offers to 
capture users who engage but don't purchase

### 👥 Audience Breakdown
- **By Gender:** Females (41.05%) engage more than Males (23.5%)
- **By Age:** Peak engagement in the **18–30 age group**, drops significantly after 35+
- **Core Audience = Young Females aged 18–30**

### 🌍 Geographic Insights
- **High Volume Markets:** India & Brazil (high engagement, high reach)
- **High Value Markets:** Germany & UK (stronger purchasing power, better conversion potential)
- **Strategy:** Volume campaigns for India/Brazil, premium campaigns for Germany/UK

### ⏰ Time-Based Trends
- **Best Time to Run Ads:** Afternoons & Evenings (peaks around 15:00–20:00 hrs)
- **Worst Time:** Early morning (0–5 hrs) — lowest engagement
- **Calendar Spikes:** Dates 19th–21st and 25th–27th show higher engagement — 
likely linked to promotions or campaign launches
- **Insight:** Event-based campaigns drive significantly higher performance

### 📢 Ad Type Performance

| Ad Type | Impressions | Clicks | CTR | Purchase Rate | Conversion Rate | Engagement Rate |
|---------|------------|--------|-----|---------------|-----------------|-----------------|
| Video | 46K | 5K | 11.9% | 0.62% | 5.2% | 13.7% |
| Stories | 72K | 8K | 11.8% | 0.65% | 5.2% | 13.6% |
| Image | 51K | 6K | 11.7% | 0.57% | 4.9% | 13.5% |
| Carousel | 48K | 6K | 11.7% | 0.59% | 5.1% | 13.4% |

- **Best Formats:** Video > Stories > Carousel > Image
- **Recommendation:** Shift budget towards Video & Stories for better ROI

---

## 📋 Charts in the Dashboard

1. **Donut Chart** — Total Engagement by Target Gender (dynamic metric)
2. **Bar Chart** — Total Engagement by Age Group (dynamic metric)
3. **Area Chart** — Engagement Rate by Time of Day
4. **Line Chart** — Engagement Rate by Day of Week
5. **Map** — Total Engagement by Country
6. **Calendar Heat Map** — Weekly engagement mapped by date
7. **Stacked Column** — Weekly trend by Ad Type
8. **Matrix Table** — Ad Type vs. CTR, Purchase, Impressions, Engagement Rate

---

## ✅ Final Recommendations

1. **Strong awareness & engagement but low purchase efficiency** → Optimize landing 
pages, retargeting, and offers
2. **Target audience** = Females, 18–30, in India & Brazil → Refine campaigns accordingly
3. **Best ad formats** = Video & Stories → Increase budget allocation here
4. **Best times** = Afternoons & Evenings → Schedule ads in these slots
5. **Geography** = Volume from India/Brazil, Value from Germany/UK → Segment strategies
6. **Action** = Improve landing pages, offers, and retargeting campaigns to lift purchase rate

---

## 🛠️ Tools Used

- **Power BI** — Dashboard & Data Modelling
- **DAX** — KPI calculations and dynamic measures
- **Power Query** — Data transformation
- **Data Source** — Simulated Meta Ads dataset (Facebook & Instagram)

---

## 👤 Author

**Swapnjeet S** — Lead Data Analyst (10.5 years experience)  
🌐 [Website](https://topmate.io/data_tutorials) | 
📺 [YouTube](http://www.youtube.com/@datatutorials1)
