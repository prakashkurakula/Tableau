# Tableau
# 🗺️ Tableau – Normal Maps and Filled Maps

## 📌 Introduction

Maps in Tableau are used to visualize geographical data and understand how information varies across different locations.

Tableau provides different map visualization techniques to represent geographical information. Two important types are:

1. **Normal Maps (Symbol Maps)**
2. **Filled Maps (Choropleth Maps)**

Both maps help users understand geographical patterns, compare locations, and analyze business performance.

---

# 1. Normal Maps (Symbol Maps)

## 📖 What is a Normal Map?

A Normal Map, commonly called a **Symbol Map** in Tableau, is a geographical visualization that represents locations using symbols such as circles or other marks on a map.

Each symbol represents a geographical location, such as a country, state, city, or region.

The size and color of the symbols can be changed based on measures such as Sales, Profit, Quantity, or Customer Count.

### 🎯 Purpose of Normal Maps

- To identify different geographical locations.
- To compare business performance across cities or states.
- To display the distribution of sales across locations.
- To identify high-performing and low-performing locations.
- To analyze geographical patterns using different symbol sizes and colors.

## ⚙️ How to Create a Normal Map in Tableau

Follow these steps:

**Step 1:** Open Tableau Desktop.

**Step 2:** Connect to your dataset (Excel, CSV, or another supported data source).

**Step 3:** Identify the geographical field.

Examples:
- Country
- State
- City
- Region
- Postal Code

**Step 4:** Double-click the geographical field, such as `State` or `City`.

Tableau automatically generates a map using its geographical information.

**Step 5:** Drag the `Sales` measure to the **Size** option in the Marks card.

This changes the size of the circles based on sales values.

**Step 6:** Drag the `Profit` measure to **Color**.

This changes the color of the circles based on profit values.

**Step 7:** Drag additional fields such as Customer Name, Sales, or Quantity to **Tooltip**.

**Step 8:** Customize the map using colors, sizes, labels, and map formatting.

### 📌 Important Components of a Normal Map

| Component | Description |
|---|---|
| Detail | Defines the geographical level displayed on the map. |
| Size | Controls the size of geographical symbols. |
| Color | Represents measures using different colors. |
| Label | Displays information directly on the map. |
| Tooltip | Displays additional information when hovering over a symbol. |
| Latitude | Represents the north-south geographical position. |
| Longitude | Represents the east-west geographical position. |

### 💻 Example: Normal Map

**Business Scenario: Sales Analysis Across Different Cities**

A company operates in multiple cities and wants to identify which cities generate the highest sales.

**Dataset:**

| City | Sales | Profit |
|---|---:|---:|
| New York | 25000 | 5000 |
| Los Angeles | 18000 | 3500 |
| Chicago | 12000 | 2000 |
| Houston | 30000 | 7000 |
| Seattle | 15000 | 2500 |

**Steps:**

1. Drag `City` into the view.
2. Tableau generates a geographical map.
3. Drag `Sales` to Size.
4. Drag `Profit` to Color.
5. Drag `City`, `Sales`, and `Profit` to Tooltip.

**Expected Result:**

- Houston displays a larger circle because it has the highest sales.
- Chicago displays a smaller circle because it has lower sales.
- Circle colors indicate differences in profit.

**Business Insight:**

Management can easily identify cities generating higher sales and compare their profitability.

---

# 2. Filled Maps (Choropleth Maps)

## 📖 What is a Filled Map?

A Filled Map, also known as a **Choropleth Map**, is a geographical visualization in Tableau that uses different colors to fill geographical areas such as countries, states, or regions.

The color intensity represents a particular measure or category.

For example:
- Dark green represents higher sales.
- Light green represents moderate sales.
- Red represents lower sales.

Filled Maps are useful for comparing geographical areas based on numerical values or categories.

### 🎯 Purpose of Filled Maps

- To compare sales across different states or countries.
- To identify high-performing and low-performing regions.
- To analyze geographical distribution.
- To understand regional business performance.
- To identify patterns using different color intensities.

## ⚙️ How to Create a Filled Map in Tableau

Follow these steps:

**Step 1:** Open Tableau Desktop.

**Step 2:** Connect to your dataset.

**Step 3:** Identify a geographical field such as `Country`, `State`, or `Region`.

**Step 4:** Double-click the geographical field.

Tableau generates a map based on the geographical locations.

**Step 5:** In the Marks card, change the mark type to **Map** (Filled Map).

Alternatively, select the Filled Map visualization from Show Me when the selected fields support it.

**Step 6:** Drag the `Sales` measure to the **Color** option.

**Step 7:** Tableau automatically assigns colors based on the sales values.

**Step 8:** Drag additional measures such as Profit, Quantity, or Customer Count to Tooltip.

**Step 9:** Customize the color palette, labels, and map formatting.

