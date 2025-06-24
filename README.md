# USA-Real-Estate-Market-Analysis-Insight

Uncovering insights from 2.2 M+ listings across states

Hi, I’m Tanvir, and in this project, I dove deep into the 2024 U.S. real estate market to uncover hidden patterns, regional pricing dynamics, and what really drives home values in different parts of the country.  

If you're a **homebuyer**, **investor**, or simply a **data enthusiast**—this analysis will give you a clearer picture of where value lies, which cities are booming, and how you can make more informed property decisions using data.

---

## Why I Did This Project

I’ve always been fascinated by real estate trends—how the same house can cost $200K in one city and $2M in another. So I asked myself:  
**What makes one home more valuable than another?**  
Is it the size? The number of beds? The location? Or something else?

To find the answers, I used Python, Pandas, Seaborn, and Matplotlib to clean, explore, and visualize thousands of property listings across the U.S.

---

## What You'll Learn from This Project

- Which states and cities are the most (and least) expensive to buy a home  
- Whether **bedrooms** or **bathrooms** affect pricing more (spoiler: it’s not what most people think!)  
- Which ZIP codes offer surprising value—and which are overpriced  
- How to measure home value using new engineered features like **price per sqft**, **acre per bedroom**, and more  

---

## Key Analyses (with Real Insights)

Here are the major analyses I performed and the stories the data told me:

### 1. Average Property Price by State  
Hawaii leads with an average price of ~$1.4M—no surprise given its paradise appeal. But the Virgin Islands, California, and New York aren’t far behind.  
<img width="395" alt="Image" src="https://github.com/user-attachments/assets/136170df-27bb-421b-9e96-cc7f787ee4ca" />

### 2. Top 10 Cities with Highest Median Prices  
Cities like **Rancho Santa Fe** ($4.97M) and **Malibu** ($3.97M) top the charts. These aren’t just cities—they’re luxury destinations.  
<img width="413" alt="Image" src="https://github.com/user-attachments/assets/c6bdfe46-92c1-45b6-a141-59496e1eb870" />

### 3. Home Size Distribution  
Most homes fall between 1,000–3,000 sqft, which seems to be the sweet spot for American living.  
<img width="412" alt="Image" src="https://github.com/user-attachments/assets/f3494627-5857-4040-94b5-a87e9ae345be" />

### 4. Beds vs. Price  
Yes, more bedrooms mean a higher price—but not always. The relationship is not perfectly linear.  
<img width="413" alt="Image" src="https://github.com/user-attachments/assets/139e540f-6509-4c43-839f-542c826d6b8b" />

### 5. Bathrooms vs. Price — The Real Influencer  
Here’s something interesting: **Bathrooms affect price more than bedrooms.**  
Even with the same number of beds, homes with more baths are consistently more expensive.  
*If you’re renovating, consider adding a bathroom over a bedroom!*

<img width="410" alt="Image" src="https://github.com/user-attachments/assets/5fb69b81-4990-4bdf-b698-04b61991b6cb" />

### 6. Acre Lot Size vs. Price  
Larger lots = higher price? Not always. This varies drastically by state.  
<img width="409" alt="Image" src="https://github.com/user-attachments/assets/5f48264a-f8bd-4a12-9860-13f118ee5cc1" />

### 7. Correlation Heatmap  
Strongest price correlations?  
- `house_size` → 0.61  
- `bath` → 0.61
<img width="405" alt="Image" src="https://github.com/user-attachments/assets/f5eb34c3-18f9-4ee5-9b2b-45feaeface19" />

Bedrooms? Much less important than I thought.

### 8. Most Common ZIP Codes  
By finding ZIPs with the most listings, I could identify real estate hot zones.  
<img width="406" alt="Image" src="https://github.com/user-attachments/assets/096101c1-5ee6-41d4-b305-7921a08e1cd5" />

### 9. State-wise Price Category Breakdown  
I divided listings into four tiers: **Low** **Affordable**, **Mid-range**, and **Luxury**.  
Hawaii unsurprisingly leads in luxury homes, but states like Florida and Texas offer tons of affordable properties.  
<img width="413" alt="Image" src="https://github.com/user-attachments/assets/d62fc519-8a30-4074-a065-2cfa246ecf14" />

