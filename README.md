# Jio_Mart_Report:

Dashboard link:https://1drv.ms/u/c/97ecacf04094eef0/EZvJWJv4hhtGge2JGBWnhFIBCVFZXwn7kagU66sk-ql5UQ?e=Gbg2ik

# Problem Statement:
This report help you understand about customer behaviour and price about the product also. 

Steps followed:   
-Step-1 : Clean data using excel and power Query editor, like remove duplicate and null values and give a proper format(Tabular format) which is understandable for analyzing and taking decision on the business problem.

-Step-2 : Load data in power BI desktop.

-Step-3 : Selecting the charts as per data view. like select column chart for shown sales price as per category, using slicers for filtering the data. 

-Step-4 : There are 2 calculated columns created one is "Type of Price" and another is "Rating group"

for creating new column following expression was written;
       Type of price=

	(if sale_price = market_price (" Price as per the market")
	(if sale_price < market_price ("under_price")
	(else "over price")
	
	Rating group=
	(if table[age] <=2 "1 to 2")
	(if table[age] <=3 "2 to 3")
	(if table[age] <=4 "3 to 4")
	(else "4 to 5")

snap of calculated columns:
![Image](https://github.com/user-attachments/assets/e66789bd-a301-493b-9ba4-1c41c307fdeb)


-Step-5 : New measure was created to find total market price and avg market price.
	
	Total market price= sum(market price)
	Avg.market price= Avg(market price)

A card was used to represent market price.

snap_of_total_mrket_price:
![Image](https://github.com/user-attachments/assets/2a123ae7-4e6a-4662-887e-c3001a199aa1)

snap_of_avg_market_price:
![Image](https://github.com/user-attachments/assets/08f39e85-f294-4e53-9a64-258120307b61)

-Step-6 : New measure was created to find total sale price and avg sale price.
	
	Total sale price= sum(sale price)
	Avg.sale price= Avg(sale price)

A card was used to represent sale price.

snap_of_total_sale_price:
![Image](https://github.com/user-attachments/assets/336d8e56-3b4f-4f2a-ab55-732a16afc360)

snap_of_avg_sale_price:
![Image](https://github.com/user-attachments/assets/8d37ab8c-53cc-4720-805f-7e1c75478091)

-Step-7 : New measure was created to find count of product type.
	
	count of product type: count(type)
	
A card was used to represent count of type.

snap_of_count type:
![Image](https://github.com/user-attachments/assets/575ed9f3-4443-443f-8706-8f7237305887)

# Snap of report:
![Image](https://github.com/user-attachments/assets/bc8fe254-7ec9-4f42-8c8c-03d7180d4b88)
