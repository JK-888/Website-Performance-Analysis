# ClickSphere - Website Performance Analysis

# Project Background

ClickSphere is a growing digital media and e-commerce platform that attracts users through multiple marketing channels, including organic search, paid ads, social media, and referral partners. As the company continues to scale, understanding how users interact with its website has become critical for optimizing both traffic acquisition and user engagement.The leadership team wants to know the surface-level metrics like pageviews and sessions to uncover actionable insights on user behavior, marketing channel effectiveness, and traffic quality. I am part of digital analyst tean, to do a website performance analysis using user, session, and engagement data.

Insights and recommendations are provided on the following key areas:

#### 1. Sessions & Users Over Time
#### 2. Channel Contribution
#### 3. Engagement by Channel
#### 4. Engagement Rates
#### 5. Engaged vs Non-Engaged Sessions
#### 6. Hourly Traffic Trends
#### 7. Engagement Rate vs Sessions Over Time

Notebook containing data inspection, cleaning & analysis with python can be found here [link](https://colab.research.google.com/drive/15qqYiF3vXpXnwX-y_xhH7GDZYAUdu6Km?usp=drive_link)


# Data Structure & Initial Checks

The table consists of 10 columns:

- Column 1: Channel Group
- Column 2: DateHour
- Column 3: Users
- Column 4: Sessions
- Column 5: Engaged Sessions
- Column 6: Average engagemnet time per session
- Column 7: Engaged session per user
- Column 8: Events per session
- Column 9: Engagement rate
- Column 10: Event Count



<img width="1764" height="603" alt="Screenshot (12)" src="https://github.com/user-attachments/assets/34bffaf5-3f1a-4a5b-a962-f60c0b9e21ec" />


# Executive Summary

## Overview of findings – User Traffic & Engagement Analysis


- **Strong Traffic Volume**  
  - Total sessions show **consistent daily cycles**, peaking above **100+ sessions/day**.  
  - **Sessions consistently exceed users**, confirming repeat visits within the same day.  

- **Top Traffic Channels**  
  - **Organic Social** dominates with ~**50k users**, highest sessions, and strong engagement.  
  - **Direct traffic** follows (~**30k users**), indicating strong brand recall but lower engagement intent.  
  - **Organic Search & Referral** contribute ~**27k–28k users each**, with **Referral driving higher-quality, engaged sessions**.  

- **Engagement Patterns**  
  - **Organic Video** shows the **highest average engagement (~180s)** but is inconsistent.  
  - **Referral traffic** delivers **steady engagement (~95s)** with low variability → high-quality source.  
  - **Direct, Organic Social, and Organic Search** have **short but stable sessions (~45–52s)**.  
  - **Email campaigns** are inconsistent, ranging from **very high to near-zero engagement**.  

- **Traffic by Time of Day**  
  - **Organic Social peaks (19:00, ~3.5k visits)**, sustaining strong activity between **10:00–20:00**.  
  - **Direct traffic** is steady, peaking late evening (**23:00, ~2.6k visits**).  
  - **Referral traffic** peaks around **11:00 (1.8k)** and **21:00 (1.8k)**.  
  - **Email & Organic Video** remain minimal contributors.  

- **Engagement Rate vs Sessions**  
  - Despite **traffic spikes**, engagement rate remains **flat and very low**, showing users visit but do not interact deeply.

 

# Insights Deep Dive




<img width="860" height="513" alt="1" src="https://github.com/user-attachments/assets/f793c761-b116-4dcf-a3a0-02d6e3fdecce" />


- **Consistent Daily Pattern**  
  Both sessions and users follow a clear **daily cycle** with peaks during specific hours (likely working hours) and dips late at night.  

- **Sessions Exceed Users**  
  Sessions consistently outnumber users, indicating that many users return multiple times within the same day.  

- **Traffic Fluctuations**  
  Noticeable spikes (e.g., around the 18th and 30th) suggest **campaigns, promotions, or external factors** driving extra activity.  

- **Steady Growth**  
  Overall, both sessions and users show relatively **stable engagement across the month**, without drastic drop-offs.  




<img width="725" height="557" alt="2" src="https://github.com/user-attachments/assets/327c43a1-52b0-4d2c-8394-3f0ac848285a" />


- **Organic Social** is the leading channel, driving nearly **50,000 users**, making it the top source of traffic.
- **Direct traffic** is the second-largest contributor, with around **30,000 users**, indicating strong brand recall and customer loyalty.
- **Organic Search** and **Referral** channels are almost at the same level (~27k–28k users), showing consistent performance but with room for growth.
- **Email** and **Organic Video** are underperforming, contributing very little to overall users.
- **Unassigned traffic** exists, though minimal, which could indicate **tracking issues**.



 


<img width="705" height="557" alt="3" src="https://github.com/user-attachments/assets/5a99f103-54d4-4031-8d8a-49b81cff1a99" />


 **Highest Engagement – Organic Video**
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
  - 



  
  
<img width="701" height="557" alt="4" src="https://github.com/user-attachments/assets/455ef1b4-0ddb-4a4d-ab4a-75d57aa58bff" />



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
  


<img width="725" height="557" alt="5" src="https://github.com/user-attachments/assets/7c2fe63f-cf92-45a7-b534-1c93c31aa00a" />




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
  







<img width="941" height="658" alt="6" src="https://github.com/user-attachments/assets/970b1521-ff1a-4c08-a0e4-e37c4cff4d45" />






1. **Top Traffic Channels**
- **Organic Social** dominates traffic across all hours, especially during **midday (10 AM – 4 PM)** and again around **8–10 PM**, peaking **above 3,500**.  
- **Direct** and **Organic Search** consistently contribute **medium-to-high traffic**, with peaks in the **evening (7 PM – 11 PM)**.  
- **Email** is almost negligible (**close to zero all day**).  
- **Organic Video** shows **modest traffic**, performing slightly better in **evenings**.  
- **Referral** maintains **stable but low traffic** throughout the day.  


2. **Hourly Patterns**
- **Morning (6 AM – 9 AM):** Moderate traffic across **Direct, Organic Search, and Social**.  
- **Midday (10 AM – 4 PM):** **Highest traffic** for **Organic Social** and strong performance in **Organic Search**.  
- **Evening (7 PM – 11 PM):** **Second-highest traffic window** across almost all channels, suggesting strong user engagement **post-work hours**.  
- **Late Night (12 AM – 5 AM):** **Sharp traffic drop** across all channels.  


3. **Unassigned Traffic**
- Small but steady contribution across hours (**10–38**), suggesting **tracking or attribution gaps**.  

  



  
   
<img width="895" height="479" alt="7" src="https://github.com/user-attachments/assets/f013d71e-f75d-4c34-a677-3836fd074c9f" />



1. **High Session Fluctuations**  
   - The number of sessions shows a strong cyclical pattern with noticeable daily spikes and drops.  
   - Peaks cross **100+ sessions** frequently, while dips go down to **20–30 sessions**.  

2. **Low Engagement Rate Stability**  
   - Engagement rate remains **consistently flat** at a very low level compared to the sessions trend.  
   - This suggests that while traffic volume is high, user engagement is not increasing proportionally.  

3. **Mismatch Between Traffic & Engagement**  
   - Despite session spikes, engagement rate does not scale up.  
   - This indicates that **users visit but do not interact deeply** with the platform.
  


# Recommendations 


### 1. Align Marketing With Peak Session Hours  
- User sessions consistently spike above 80–100 during certain hours, but engagement rates remain flat.  
- **Recommendation:** Concentrate ad spend, push notifications, and campaign launches during these high-traffic windows.  
- **Why:** Ensures maximum ROI by capturing audiences when they are most active.  


### 2. Focus on Engagement Quality Over Traffic Volume  
- Engagement rate remains nearly zero despite large session fluctuations.  
- **Recommendation:** Redesign landing pages, improve CTAs, and personalize user experiences to make sessions meaningful.  
- **Why:** Converting traffic into engaged users will have greater long-term business impact than raw session counts.  



### 3. Reduce Drop-Off During Session Surges  
- Even with session surges above 100, engagement does not scale up.  
- **Recommendation:** Introduce retention features like in-session surveys, gamified elements, or chatbots.  
- **Why:** Keeps users from bouncing and increases interaction before session exit.  



### 4. Test & Iterate on Content and Features  
- Flat engagement line signals low influence from current features or content.  
- **Recommendation:** Run A/B tests with interactive formats such as videos, quizzes, or micro-conversions.  
- **Why:** Helps identify what resonates with users and drives higher engagement rates.  


### 5. Segment Engagement by Channel Group  
- Sessions are high across all channels, but engagement rates stay low across the board.  
- **Recommendation:** Break down performance by channel (organic, paid, referral, direct) and tailor engagement tactics for each.  
  - **Organic:** Stronger CTAs and optimized landing pages  
  - **Paid:** Retargeting campaigns to re-engage non-converters  
  - **Referral:** Loyalty programs or referral rewards  
- **Why:** Channel-specific strategies prevent wasted effort and maximize ROI.  








