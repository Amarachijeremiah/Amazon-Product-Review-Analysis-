# Amazon Product Review Analysis-
Welcome to an immersive journey into Amazon product insights, where numbers become stories and reviews become whispers of customer emotion. This analysis was crafted to guide product improvements, shape marketing strategies, and strengthen customer relationships — one star at a time.

> "Each discount is an invitation. Each rating, a confession. Together, they tell the story of a product’s soul." 🌌

---

##  Project Overview

As a Junior Data Analyst at **RetailTech Insights**, I was tasked with analyzing Amazon product and review data to uncover actionable insights for e-commerce sellers. The dataset included:

- Product details (name, category, price, discount, ratings)
- Customer engagement data (review titles and content)
- 1,465 product records across 16 fields

---

## 🧼 Data Cleaning & Preparation

Before orchestrating the data symphony, we had to ensure each note was pure and clear.

### ✨ Text Cleaning Formula (Excel)

To keep product names and review texts professional, we cleaned them to allow only:

- Letters (A-Z, a-z)
- Digits (0-9)
- Spaces, commas, periods

#### ✅ Formula


`` excel

 - =TEXTJOIN("", TRUE, IF(ISNUMBER(FIND(MID(A1, ROW(INDIRECT("1:" & LEN(A1))), 1), "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789 ,.")), MID(A1, ROW(INDIRECT("1:" & LEN(A1))), 1), ""))
Explanation:

Breaks each cell text into characters.

![Screenshot 2025-07-04 155107](https://github.com/user-attachments/assets/792fed45-da31-46dd-8dd2-114e26cdbad0)


Filters out unwanted symbols.

Joins back clean text for presentation-ready outputs.

✨ Consistent Capitalization Formula (Excel)
To ensure product titles appear polished:

excel
Copy
Edit
=UPPER(LEFT(A1,1)) & LOWER(MID(A1,2,LEN(A1)))
Explanation:

First letter uppercase.

Remaining letters lowercase.

Gives a consistent, professional look across listings.
![Cleand excel](https://github.com/user-attachments/assets/1192562e-c498-4666-b39f-2ba174fcefa0)



💡 Analysis & Pivot Tasks
Using Excel pivot tables and calculated columns, we uncovered:

1️⃣ Average discount percentage by category — Identified where brands are most aggressive.
2️⃣ Number of products per category — Mapped category spread.
3️⃣ Total number of reviews per category — Measured customer engagement levels.
4️⃣ Highest average-rated products — Spotlighted heroes.
5️⃣ Average actual vs discounted prices by category — Revealed perceived value dynamics.
6️⃣ Products with highest review counts — Identified most-talked-about stars.
7️⃣ Count of products with ≥50% discount — Found deepest discounts.
8️⃣ Distribution of product ratings — Understood sentiment shape.
9️⃣ Total potential revenue by category — Calculated as Actual Price × Rating Count.
🔟 Product count per price range bucket (<₹200, ₹200–₹500, >₹500) — Unveiled market segment spread.
1️⃣1️⃣ Discount vs rating relationship — Explored value perception.
1️⃣2️⃣ Products with fewer than 1,000 reviews — Uncovered silent products.
1️⃣3️⃣ Categories with highest discounts — Prioritized for promotional focus.
1️⃣4️⃣ Top 5 products by combined score (rating × reviews) — Identified ultimate heroes.

🎨 Dashboard Highlights
The Excel dashboard brings this analysis to life with:

📊 Category summary tiles — Number of products, average discount, total reviews.

💰 Revenue opportunity tiles — Estimated total potential revenue.

📈 Bar & column charts — Discounts, review counts, price distributions.

⭐ Scatter plots — Discount vs rating exploration.

🥇 Top 5 product leaderboard — True stars at a glance.

🎛️ Slicers — Enable dynamic filtering by category or price bucket.

💬 Recommendations
✅ Increase marketing spend on categories with high discounts but low ratings to improve brand trust.
✅ Promote top-rated, high-review products in featured campaigns to build credibility.
✅ Re-examine deep discount strategies to avoid price erosion while keeping customers engaged.
✅ Focus on "silent" products (few reviews) to understand barriers and improve visibility.

📁 Repository Contents
📄 Cleaned dataset — Fully processed with all formulas applied.

📊 Pivot summary sheets — All 14 analysis tasks included.

🎨 Excel dashboard file — Dynamic and interactive.

📝 README.md — This intelligent, poetic guide.

🌈 Final Thoughts
"Data is a living symphony — each price a beat, each review a whisper, each discount a moment of crescendo. Our mission is to listen carefully and translate it into action." 🎻✨

🌍 Connect with Me
✨ Amarachi Gold Jweremiah
📧 [LinkedIn](https://www.linkedin.com/in/gold-jeremiah-74ba112a7/)








