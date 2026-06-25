Project: E-commerce User Journey & Purchase Attribution Analysis
1. Project Overview
Project Type: Independent User Behavior Analysis

Data Source: Public E-commerce User Behavior Logs

Time Period: November 25, 2017 – December 4, 2017 (10 days)

Data Volume: 987,370 behavior records from 9,739 users

Behavior Types: Page View (pv), Favorite (fav), Add-to-Cart (cart), Purchase (buy)

Tech Stack: Python (Pandas, Matplotlib, Seaborn)

2. Business Problem
The operations team wanted to know: What kind of upfront user behavior truly drives final purchases?

To answer this, I conducted a three-dimensional analysis:

User Behavior Paths: Compared conversion rates across four user groups based on their pre-purchase actions.

Temporal Dimension: Analyzed the distribution of behaviors across 24 hours to pinpoint high-conversion windows.

Product Category Dimension: Contrasted the top-ranked categories for views, favorites, cart-adds, and purchases to check for misalignment between interest and actual sales.

3. Key Findings
3.1 The Counter-Intuitive Conversion Path
I segmented users based on their complete set of behaviors before their first purchase. The results challenged a core business assumption.

Analysis Logic: Extracted each user's behavior path prior to their first buy and categorized them into four groups.

Result:

"Click-Only" users had the highest conversion rate at 77.55%.

"Click + Add-to-Cart" users converted at 65.28%.

"Click + Favorite" users converted at 60.03%.

Users with all three behaviors converted at 58.87%.

Insight: This overturned the conventional wisdom that "add-to-cart" is the strongest purchase signal. It revealed a large segment of "search-and-buy" users with rigid demand who bypass browsing and cart mechanics.

3.2 The "Night Owl" Conversion Window
Analysis Logic: Analyzed the hourly distribution of different behaviors and calculated the buy-to-view ratio for each hour.

Result: While traffic peaks occurred around noon and in the evening, the late-night hours of 0-2 AM showed a disproportionately high purchase-to-view ratio.

Insight: This suggests the existence of "quiet, late-night decision-makers" who are more likely to finalize a purchase with fewer distractions.

3.3 High User Stickiness
Result: The platform had a strong repurchase rate of 66.07%, indicating that users who made a first purchase were very likely to return and buy again. The overall bounce rate (users with only page views) was low at 6.00%.

4. Business Recommendations
Based on these insights, I proposed three actionable strategies:

Product - Streamline the Path: Ensure the "Buy Now" flow is as seamless as possible for "search-and-buy" users. Do not force them to go through an add-to-cart process.

Operations - Target the "Night Owls": Create a "Night Owl Zone" with limited-time flash deals between 0-2 AM to capitalize on this high-intent, low-distraction window.

Category Management - Differentiate Roles: Distinguish between categories. Use targeted coupons to convert users in high-interest, low-purchase categories, and increase exposure for high-conversion categories that lack traffic.

5. Limitations & Future Work
Data Period: The 10-day dataset is too short to rule out weekly patterns or special event effects.

Missing Fields: Lack of price/value data prevents a deeper analysis of user value segmentation and the "quality" of purchases.

Statistical Testing: Future work could apply chi-squared tests to validate the significance of the conversion rate differences between the identified user groups.
