---
name: Home
assetId: 7e08009c-39f4-4f88-91af-ea6f803d4fad
type: page
cards: true
page_width: full
---

{% table
  data="demo_daily_orders"
/%}

{% bar_chart
  data="demo_daily_orders"
  x="date"
  date_grain="month"  
  y="sum(total_sales)"
/%}

{% line_chart
  title="Total Sales Over Time"
  data="demo_daily_orders"
  x="date"
  y="sum(total_sales)"
  date_grain="month"
  y_fmt="usd"
/%}