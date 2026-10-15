# AdventureWorks Sales Analysis | Power BI

[English](#english) | [Русский](#русский)

<a id="english"></a>
## English

An end-to-end Power BI sales analytics project built on the AdventureWorks dataset. The report combines executive KPIs, product performance, customer segmentation, geographic analysis, and time-intelligence views in a five-page interactive dashboard.

## Live Dashboard

[Open the interactive Power BI report](https://app.powerbi.com/links/BynCJQ-POV?ctid=1cd03a56-3a2e-40dc-aefc-09745cd2cbc2&pbi_source=linkShare)

## Dashboard Pages

1. **Executive Overview** - revenue, profit, margin, orders, quantity sold, average order value, YoY performance, and YTD comparison.
2. **Product Analysis** - category revenue, profit margin by category, top products by profit, and top products by quantity sold.
3. **Customer Analysis** - customer count, revenue per customer, occupation segments, and income-group behavior.
4. **Geographic Analysis** - revenue performance by country and sales territory region.
5. **Time Analysis** - monthly revenue, previous-year comparison, YTD performance, monthly YoY growth, and YTD YoY growth.

## Key KPIs

For the selected 2013 view:

| KPI | Value |
|---|---:|
| Revenue | **$16.35M** |
| Profit | **$6.77M** |
| Profit Margin | **41.37%** |
| Orders | **21K** |
| Quantity Sold | **53K** |
| Average Order Value | **$768.08** |
| Revenue YoY | **179.87%** |

## Key Insights

- **Bikes dominate total revenue**, substantially exceeding Accessories and Clothing.
- **Accessories have the highest profit margin**, at roughly 62%, while Bikes and Clothing are around 40%.
- The **Professional** occupation segment generates the most revenue and also has the highest revenue per customer.
- The **60K income group** contains the largest customer segment and generates the highest revenue among the income bands.
- The **United States** is the strongest country by revenue, followed by Australia.
- Current-year monthly revenue remains above the previous year throughout the selected period.
- Monthly YoY growth is strongest around **May**, while **February** shows the weakest YoY growth in the selected year.

## Data Model

The report uses a fact-and-dimension model centered on **FactInternetSales** with:

- DimDate
- DimCustomer
- DimProduct
- DimProductSubcategory
- DimProductCategory
- DimSalesTerritory

This structure supports slicing sales measures across time, customers, products, and geography.

## Core Measures

The model includes business and time-intelligence measures such as:

- Revenue
- Cost
- Profit
- Profit Margin
- Orders
- Quantity Sold
- Customers
- Average Order Value
- Revenue per Customer
- Revenue Previous Year
- Revenue YoY %
- Revenue YTD
- Revenue YTD Previous Year
- Revenue YTD YoY %

## Skills Demonstrated

- Power BI Desktop
- DAX measures
- Time intelligence: previous year, YTD, and YoY
- Data modeling and relationships
- KPI design
- Product and customer segmentation
- Geographic sales analysis
- Interactive slicers and cross-filtering
- Dashboard layout and visual consistency

## Project Files

- [Download the Power BI project](AdventureWorks_Sales_Analysis.pbix) - editable `.pbix` file
- [View the exported report](AdventureWorks_Sales_Analysis.pdf) - five-page PDF
- [Browse dashboard screenshots](screenshots/) - report pages and data model preview

## Dashboard Preview

### Executive Overview

![Executive Overview](screenshots/executive-overview.png)

### Product Analysis

![Product Analysis](screenshots/product-analysis.png)

### Customer Analysis

![Customer Analysis](screenshots/customer-analysis.png)

### Geographic Analysis

![Geographic Analysis](screenshots/geographic-analysis.png)

### Time Analysis

![Time Analysis](screenshots/time-analysis.png)

### Data Model

![Data Model](screenshots/data-model.png)

## Repository Structure

```text
adventureworks-powerbi-sales-analysis/
├── AdventureWorks_Sales_Analysis.pbix
├── AdventureWorks_Sales_Analysis.pdf
├── README.md
├── PROJECT_NOTES.md
└── screenshots/
    ├── executive-overview.png
    ├── product-analysis.png
    ├── customer-analysis.png
    ├── geographic-analysis.png
    ├── time-analysis.png
    └── data-model.png
```

## Author

**Yrysdaulet**  
Portfolio project focused on Power BI, business intelligence, data analytics, and DAX.

---

<a id="русский"></a>
## Русский

Это сквозной аналитический проект в **Power BI** на датасете AdventureWorks. Отчёт объединяет ключевые бизнес-показатели, анализ товаров, сегментацию клиентов, географический анализ и Time Intelligence в пятистраничном интерактивном дашборде.

### Интерактивный отчёт

[Открыть интерактивный отчёт Power BI](https://app.powerbi.com/links/BynCJQ-POV?ctid=1cd03a56-3a2e-40dc-aefc-09745cd2cbc2&pbi_source=linkShare)

### Страницы отчёта

1. **Executive Overview** — выручка, прибыль, маржинальность, количество заказов, проданные единицы, средний чек, YoY и сравнение YTD.
2. **Product Analysis** — выручка по категориям, маржинальность категорий, топ товаров по прибыли и количеству продаж.
3. **Customer Analysis** — количество клиентов, выручка на клиента, сегментация по профессии и уровню дохода.
4. **Geographic Analysis** — выручка по странам и регионам продаж.
5. **Time Analysis** — помесячная динамика выручки, сравнение с предыдущим годом, YTD, YoY и YTD YoY.

### Ключевые KPI

Для выбранного 2013 года:

| Показатель | Значение |
|---|---:|
| Выручка | **$16,35 млн** |
| Прибыль | **$6,77 млн** |
| Маржинальность | **41,37%** |
| Заказы | **21 тыс.** |
| Продано единиц | **53 тыс.** |
| Средний чек | **$768,08** |
| Рост Revenue YoY | **179,87%** |

### Основные выводы

- Категория **Bikes** формирует подавляющую часть общей выручки.
- **Accessories** имеют самую высокую маржинальность — около **62%**, тогда как Bikes и Clothing находятся примерно на уровне 40%.
- Сегмент клиентов **Professional** приносит наибольшую выручку и показывает один из самых высоких показателей выручки на клиента.
- Группа дохода около **60K** является крупнейшей по количеству клиентов и формирует наибольшую выручку среди групп дохода.
- По странам лидируют **United States**, затем **Australia**.
- Помесячная выручка выбранного года выше показателей предыдущего года во всех отображённых месяцах.
- Самый высокий YoY-рост наблюдается примерно в **мае**, самый низкий — в **феврале**.

### Модель данных

Отчёт построен вокруг таблицы фактов **FactInternetSales** и связанных таблиц измерений:

- DimDate
- DimCustomer
- DimProduct
- DimProductSubcategory
- DimProductCategory
- DimSalesTerritory

Такая модель позволяет анализировать продажи по времени, клиентам, товарам и географии, а также использовать иерархию Category → Subcategory → Product.

### Основные DAX-меры

В проекте используются бизнес-метрики и Time Intelligence:

- Revenue
- Cost
- Profit
- Profit Margin
- Orders
- Quantity Sold
- Customers
- Average Order Value
- Revenue per Customer
- Revenue Previous Year
- Revenue YoY %
- Revenue YTD
- Revenue YTD Previous Year
- Revenue YTD YoY %

### Что демонстрирует проект

- Power BI Desktop
- DAX
- Time Intelligence: Previous Year, YTD, YoY
- Моделирование данных и связи между таблицами
- KPI и бизнес-метрики
- Анализ товаров и клиентов
- Географический анализ продаж
- Drill-down, срезы и кросс-фильтрация
- Проектирование структуры и визуального оформления дашборда

### Файлы проекта

- [Скачать Power BI проект](AdventureWorks_Sales_Analysis.pbix) — редактируемый файл `.pbix`
- [Открыть PDF-версию отчёта](AdventureWorks_Sales_Analysis.pdf) — экспорт пяти страниц
- [Открыть скриншоты](screenshots/) — страницы дашборда и модель данных

### Структура репозитория

```text
adventureworks-powerbi-sales-analysis/
├── AdventureWorks_Sales_Analysis.pbix
├── AdventureWorks_Sales_Analysis.pdf
├── README.md
├── PROJECT_NOTES.md
└── screenshots/
    ├── executive-overview.png
    ├── product-analysis.png
    ├── customer-analysis.png
    ├── geographic-analysis.png
    ├── time-analysis.png
    └── data-model.png
```

### Автор

**Yrysdaulet**  
Портфолио-проект по Power BI, Business Intelligence, аналитике данных и DAX.
