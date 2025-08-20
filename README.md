# ClickSphere - Website Performance Analysis

## Project Background

ClickSphere is a growing digital media and e-commerce platform that attracts users through multiple marketing channels, including organic search, paid ads, social media, and referral partners. As the company continues to scale, understanding how users interact with its website has become critical for optimizing both traffic acquisition and user engagement.The leadership team wants to know the surface-level metrics like pageviews and sessions to uncover actionable insights on user behavior, marketing channel effectiveness, and traffic quality. I am part of digital analyst tean, to do a website performance analysis using user, session, and engagement data.

Insights and recommendations are provided on the following key areas:

### 1. Sessions & Users Over Time
- Clear **daily cycle** with traffic peaks during working hours and dips at night.  
- **Sessions consistently exceed users**, meaning repeat visits within a day.  
- Noticeable spikes (e.g., mid and end of month) likely tied to **campaigns or promotions**.  
- Overall engagement is **steady with no major drop-offs**.  

### 2. Channel Contribution
- **Organic Social** dominates (~50k users), making it the top driver of traffic.  
- **Direct traffic** is strong (~30k), showing brand loyalty and recall.  
- **Organic Search** & **Referral** (~27k–28k) are consistent performers.  
- **Email** and **Organic Video** underperform with minimal contributions.  
- Small share of **Unassigned traffic**, likely due to **tracking gaps**.  

### 3. Engagement by Channel
- **Highest Engagement:** Organic Video (~180s), though inconsistent.  
- **Moderate Engagement:** Referral (~95s, consistent), Unassigned (~80s, variable).  
- **Lowest Engagement:** Direct (~45s), Organic Social (~52s), Organic Search (~47s).  
- **Email:** Unstable engagement (~72s) with high variability across campaigns.  

### 4. Engagement Rates
- **Referral & Organic Search** → Strongest, with consistent median engagement.  
- **Organic Social** → Promising, but variable.  
- **Direct Traffic** → Moderate, steady but limited growth potential.  
- **Email** → Extremely variable (0–1.0), depending on campaign quality.  
- **Unassigned & Organic Video** → Weak engagement overall.  

### 5. Engaged vs Non-Engaged Sessions
- **Organic Social, Referral, and Organic Search** drive **more engaged than non-engaged sessions** → high-quality audiences.  
- **Direct Traffic** → Slightly more non-engaged sessions → weaker intent.  
- **Email & Organic Video** → Minimal impact.  
- **Unassigned** → Very small, but points to tracking issues.  

### 6. Hourly Traffic Trends
- **Organic Social** peaks between **10:00–20:00**, maxing at **19:00 (~3.5k visits)**.  
- **Direct Traffic** is steady, with late evening spikes (**23:00 ~2.5k visits**).  
- **Email** → Almost negligible, except minor traffic at **2:00 and 19:00**.  
- **Organic Search** → Strong in midday (**10:00–18:00**) with peaks at **15:00 & 19:00**.  
- **Referral** → Consistent contributor with peaks at **11:00 & 21:00**.  
- **Unassigned** → Small, peaking at **15:00 & 19:00 (~38 visits)**.  

### 7. Engagement Rate vs Sessions Over Time
- Sessions show **strong cyclical fluctuations**, often peaking **100+**.  
- Engagement rate remains **flat and low**, indicating weak interaction depth.  
- High traffic does not translate into proportional engagement → focus should shift from **volume to quality engagement**.
  