### 📌 Important Components of a Filled Map

| Component | Description |
|---|---|
| Detail | Identifies geographical areas such as states or countries. |
| Color | Fills geographical areas based on measures or dimensions. |
| Label | Displays geographical names or numerical values. |
| Tooltip | Displays additional information when hovering over an area. |
| Geography | Defines the geographical boundaries of the map. |
| Color Palette | Helps distinguish high and low values. |

### 💻 Example: Filled Map

**Business Scenario: State-Wise Sales Analysis**

A company wants to analyze sales performance across different states and identify which states generate the highest revenue.

**Dataset:**

| State | Sales |
|---|---:|
| California | 50000 |
| Texas | 35000 |
| New York | 45000 |
| Florida | 20000 |
| Washington | 15000 |

**Steps:**

1. Drag `State` into the view.
2. Tableau generates a geographical map.
3. Select the Filled Map mark type.
4. Drag `Sales` to Color.
5. Drag `State` and `Sales` to Tooltip.
6. Customize the color palette.

**Expected Result:**

- California appears with a darker color because it has the highest sales.
- New York appears with a relatively dark color.
- Washington appears with a lighter color because it has the lowest sales.

**Business Insight:**

Management can identify which states contribute more revenue and which states need additional business attention.

---

# 3. Difference Between Normal Maps and Filled Maps

| Feature | Normal Map | Filled Map |
|---|---|---|
| Other Name | Symbol Map | Choropleth Map |
| Visualization | Uses symbols or circles | Uses filled geographical areas |
| Representation | Points or locations | Geographical boundaries |
| Size | Can represent values using symbol size | Does not use symbol size to fill areas |
| Color | Can represent measures or categories | Represents measures or categories through area colors |
| Best Used For | Comparing individual locations | Comparing geographical regions |
| Example | City-wise Sales | State-wise Sales |
| Main Purpose | Location-based analysis | Area-based analysis |

### 🔍 Key Difference

**Normal Map:** Uses circles or symbols to represent geographical locations.

**Filled Map:** Uses different colors to represent geographical areas.

---

# 4. Real-Time Business Scenarios

## Scenario 1: Retail Sales Analysis

**Requirement:** A retail company wants to identify which cities generate the highest sales.

**Solution:** Use a Normal Map.

- City → Detail
- Sales → Size
- Profit → Color
- Sales and Profit → Tooltip

**Business Benefit:** Helps identify high-revenue cities.

## Scenario 2: Regional Performance Analysis

**Requirement:** A company wants to compare sales performance across different states.

**Solution:** Use a Filled Map.

- State → Detail
- Sales → Color
- Profit → Tooltip

**Business Benefit:** Helps identify high-performing and low-performing states.

## Scenario 3: Customer Distribution Analysis

**Requirement:** A business wants to understand the geographical distribution of customers.

**Solution:** Use a Normal Map.

- City → Detail
- Customer Count → Size
- Region → Color

**Business Benefit:** Helps identify locations with more customers.

## Scenario 4: Country-Wise Revenue Analysis

**Requirement:** An international company wants to compare revenue across different countries.

**Solution:** Use a Filled Map.

- Country → Detail
- Revenue → Color
- Country and Revenue → Tooltip

**Business Benefit:** Helps management understand the revenue contribution of different countries.

---

# 5. Important Tableau Concepts Related to Maps

### 1. Geographic Roles

Geographic Roles help Tableau recognize geographical fields.

Examples:
- Country/Region
- State/Province
- City
- Postal Code
- County

**How to Assign a Geographic Role:**

1. Right-click a geographical field.
2. Select Geographic Role.
3. Choose the appropriate geographical category.

### 2. Generated Latitude and Longitude

Tableau automatically generates Latitude and Longitude for recognized geographical locations.

- Latitude (generated): Represents the north-south position.
- Longitude (generated): Represents the east-west position.

These fields help Tableau position geographical locations on the map.

### 3. Map Layers

Map Layers allow users to customize the background map and display geographical details.

Examples:
- Streets
- Borders
- Country and region names
- Coastlines

### 4. Tooltip

A Tooltip displays additional information when a user hovers over a geographical mark or area.

Example:

- State: California
- Sales: 50,000
- Profit: 10,000

### 5. Color Encoding

Color Encoding represents measures or dimensions using different colors.

Example:

- Dark Green → High Sales
- Light Green → Medium Sales
- Red → Low Sales

---

# 6. Advantages of Normal Maps and Filled Maps

## Advantages of Normal Maps

1. Easy to identify geographical locations.
2. Helps compare individual cities and locations.
3. Supports size-based comparisons.
4. Helps analyze customer distribution.
5. Provides interactive geographical analysis.

## Advantages of Filled Maps

