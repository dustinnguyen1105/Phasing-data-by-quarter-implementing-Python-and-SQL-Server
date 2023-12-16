Phasing-data-by-quarter-using-Python-and-SQL-Server

<h1>How to use this repo?</h1>

You are a distribution company that sells dental care products to retail stores across the country. Let's just assume that those retail stores sell all the product quantity till the repeat order date for the same product. Since they don't want to share their POS data with us, we have to assume that the average quantity of a product sold per day is the actual POS sales data.

![image](https://github.com/dustinnguyen1105/Phasing-data-by-quarter-implementing-Python-and-SQL-Server/assets/153787396/fe0c88ca-8898-4e03-b945-0e223231f9ab)

Therefore, in order to calculate the actual sales of the retail stores per month/quarter/year we will perform a simple calculation like below:
For example, the toothbrush product is purchased 100 units, the purchase date is 12/16/2023 and the repeat order date for the same product is 11/13/2024.
1. The total days between the purchased date and the repeat order date is 333 days.
2. So the average quantity that the retail stores sell that particular product = 100 / 333 = 0.3003 (unit/per day)
3. Finally, if you want to phase by quarter the total quantity per unit will be:
The unit sold in Q1-2024 = 0.3003 * 91 (total days in Q1-2024) = 27.33 (unit)<br>
However in Q4-2023 the total unit sold = 0.3003 * 16 (total days in Q4-2024 = 12/31/2023 - 12/16/2023 + 1) = 4.80 (unit)   

Visist my notebook for the detail code, I will extract similar data from SQL Server for drug products in tender hospital data and perform phasing by Quarter/Month.
