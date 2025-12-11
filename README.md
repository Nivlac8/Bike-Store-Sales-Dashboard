# 🚴 Bike Store Analytics: Dynamic Search & Sales Dashboard

### 📌 Project Overview
This project solves a common retail problem: efficient inventory management and pricing analysis. I built a dual-purpose Excel application that serves two user types:
1.  **Sales Staff:** A front-end "Search Tool" allowing instant retrieval of product specs, pricing, and stock status during customer interactions.
2.  **Management:** A back-end "Analytics Dashboard" providing high-level insights into brand distribution and pricing strategies.

### 📂 Project Files
| File Name | Description | Download/View |
| :--- | :--- | :--- |
| **Bike_Store_Analytics.xlsx** | The complete functional Excel Application (Search Tool + Dashboard). | [📥 Download File](Bike_Store_Analytics.xlsx) |
| **search_tool_preview.png** | Screenshot of the front-end Search UI. | [👁️ View Image](search_tool_preview.png) |
| **dashboard_preview.png** | Screenshot of the back-end Analytics Dashboard. | [👁️ View Image](dashboard_preview.png) |

### 📊 The Dataset
**Source:** [Bike Store Relational Database (Kaggle)](https://www.kaggle.com/datasets/dillonmyrick/bike-store-sample-database)
*(Note: The raw data is also fully embedded within the `Products` and `Brands` sheets of the Excel file for offline access.)*

**Structure:**
* **Products Table:** `product_id`, `product_name`, `list_price`, `model_year`
* **Brands Table:** `brand_id`, `brand_name`
* **Stocks Table:** Inventory counts by store location

### 🛠️ Skills Applied
**Tool:** Microsoft Excel (Advanced)

#### 1. Application Development (The Search Tool)
* **Dynamic Lookups:** Engineered a search engine using `VLOOKUP` and `INDEX-MATCH` to link disparate datasets (Products ↔ Brands) based on user input.
* **Error Handling:** Implemented `IFERROR` wrappers to ensure a clean, professional UI that handles missing or incorrect search terms gracefully.
* **User Interface Control:** Utilized Data Validation (Dropdown Lists) and Cell Protection to prevent user error and breakages in the formula logic.

#### 2. Data Analysis & Visualization (The Dashboard)
* **Pivot Table Modeling:** Aggregated raw sales data to calculate key metrics like "Average Price per Brand" and "SKU Count by Category."
* **Interactive Slicers:** Connected multiple charts to a single Slicer control, enabling instant filtering by **Model Year** and **Category**.
* **Data Cleaning:** Sanitized the raw dataset by removing non-breaking spaces (ASCII 160) and correcting text-to-number formatting issues using data transformation tools.

### ⚙️ How to Use This Tool
1.  **Download** the `Bike_Store_Analytics.xlsx` file.
2.  **Open** the file in Excel (Desktop or Web).
3.  Navigate to the **Search_Tool** tab.
4.  Select a bike from the **Dropdown Menu** (Cell A3) to see the dynamic price update.
5.  Navigate to the **Dashboard** tab and use the **Slicers** to filter the charts.

---
*Created as part of a Data Analytics Portfolio Project.*
