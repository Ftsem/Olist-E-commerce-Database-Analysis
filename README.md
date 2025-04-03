# Olist-E-commerce

Olist is a Brazilian Startup with funding from multiple large banks and companies. It serves a similar niche as Amazon marketplace, connecting small and large sellers to customers on a single website, handling logistics of getting product to the customer from the seller. I have analysed the provided data from 2016 to 2018 to offer data-driven improvements to business operations and strategy.






# 1. Order Trends Over Time

As I investigated the Olist dataset, based on the available data, I decided to analyze the data with the goal of increasing the count of orders. One of the ways to improve it was through effective marketing campaigns and sales strategies, and one of the most important factors for a successful campaign or sale was timing.

To propose the optimal timing to the company, I focused on identifying trends in total order counts based on different days, times of day, and months.



![Order Trends Over Time](https://github.com/Ftsem/Olist-E-commerce-Database-Analysis/blob/0cce2ac808bf69e05f5ad67d3b9f9bba9d7c3370/Order_Trends_Over_Time.png)


## Insights

#### 1. Number of Orders by Month
- **Highest Orders:**
  - **August**: 10.8K orders
  - **May**: 10.5K orders
  - **July**: 10.3K orders
- **Lowest Orders:**
  - **September**: 4.3K orders, showing a clear decline in sales.
- **Consistent Trends:**
  - **March and June** had stable orders between 9K and 9.5K, indicating steady demand.

#### 2. Number of Orders by Weekday
- **Highest Orders:**
  - **Monday**: 16.1K orders
  - **Tuesday**: 15.9K orders
  - **Wednesday**: 15.5K orders
- **Lowest Orders:**
  - **Saturday**: 10.8K orders, typical for weekends where orders tend to be lower.

#### 3. Number of Orders by Time of Day
- **Highest Orders:**
  - **Afternoon**: 38.13K orders
  - **Morning**: 26.84K orders
- **Lowest Orders:**
  - **Night**: 16.06K orders, showing a dip in activity during late hours.
  - **Evening**: 17.84K orders, less than the afternoon but still significant.



## Recommendations

#### 1. **Target High-Order Months for Marketing Campaigns:**
- Focus marketing efforts during **August** and **May**, the months with the highest order counts.
- Consider running promotional campaigns or flash sales to boost engagement during these months.

#### 2. **Focus on Weekdays for Promotions:**
- Launch special weekday promotions early in the week (especially on **Monday** through **Wednesday**) to maximize sales.
- Consider targeting **weekends (Saturday and Sunday)** with weekend-specific deals or reminders.

#### 3. **Adjust Delivery and Order Timing:**
- Since most orders happen in the **afternoon** and **morning**, prioritize marketing activities during these times.
- For **night-time** orders, avoid offering time-sensitive deals but consider scheduling campaigns or reminders to reach customers for next-day purchases.

#### 4. **Address Seasonal Trends in Order Volumes:**
- Implement pre-holiday sales or target specific customer segments in **November** and **December** where orders dip.
- Investigate the causes of the dip during these months (e.g., external market factors or seasonality).

#### 5. **Optimize for Weekday Traffic:**
- As weekdays show higher order volumes, schedule product launches, deals, and campaigns around **Monday to Wednesday** to capture customers when they are most active.

---

# 2. Delayed Deliveries Trends By Location
For further investigation, I aim to explore the **relationship between delayed orders** and **different customer cities**. To achieve this, I will be using the `olist_orders_dataset` and `Olist_customer_dataset`.

### Observations:
At first glance, I noticed that **São Paulo**, **Rio de Janeiro**, and **Salvador** had the highest number of delayed deliveries. However, this is expected, as these cities are Brazil's largest and most populated. 

### Next Steps:
To refine the analysis, I decided to understand which cities have the **highest delayed delivery rates** when compared to the total number of deliveries. This will help identify regions with delivery issues relative to their size, rather than just focusing on total order volume.

The key questions I will address include:
- Which cities have the highest **delay delivery rates** (delayed deliveries as a percentage of total deliveries)?
- How do these rates compare across different cities, especially in larger versus smaller cities?
- Can we identify cities that might need additional logistics support or improvements?

### Approach:
1. **Data Analysis**: 
   - I will calculate the delay rate by dividing the number of delayed deliveries by the total number of deliveries in each city.
   
2. **City-Level Comparison**:
   - I'll compare these rates across various cities to identify regions with the highest percentage of delayed orders.

3. **Customer City Insights**:
   - This investigation will offer insights into delivery performance and customer satisfaction in different areas, helping the company focus on cities with the highest delays.

## Insights

1. **Highest Delayed Deliveries by City:**
   - As shown in the analysis, **São Paulo** and **Rio de Janeiro** have the highest number of delayed deliveries. However, since these cities are more populous, the total order volume is also higher, which is to be expected.
   
2. **Delayed Delivery Rates:**
   - When comparing **delayed delivery rates** (delayed orders as a percentage of total deliveries), cities like **Armação dos Búzios** (46.43%) and **Santarém** (34.88%) stand out for having higher proportions of delayed deliveries relative to their order volume. This suggests that these cities may have logistical or infrastructure challenges affecting timely deliveries.

3. **Smaller Cities with Higher Delays:**
   - While large cities like **São Paulo** and **Rio de Janeiro** have higher raw numbers of delayed deliveries, some smaller cities such as **Armação dos Búzios**, **Maceió**, and **Santarém** have significantly higher rates of delayed deliveries per order. This could indicate that smaller cities are facing unique challenges that may not be as apparent in larger metropolitan areas.

4. **Coastal and Tourist-Heavy Cities:**
   - **Maceió**, **Santarém**, and **Armação dos Búzios** have the highest delayed delivery ratios. Upon further investigation, I found that these cities are coastal and popular tourist destinations. This could impact delivery logistics due to increased seasonal demand, fluctuating population sizes, and potential infrastructure challenges during peak tourist seasons.

## Recommendations

1. **Target High Delay Cities for Operational Improvements:**
   - Focus on cities with high **delayed delivery rates**, such as **Armação dos Búzios**, **Santarém**, and **Maceió**, to identify potential logistical bottlenecks or service inefficiencies. These cities should be prioritized for process improvements, such as optimizing delivery routes or enhancing local delivery infrastructure.

2. **Scale Logistics Support in Smaller Cities and Tourist Areas:**
   - While large cities will naturally have more delays due to their size and order volume, smaller coastal cities with high delayed delivery rates, such as **Armação dos Búzios** and **Maceió**, should receive more targeted logistics support. Enhance shipping times or offer local incentives for faster deliveries, especially during tourist seasons when demand spikes.

3. **Address Seasonal Demand in Tourist Destinations:**
   - **Maceió**, **Armação dos Búzios**, and **Santarém** experience higher delayed delivery ratios due to their status as **tourist hotspots**. During peak tourist seasons, these cities face an influx of visitors, which can strain logistics and delivery systems. Consider offering **seasonal delivery options** or **temporary delivery hubs** in these cities to handle increased demand.

4. **Data-Driven Campaigns for Larger Cities:**
   - For cities like **São Paulo**, **Rio de Janeiro**, and **Salvador**, it may be more effective to focus on improving customer communication and offering incentives for customers to choose alternative delivery times (e.g., choosing faster delivery options), as they are already dealing with high volumes.

5. **Regular Monitoring and Feedback Loop:**
   - Continuously monitor the delivery status for each city, especially those with high delay rates. Implement a feedback loop to track improvements after changes in logistics or services are made, ensuring that delivery times are improving and customer satisfaction is rising.

---

By focusing on cities with high delivery delay rates, particularly **coastal cities** and **tourist destinations**, this investigation can help guide the company towards making informed decisions regarding delivery logistics, customer satisfaction, and operational efficiencies in different regions.





