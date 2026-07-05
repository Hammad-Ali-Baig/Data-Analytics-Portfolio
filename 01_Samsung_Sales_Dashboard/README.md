# Samsung Supply Chain & Shipment Analytics Dashboard

A single-page Power BI dashboard analyzing shipment performance, inventory health, and profitability across Samsung's customer, product, and supplier network.

## 📊 Overview

This dashboard consolidates shipment, product, customer, and supplier data into a single operational view, designed to help supply chain and logistics stakeholders monitor delivery performance, inventory levels, and profitability at a glance.

## 🗂️ Data Model

The report uses a star-schema style model with one fact table and three dimension tables:

| Table | Role |
|---|---|
| `fact_shipment` | Fact table — shipment-level transactions (quantity, delay, revenue, cost) |
| `dim_customer` | Dimension — customer name and attributes |
| `dim_product` | Dimension — product name and attributes |
| `dim_supplier` | Dimension — supplier name, carrier |
| `Measuress` | Dedicated measures table holding all DAX calculations |

## 📐 Key DAX Measures

- **Gross Revenue** / **Total Revenue** — total shipment revenue
- **Profit** / **Profit Margin %** — profitability by shipment
- **Inventory Value** — value of stock on hand
- **Safety Stock** — minimum stock threshold
- **Total Shipment** / **Total Shipment Quantity** — shipment volume
- **Total Delivered Quantity** — units successfully delivered
- **Total Delay** / **Total Qty Delay** — delay tracking across shipments
- **Perfect Order %** — percentage of orders delivered on-time, complete, and damage-free
- **Avg Load Time** — average time to load a shipment
- **Order Qty** — total quantity ordered

## 📈 Visuals

- KPI cards for top-line metrics (revenue, profit, delay, perfect order rate, etc.)
- Donut charts breaking down shipments by carrier / product / customer
- Clustered bar charts comparing performance across customers, products, and suppliers
- Custom theme and branded imagery for a polished, presentation-ready layout

## 🛠️ Tools Used

- **Power BI Desktop** — data modeling, DAX, report design
- Custom Power BI theme (JSON) for consistent branding

## 🚀 How to Use

1. Download `samsung.pbix` and open it in Power BI Desktop.
2. If prompted, point the data source connections to your own copy of the underlying dataset (customer, product, supplier, and shipment tables).
3. Explore the report using the cross-filtering visuals — click any bar or donut segment to filter the rest of the page.

## 👤 Author

Built by **Hammad** as part of a data analytics portfolio focused on supply chain and logistics analytics using Power BI.
