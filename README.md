# Retail-Dashboard
a Retail Dashboard I have created based on a sales data file. It includes the best selling products, QoQ statistics on revenue, quantities and active customers. The dashboard is interactive through slicers, allowing selection of specific regions, customer segments, and the sales channel.
It answers questions on sales trends in different categories of customers, sales channels and geographic regions. It also answers the question about which products perfomred best in different quarters.

The data sources exists out of three csv's:
sales.csv
  OrderID
  OrderDate
  CustomerID
  Product
  Quantity
  UnitPrice
  Status
  Channel
regions.csv
  Country
  Region
customers.csv
  CustomerID 
  Name
  Segment
  Country

These data sources were transformed into a single data model:
FactSales
  OrderID
  OrderDate
  Year
  Quarter
  MonthNum
  CustomerID
  Name
  Segment
  Country
  Regions
  Product
  Quantity
  UnitPrice
  LineRevenue
  OrderSize
  Channel
  Status

This transformation was done with Power Query, through merging queries, replacing values to clean the data, trimming data, and correcting data types.

Then, pivot tables were created together with slicers to facilitate the dynamic data sources for a dashboard. 

Lastly, the dashboard itself was created to show the most important data and to respond to the slicers that are included.

