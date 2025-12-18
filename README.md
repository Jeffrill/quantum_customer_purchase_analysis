# Customer Purchase Behavior Analysis
## **Project Overview**
 Python-driven analysis of retail transaction and customer data to identify purchasing patterns, high-value customer segments, and key revenue drivers.
 Analyzed 264,836 transactions from 72,637 unique customers to understand purchasing patterns across life stages and customer types. This project demonstrates a complete analytics workflow: from data quality assessment through customer segmentation to actionable business recommendations.


## Business Objective

Answer three critical questions:
1. Which customer segments generate the most revenue?
2. What purchasing patterns distinguish high-value from low-value customers?
3. Where are the biggest opportunities for revenue growth?

## Key Findings

**1. Older Demographics Drive Revenue**
- Older singles/couples: Highest revenue segment
- Retirees: Second-highest revenue generator
- Older families: Third in revenue contribution
- Young families and young singles significantly underperform despite larger populations

**2. Mainstream Customers Outperform Premium (Counterintuitive)**
- Mainstream segment: Highest total revenue from 29,245 customers
- Budget segment: Second in revenue from 24,470 customers
- Premium segment: Lowest revenue from 18,922 customers
- **Key Insight:** Volume of moderate spenders generates more revenue than fewer "premium" customers

**3. Purchase Frequency Varies by Segment**
- High-value segments show distinct purchasing patterns
- Frequency analysis reveals opportunities for targeted retention campaigns

**4. Product Preferences**
- Top 10 products identified account for significant portion of sales
- Product preferences show variation across customer life stages

## Skills Demonstrated

✓ **Data Cleaning & Integration**: Merged transaction and customer tables, standardized inconsistent categories  
✓ **Customer Segmentation**: Analyzed behavior across life stages and customer types  
✓ **Statistical Analysis**: Revenue distribution, outlier detection, comparative metrics  
✓ **Python Proficiency**: pandas (data manipulation), matplotlib/seaborn (visualization)  
✓ **Business Translation**: Converted analytical findings into specific, actionable recommendations  


## Tools & Technologies

- **Python**: pandas, NumPy, matplotlib, seaborn
- **Jupyter Notebook**: Interactive analysis and documentation
- **Data Visualization**: Custom charts showing segment performance and trends

## **Dataset**
Retail transaction and customer dataset containing:
- 264,836 transactions
- Approximately 72,637 unique customers
- Customer life stage classifications( Budget, Mainstream, Premium)
- Transaction history covering 2018-07-01 to 2019-06-30

## Project Structure
```
customer-purchase-analysis/
├── customer_analysis.ipynb      # Complete analysis with code and insights
├── visualizations/               # 6 key charts showing findings
│   ├── revenue_by_lifestage.png
│   ├── customer_type_comparison.png
│   ├── purchase_frequency.png
│   ├── top_products.png
│   ├── monthly_trends.png
│   └── segment_behavior.png
├── data/
│   └── data_description.txt     # Dataset overview (data not included)
└── README.md                    # This file
```

## Analysis Workflow

### 1. Data Quality Assessment
- Checked for missing values in transaction and customer behavior tables
- Identified and fixed product name inconsistencies (spacing, spelling errors)
- Validated transaction integrity and customer linking

### 2. Data Preparation & Integration
- Merged transaction data with customer behavior data on loyalty_card_number
- Created time-based features (year, month, quarter) from transaction dates
- Calculated aggregate metrics by customer segment
- Prepared clean dataset for analysis

### 3. Customer Segmentation Analysis

**By Life Stage:**
- Calculated total revenue per life stage
- Identified older singles/couples as top revenue driver
- Retirees as second-highest contributing segment
- Analyzed purchase frequency patterns across life stages

**By Customer Type:**
- Compared Budget vs. Mainstream vs. Premium performance
- **Key Discovery**: Mainstream customers generate more total revenue than Premium customers
- Calculated revenue per customer and purchase frequency by type

### 4. Product Performance Analysis
- Identified top 10 best-selling products by revenue
- Analyzed product preferences across customer segments
- Evaluated product diversity in customer purchases

### 5. Temporal Analysis
- Monthly revenue trends to identify seasonality
- Peak purchasing periods identified

## Key Visualizations
All visualizations include labeled values for clarity and immediate insight.

**Revenue by Life Stage**
<img width="1000" height="600" alt="customer_revenue_by_lifestage" src="https://github.com/user-attachments/assets/5298a7b0-3f9d-48ba-ad20-2c0cc6ecfc33" />
- Shows older singles/couples and retirees as dominant revenue sources
- Clear revenue hierarchy across all seven life stage segments