### 10. Price Distribution by State  
California has a massive price range—million-dollar homes next to mid-range ones.  
<img width="401" alt="Image" src="https://github.com/user-attachments/assets/3cbd65ce-3766-4359-a21e-3c9a3e968025" />

### Luxury vs Non-Luxury Homes — Market Share
To better understand how many properties actually fall into the “Luxury” category, I created a new feature called is_luxury_home which flags homes priced over $1,000,000.
**After segmenting the data:**
- Only 9.5% of homes are luxury listings.
- The remaining 90.5% are non-luxury—meaning the market is largely mid-range or affordable.

<img width="408" alt="Image" src="https://github.com/user-attachments/assets/b0b72307-e2fc-4cef-9df8-4af1478d9446" />

**Why this matters:**
This finding is important for anyone working in real estate, especially marketers, sales agents, and investors.

-For **agents**, this indicates that most buyers are looking for affordable homes, not luxury mansions.
-For **investors**, the non-luxury market might offer quicker turnover and broader appeal.
-For **luxury sellers**, a more targeted and exclusive marketing strategy will be needed.

### Price per Sqft Distribution (Filtered)
To make home prices easier to compare across cities, I engineered a new metric: price_per_sqft.
But here's the thing—some ultra-luxury homes are priced far above $2,000 per square foot, which skews the distribution. So I filtered them out to reveal the real story.

**After filtering:**
-Most homes fall in the range of $100–$400 per sqft
-There’s a clear peak around this range, showing where the market truly lies.

<img width="408" alt="Image" src="https://github.com/user-attachments/assets/936667d5-f298-4a11-88ea-52b142ab6a09" />

**Why this matters:**
By cleaning out the extreme outliers, the chart became much easier to interpret and more useful for analysis.

**Now we can:**
-Set realistic benchmarks for buyers and sellers
-Identify affordable vs. premium zones across cities
-Focus marketing around the most active price range

---

## Feature Engineering: Making Raw Data Smarter

Sometimes raw data isn’t enough. I created new features to get deeper insights:

- **Price per Sqft** – A better way to compare value across cities  
- **Is_Luxury_Home** – A binary tag for homes priced above $1M  
- **Bedroom/Bathroom Ratio** – Tells us how balanced a home layout is  
- **Acre per Bedroom** – Helps evaluate land usage efficiency  
- **Luxury vs Non-Luxury Share** – Pie chart reveals market share: only 8.6% of listings are luxury homes  
- **Filtered Price per Sqft Distribution** – Removed extreme outliers to highlight the real pricing sweet spot ($100–$400/sqft)

---

## Bonus Visualization

### Average Price per Sqft in Top 10 Cities
This chart shows where every square foot really costs you—NYC, LA, and Miami lead the pack.
*Lollipop chart that visually pops*

<img width="413" alt="Image" src="https://github.com/user-attachments/assets/22a48a18-f656-411e-9844-fdc640c99d4d" />

---

## Real-World Takeaways

Here’s what this analysis taught me (and hopefully you too):

-  **Location** is still king in real estate  
-  **Bathrooms matter more than bedrooms** when it comes to price impact  
-  **ZIP codes reveal hidden gems**—some affordable, some overpriced  
-  **California dominates the luxury market**, but **Florida is full of value**

---

## Dataset Details

- Name: **USA Real Estate Dataset**  
- Source: [Kaggle Dataset]()  
- Shape of dataset: (2226382, 12)  
- Key columns: `price`, `bed`, `bath`, `acre_lot`, `house_size`, `city`, `state`, `zip_code`

---

## What’s Next?

This project was focused on exploration and storytelling.  
Next steps could include:

- Building **price prediction models (ML)**  
- Creating a **recommendation engine** for property hunters  
- Combining with external data like crime rates or school ratings

---

> **“Real estate is not just about land and buildings. It’s about people, patterns, and possibilities. And data helps us see that.”**