Notebook containing data inspection, cleaning & analysis with python can be found here [link](https://colab.research.google.com/drive/15qqYiF3vXpXnwX-y_xhH7GDZYAUdu6Km?usp=drive_link)


## Data Structure & Initial Checks

![Website Performance]("Screenshot (12).png")






## Insights from Sessions & Users Over Time

- **Consistent Daily Pattern**  
  Both sessions and users follow a clear **daily cycle** with peaks during specific hours (likely working hours) and dips late at night.  

- **Sessions Exceed Users**  
  Sessions consistently outnumber users, indicating that many users return multiple times within the same day.  

- **Traffic Fluctuations**  
  Noticeable spikes (e.g., around the 18th and 30th) suggest **campaigns, promotions, or external factors** driving extra activity.  

- **Steady Growth**  
  Overall, both sessions and users show relatively **stable engagement across the month**, without drastic drop-offs.  

## Recommendations

- **Leverage Peak Hours**  
  Focus marketing campaigns, product launches, or email pushes during high-traffic hours to maximize visibility.  

- **Boost Engagement During Lows**  
  Introduce retention tactics (notifications, discounts, or new content) to encourage activity during off-peak hours.  

- **Investigate Spikes**  
  Analyze what caused the traffic surges (18th, 30th). If tied to campaigns, replicate strategies for future growth.  

- **Optimize Returning User Experience**  
  Since sessions > users, enhance features for repeat visitors (personalization, loyalty programs) to sustain engagement.


## 📊 Insights & Recommendations

### 🔍 Insights
- **Organic Social** is the leading channel, driving nearly **50,000 users**, making it the top source of traffic.
- **Direct traffic** is the second-largest contributor, with around **30,000 users**, indicating strong brand recall and customer loyalty.
- **Organic Search** and **Referral** channels are almost at the same level (~27k–28k users), showing consistent performance but with room for growth.
- **Email** and **Organic Video** are underperforming, contributing very little to overall users.
- **Unassigned traffic** exists, though minimal, which could indicate **tracking issues**.

### ✅ Recommendations
- **Double down on Organic Social**: Invest more in high-performing platforms, content, and campaigns that are driving this large share of traffic.  
- **Strengthen Direct & Referral channels**: Enhance customer retention programs and partnerships that encourage repeat visits and referral traffic.  
- **Optimize SEO strategy**: Target high-intent keywords and optimize existing content to push **Organic Search** beyond its current plateau.  
- **Revamp Email & Video campaigns**: Experiment with **personalized email campaigns** and **short-form video content** to capture more users.  
- **Fix tracking gaps**: Address the **Unassigned channel** by improving analytics implementation to ensure all traffic is attributed correctly.  

# 📊 Channel Engagement Analysis

## 🔍 Insights
- **Highest Engagement – Organic Video**
  - Drives the **longest average engagement (~180s)**, far exceeding other channels.
  - Shows **large variability (wide error bars)** → performance is inconsistent.

- **Moderate Engagement – Referral & Unassigned**
  - Referral traffic has **steady engagement (~95s)** with low variability → consistent quality.
  - Unassigned traffic performs moderately (~80s) but with higher variation.

- **Low Engagement – Direct, Organic Social, Organic Search**
  - Direct (~45s), Organic Social (~52s), and Organic Search (~47s) show the **lowest engagement**.
  - Stable but short sessions.

- **Email Engagement – Unstable**
  - Average engagement (~72s) but with **very high variability** → campaign quality strongly impacts outcomes.

---

## ✅ Recommendations
- **Leverage Organic Video**
  - Invest in **video content strategy** (educational, storytelling).
  - Standardize best-performing formats to reduce inconsistency.

- **Optimize Referral Partnerships**
  - Strengthen and expand referrals since they **consistently drive quality engagement**.
  - Identify best referral sources and scale them.

- **Improve Direct, Social & Search**
  - Enhance **landing page experience** and content targeting for better depth.
  - Experiment with **personalization** to increase engagement.

- **Stabilize Email Campaigns**
  - Use **A/B testing** (subject lines, audience segmentation).
  - Focus on **value-driven content** (exclusive offers, insights).

- **Cross-Channel Strategy**
  - Integrate **video into email & social campaigns** to lift performance.
  - Apply **referral learnings** to improve targeting in other channels.


# 📊 Engagement Rate Analysis by Channels

## 🔎 Insights
1. **Referral & Organic Search Perform Best**  
   - Median engagement rate is higher for **Referral** and **Organic Search** channels compared to others.  
   - These channels also show a tighter spread, indicating **consistent engagement**.

2. **Organic Social is Promising**  
   - Engagement is relatively strong, with a median above 0.5.  
   - However, it shows higher variability, meaning engagement is not always predictable.

3. **Direct Traffic is Moderate**  
   - Engagement rate is steady but slightly lower than Organic Social and Search.  
   - Indicates that while **direct visitors engage**, the potential to scale is limited.

4. **Email Shows Extreme Variation**  
   - Engagement ranges from near **0 to 1.0**, highlighting **inconsistent performance**.  
   - Some campaigns perform very well, while others fail to engage.

5. **Unassigned & Organic Video Underperform**  
   - Both show **very low engagement rates**.  
   - Either due to poor tracking (unassigned) or lack of effective video strategy.

---

## ✅ Recommendations
1. **Double Down on Referral & Organic Search**  
   - Invest more in **SEO strategies** and **partnership-driven referral programs**.  
   - Focus on keyword optimization and content partnerships.

2. **Stabilize Organic Social Engagement**  
   - Analyze high-performing posts to identify **content patter**


# 📊 Insights & Recommendations

## 🔍 Insights
1. **Organic Social**
   - Highest number of sessions overall.  
   - Engaged sessions are significantly higher than non-engaged, showing strong user interest and interaction.  

2. **Referral**
   - Shows a notable difference with much higher engaged sessions compared to non-engaged.  
   - Indicates referral traffic is highly valuable and drives quality users.  

3. **Organic Search**
   - More engaged than non-engaged, suggesting effective SEO efforts are attracting relevant audiences.  

4. **Direct Traffic**
   - Non-engaged sessions slightly outweigh engaged sessions.  
   - Suggests users directly accessing may lack intent or find less value compared to other channels.  

5. **Email & Organic Video**
   - Very low or negligible engagement, signaling underutilization or weak performance.  

6. **Unassigned Traffic**
   - Minimal volume, but may indicate tracking or tagging issues.  

---

## ✅ Recommendations
1. **Double Down on Organic Social & Referral**  
   - Invest more in social campaigns and referral partnerships, as these channels show high engagement.  
   - Consider boosting budget allocation, influencer collaborations, and community-building.  

2. **Optimize Direct Traffic**  
   - Improve landing page experiences and calls-to-action (CTAs) for direct visitors.  
   - Segment direct traffic sources (e.g., bookmarks, offline campaigns, untagged links) to understand behavior better.  

3. **Strengthen SEO Strategy**  
   - Since organic search is already performing well, focus on long-tail keywords and content marketing.  
   - Monitor bounce rates and refine high-traffic but low-engagement keywords.  

4. **Revisit Email & Video Strategy**  
   - For **email**: personalize subject lines, improve segmentation, and enhance CTA clarity.  
   - For **video**: optimize titles/thumbnails, cross-promote on social, and embed in high-traffic pages.  

5. **Fix Tracking for “Unassigned”**  
   - Review UTM parameters and analytics setup to reduce unassigned traffic.  
   - Ensure proper tagging in campaigns for accurate attribution.  



# 📊 Insights & Recommendations: Traffic by Hours & Channel

## 🔎 Key Insights
1. **Organic Social dominates**  
   - Highest traffic volumes are consistently observed through *Organic Social*, peaking between **10:00–20:00 hours**.
   - Peak traffic occurs at **19:00 (3469 visits)** and **20:00 (3206 visits)**.

2. **Direct traffic remains steady**  
   - Direct channel traffic is consistently high across all hours, with noticeable spikes in the **late evening (23:00 with 2581 visits)**.

3. **Email channel underperforms**  
   - Email contributes almost **zero traffic** throughout the day, except for **small activity at 2:00, 19:00**.

4. **Organic Search shows midday strength**  
   - Organic Search performs well in **10:00–18:00 hours**, peaking at **15:00 (1898 visits)** and **19:00 (1887 visits)**.

5. **Referral traffic is moderate**  
   - Traffic from referrals peaks at **11:00 (1790)** and **21:00 (1799)**.
   - Consistently contributes in the range of **500–1700 visits**.

6. **Unassigned traffic is small but present**  
   - Peaks at **15:00 (38)** and **19:00 (38)**.
   - Represents minor traffic, possibly from untracked campaigns.

---

## 💡 Recommendations
1. **Capitalize on Organic Social peak hours**  
   - Schedule high-priority content, ads, or promotions between **18:00–21:00** when Organic Social is at its strongest.
   - Experiment with reels, live sessions, or trending formats to maximize reach.

2. **Re-engage Email as a channel**  
   - Current engagement is minimal; optimize subject lines, personalization, and send times.
   - Test campaigns around **early morning (8–10 AM)** or **evening (19–21 PM)** where other channels peak.

3. **Optimize Direct & Organic Search overlap**  
   - Direct & Search both show strong traffic in evenings; ensure **landing pages and CTAs** are optimized for conversions.
   - Implement A/B testing on **checkout flows** during high-traffic windows.

4. **Strengthen Referral partnerships**  
   - Since Referral traffic peaks at **11:00 & 21:00**, collaborate with affiliates/blogs to push promotions during these hours.

5. **Investigate Unassigned traffic**  
   - Likely due to **poor tracking or missing UTM parameters**.
   - Improve analytics tagging to correctly classify and measure performance.

6. **Cross-channel strategy**  
   - Drive synergy: push Email reminders when Organic Social traffic spikes, or retarget Referral users via Social Ads.

---

✅ **Action Plan:** Focus on **Organic Social & Direct** for growth, optimize **Email campaigns**, and improve **attribution tracking** for better decision-making.



# 📊 Engagement Rate vs Sessions Over Time

## 🔍 Insights
1. **High Session Fluctuations**  
   - The number of sessions shows a strong cyclical pattern with noticeable daily spikes and drops.  
   - Peaks cross **100+ sessions** frequently, while dips go down to **20–30 sessions**.  

2. **Low Engagement Rate Stability**  
   - Engagement rate remains **consistently flat** at a very low level compared to the sessions trend.  
   - This suggests that while traffic volume is high, user engagement is not increasing proportionally.  

3. **Mismatch Between Traffic & Engagement**  
   - Despite session spikes, engagement rate does not scale up.  
   - This indicates that **users visit but do not interact deeply** with the platform.  

---

## ✅ Recommendations
1. **Improve Content Quality & Relevance**  
   - Optimize landing pages to ensure visitors find value immediately.  
   - Introduce personalized recommendations, better UX, and interactive elements.  

2. **Targeted Retention Strategies**  
   - Use email campaigns, push notifications, or loyalty rewards to encourage repeat engagement.  
   - Run A/B tests on key pages to identify what drives higher interaction.  

3. **Analyze Drop-off Points**  
   - Track user journeys to identify where engagement fails (bounce rates, session duration).  
   - Fix bottlenecks such as poor navigation, irrelevant content, or slow load times.  

4. **Quality Traffic Acquisition**  
   - Focus on bringing **high-intent users** via targeted marketing instead of only increasing session count.  
   - Invest in channels that bring engaged users rather than volume-driven traffic.  

---

## 📌 Conclusion
- **Sessions are healthy and consistent, but engagement is lacking.**  
- Efforts should shift from **acquiring traffic** to **converting and retaining engaged users**.




  