**Revenue by Customer Type**
<img width="1000" height="600" alt="customer_class_comparison" src="https://github.com/user-attachments/assets/a39d3860-b1af-486f-8443-9676773e3b8b" />
- Demonstrates Mainstream segment outperforming Premium
- Includes customer counts and revenue per customer metrics

**Purchase Frequency by Segment**
<img width="1000" height="600" alt="purchase_frequency" src="https://github.com/user-attachments/assets/8147fe00-28bd-41c6-be62-2b8687d27143" />
- Highlights which segments shop most frequently
- Identifies engagement opportunities in underperforming segments

**Top 10 Products**
<img width="1300" height="600" alt="top_products" src="https://github.com/user-attachments/assets/fe110efd-837f-4e0d-a751-5e17fb509da9" />
- Best-selling chips products by total revenue
- Foundation for inventory and merchandising decisions

**Monthly Revenue Trends**
<img width="1400" height="600" alt="monthly_revenue" src="https://github.com/user-attachments/assets/d291fd7b-5daf-4d57-a42a-f11ccbc7f96a" />
- Seasonality patterns in chips purchases
- Identifies peak and low-performing periods

  ## Business Recommendations

### Priority 1: Protect Core Revenue - Older Singles/Couples & Retirees (Immediate)
**Finding:** Older singles/couples and retirees drive the majority of revenue

**Actions:**
- Implement VIP loyalty program specifically for these high-value segments
- Monitor purchase frequency closely; trigger retention outreach for any drop-offs
- Ensure product selection and inventory align with their preferences
- Optimize store operations (hours, promotions, layout) for older demographic shopping patterns

**Why:** These two segments are the revenue foundation. Losing even 5% of these customers would significantly impact the bottom line. Retention is cheaper than acquisition.

**Expected Impact:** Maintain 95%+ retention rate, protect largest revenue base

---

### Priority 2: Investigate and Fix Premium Segment Underperformance (3-6 months)
**Finding:** Premium customers generate the least revenue despite their classification

**Actions:**
- Survey Premium customers to understand satisfaction levels and unmet needs
- Analyze purchase frequency: Why are they shopping less than Mainstream customers?
- Review product offerings: Do premium products meet their expectations?
- Determine if the Premium classification criteria are appropriate or need revision

**Why:** This is a counterintuitive finding that suggests either misclassification, poor product-market fit, or untapped potential in this segment.

**Expected Impact:** Understand the gap between Premium label and actual behavior; inform strategy to either improve Premium performance or reclassify customers

---

### Priority 3: Reallocate Marketing to Match Revenue Reality (Next Quarter)
**Finding:** Older demographics drive revenue, but marketing may target younger segments

**Actions:**
- Shift 30-40% of marketing budget toward channels that reach older audiences (traditional media, direct mail, community partnerships)
- Reduce spend on social media and channels primarily reaching younger demographics unless strategic for long-term growth
- Test messaging and promotions specifically designed for older singles/couples and retirees
- Partner with senior organizations and retirement communities for customer acquisition

**Why:** Marketing effectiveness improves dramatically when targeting actual high-value customers rather than assumed targets.

**Expected Impact:** -20% customer acquisition cost for high-value segments, improved marketing ROI

  
## Future Enhancements

- RFM (Recency, Frequency, Monetary) analysis for more granular segmentation
- Customer lifetime value prediction modeling
- Basket analysis: What products are frequently purchased together?
- Time-series forecasting for demand planning
- Campaign effectiveness measurement framework

## Technical Notes

- Analysis conducted using Python 3.x
- All visualizations saved at 300 DPI for presentation quality
- Data cleaning documented with before/after metrics
- Reproducible analysis: Run notebook top-to-bottom to replicate findings

## How to Use This Repository

1. **Start with README** (you're here) - Get project overview and key findings
2. **Review `customer_analysis.ipynb`** - See complete analysis with code, visualizations, and detailed insights
3. **Check `visualizations/` folder** - View all charts independently
4. **Read inline comments** - Code is documented with business context

## Contact

**Jeffery Omoake**  
Data Analyst  
📧 jeffreyomoake01@gmail.com  
🔗 https://www.notion.so/jefferyomoake/Jeffery-Omoake-Data-Analyst-Portfolio-2c370a80defc80929584ca3adf23d9cb?source=copy_link

---

*This is a portfolio project demonstrating data analysis capabilities using retail transaction data. Findings and recommendations are based on analytical exploration and industry best practices.*