1. Easy to compare geographical regions.
2. Identifies high-performing and low-performing areas.
3. Helps visualize regional sales distribution.
4. Provides better understanding of geographical patterns.
5. Supports business decision-making.

---

# 7. Limitations of Maps in Tableau

1. Incorrect geographical data can result in unknown locations.
2. Too many symbols can make a Normal Map difficult to understand.
3. Filled Maps may not be suitable for displaying individual customer locations.
4. Similar colors can make comparisons difficult.
5. Geographic maps require correctly recognized geographical fields.
6. Some geographical areas may not be available in Tableau's built-in geographic database.

---

# 8. Best Practices for Creating Maps

1. Always verify Geographic Roles before creating a map.
2. Use Normal Maps for individual locations.
3. Use Filled Maps for geographical areas.
4. Select appropriate colors to improve readability.
5. Avoid using too many colors.
6. Use Tooltips to display additional information.
7. Include meaningful titles.
8. Check for unknown or unmatched geographical locations.
9. Avoid overcrowding the map with labels.
10. Choose the appropriate geographical level for your analysis.

---

# 9. Interview Questions and Answers

**Q1. What is a Normal Map in Tableau?**

A: A Normal Map, also called a Symbol Map, represents geographical locations using symbols such as circles. The size and color of the symbols can represent measures such as Sales, Profit, and Quantity.

**Q2. What is a Filled Map in Tableau?**

A: A Filled Map represents geographical areas using different colors. It is useful for comparing measures across states, countries, and regions.

**Q3. What is the main difference between Normal Maps and Filled Maps?**

A: Normal Maps use symbols to represent geographical locations, whereas Filled Maps use colors to fill geographical boundaries.

**Q4. Can we use Sales in a Normal Map?**

A: Yes. We can drag Sales to Size or Color to represent sales performance across different geographical locations.

**Q5. Can we use Profit in a Filled Map?**

A: Yes. We can drag Profit to Color to compare profit performance across different geographical areas.

**Q6. What is Geographic Role in Tableau?**

A: Geographic Role tells Tableau how to identify and interpret geographical fields such as Country, State, City, and Postal Code.

**Q7. What are Generated Latitude and Longitude?**

A: These are automatically generated geographical coordinates used by Tableau to position locations on a map.

**Q8. When should we use a Filled Map?**

A: We should use a Filled Map when we want to compare geographical areas based on measures such as Sales, Profit, or Revenue.

**Q9. When should we use a Normal Map?**

A: We should use a Normal Map when we want to visualize and compare individual geographical locations using symbols.

**Q10. What is the use of Tooltip in Tableau Maps?**

A: Tooltip displays additional information when users hover over a geographical symbol or area.

---

# 10. Practical Implementation in My Tableau Workbook

I practiced Normal Maps and Filled Maps using the Superstore dataset.

### Worksheets Created

| Worksheet Name | Map Type | Purpose |
|---|---|---|
| City_info | Normal Map | City-level geographical analysis |
| Country | Normal Map | Country-level geographical analysis |
| Country_filledmap | Filled Map | Country-wise geographical visualization |
| State_Sale_Top | Normal Map | State-wise sales analysis |
| State_sale_top_filledmap | Filled Map | State-wise sales visualization using Sales |
| States_filledmap | Filled Map | State-level geographical visualization |
| states | Normal Map | State-level geographical analysis |

### Fields Used

- Country
- State
- City
- Region
- Sales

### Practical Learning Outcomes

- Learned how to create Normal Maps in Tableau.
- Learned how to create Filled Maps in Tableau.
- Understood the difference between Symbol Maps and Choropleth Maps.
- Practiced geographical analysis using Country, State, and City.
- Learned how to represent Sales using colors.
- Understood how Tableau uses generated Latitude and Longitude.
- Learned how to analyze geographical business performance.

---

# 11. Conclusion

Normal Maps and Filled Maps are important geographical visualization techniques in Tableau.

**Normal Maps** are useful for analyzing individual geographical locations using symbols, sizes, and colors.

**Filled Maps** are useful for comparing geographical areas using different color intensities.

Both visualizations help businesses understand geographical patterns, analyze sales performance, identify opportunities, and make better business decisions.

---

## 📚 Topics Covered

- [x] Introduction to Tableau Maps
- [x] Normal Maps (Symbol Maps)
- [x] Filled Maps (Choropleth Maps)
- [x] Creating Normal Maps Step by Step
- [x] Creating Filled Maps Step by Step
- [x] Difference Between Normal Maps and Filled Maps
- [x] Business Scenarios
- [x] Geographic Roles
- [x] Generated Latitude and Longitude
- [x] Tooltips and Color Encoding
- [x] Advantages and Limitations
- [x] Best Practices
- [x] Interview Questions and Answers
- [x] Practical Implementation

**Thank You!**

*Learning Tableau | Data Visualization | Data Analytics*
