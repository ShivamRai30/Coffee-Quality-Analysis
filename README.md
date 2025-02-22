# Coffee-Quality-Analysis
*The primary goal of this project is to leverage the rich dataset provided by CQI to understand the factors that contribute to coffee quality.
<br/>*By systematically evaluating various parameters such as flavor, aroma, Body, consistency etc., the project aims to identify key factors influencing coffee quality.
<br/>*This analysis will provide insights into optimizing Variety of Coffees, Processing Methods etc., and meeting consumer expectations more effectively.
## Dashboard
![Homepage](https://github.com/user-attachments/assets/c7fa6635-9fb8-4910-8df7-8c576a5632f2)
![Page 1](https://github.com/user-attachments/assets/6e6954b4-3128-4cfe-96f0-12e5da323417)
![Page 2](https://github.com/user-attachments/assets/b8b89510-f3ea-476c-b16d-c7ba286b844a)
![Page 3](https://github.com/user-attachments/assets/c4ba713f-a385-46c5-8c7d-9dad4b76d476)
![Page 4](https://github.com/user-attachments/assets/a8babcf5-621f-43c4-a038-7fe4c172c1a2)



## Business Objective & Constraints
The Coffee Quality Institute (CQI) is a non-profit organization that works to improve the quality and value of coffee worldwide. It was founded in 1996 and has its headquarters in California, USA.
CQI's mission is to promote coffee quality through a range of activities that include research, training, and certification programs. The organization works with coffee growers, processors, roasters, and other stakeholders to improve coffee quality standards, promote sustainability, and support the development of the specialty coffee industry.

## Technical Stacks: 
Excel & PowerBI

## About the Data:
The data includes a range of information on coffee production, processing, and sensory evaluation. It also contains data on coffee genetics, soil types, and other factors that can affect coffee quality.

Sensory evaluations (coffee quality scores)

<br/>* *Aroma*: Refers to the scent or fragrance of the coffee.
<br/>* *Flavor*: The flavor of coffee is evaluated based on the taste, including any sweetness, bitterness, acidity, and other flavor notes.
<br/>* *Aftertaste*: Refers to the lingering taste that remains in the mouth after swallowing the coffee.
<br/>* *Acidity*: Acidity in coffee refers to the brightness or liveliness of the taste.
<br/>* *Body*: The body of coffee refers to the thickness or viscosity of the coffee in the mouth.
<br/>* *Balance*: Balance refers to how well the different flavor components of the coffee work together.
<br/>* *Uniformity*: Uniformity refers to the consistency of the coffee from cup to cup.
<br/>* *Clean Cup*: A clean cup refers to a coffee that is free of any off-flavors or defects, such as sourness, mustiness, or staleness.
<br/>* *Sweetness*: It can be described as caramel-like, fruity, or floral, and is a desirable quality in coffee.

PLEASE NOTE: 'Total Cup Points' is literally the total of 10 features given above. There were some notebooks trying to predict the total cup points given these features. We know the exact function underlying the total cup points.

### Defects:
Defects are undesirable qualities that can occur in coffee beans during processing or storage. Defects can be categorized into two categories: Category One and Category Two defects.
Category One defects are primary defects that can be perceived through visual inspection of the coffee beans. These defects include Black beans, sour beans, insect-damaged beans, fungus-damaged beans, etc.
Category Two defects are secondary defects that are more subtle and can only be detected through tasting. These defects include Over-fermentation, staleness, rancidness, chemical taste, etc.

## Data PreProcessing
### In Power Query
<br/>1. Country Of Origin – Renamed to Country 
<br/>2. Lot Number – Converted Chinese to english 
<br/>3. Altitude – Splitted twice & created 3 columns, One delimiter column deleted, Converted datatype to number.
<br/>4. Region – Removed Empty, So 207 rows to 205. 2 Rows deleted. Replace Chinese language words to English for Consistency 
<br/>5. Number of Bags – Clear
<br/>6. Bag Weight – Extracted kg from Weight & converted to Whole Number
<br/>7. In-Country Partner – Replaced Chinese words to English 
<br/>8. Grading Date – Replaced st, th, st, nd with space, Augu to August & change type to Date. 
<br/>9. Variety – Replace blank to null, Also there were unknow & unknown rows, but from Country Taiwan only. 
<br/>10. Processing Method - Replace blank to null, 
<br/>11. Color – Replaced the text corrections 
<br/>12. Expiration : Replaced corrections & change type to Date. 
<br/>13. Remaining all the columns are clear with no errors.

## Research Questions:
<br/>1.	What are the key determinants of coffee quality as evaluated through sensory attributes such as aroma, flavor, acidity, etc.?

<br/>Obs: Aroma, flavor, Acidity, Body are the key attributes that impacts Coffee Quality much.
![Page 1](https://github.com/user-attachments/assets/b278d27c-045f-49df-b95d-fa909ac65acb)


<br/>2.	Is there a correlation between processing methods, origin regions, and coffee quality scores?

<br/>Obs: 
<br/>*The processing method impacts the coffee Bean attributes such as Acidity, Aroma, Body, Balance. 
<br/>*Regions in high Altitude specifically regions above the equator produce good quality of coffee since they receive indirect sunlight and ample amount of water which are an important contributing factor in coffee quality
![Page 2](https://github.com/user-attachments/assets/96cd1bfd-0b2a-4267-b5ba-f44f01b4e1c9)

<br/>3.	Can we identify any trends or patterns in defect occurrences and their impact on overall coffee quality?

<br/>Obs: 
<br/>*Category 2 defects are more compared to category 1 defects. 
<br/>*Washed/Wet processed beans has more defects. 
<br/>*November, April & March Graded Beans has more defects. 
<br/>*Beans with Moisture Range more than 10% has more defects.
<br/>*Occurence of defects are higher if the range of altitude is 1000 or above
![Page 3](https://github.com/user-attachments/assets/058e29db-6028-490b-a9bc-e6268352b1f9)

<br/>4.	How do different variables interact to influence the Total Cup Points, which represent an overall measure of coffee quality?

<br/>Obs: 
<br/>*The Overall Cup points of a Coffee is influenced by attributes Acidity, flavor, Aroma, Body, Balance, After taste, The increase in this attributes enhances the Coffee Quality Points.
<br/>*Beans Processed with Double Anaerobic washed, Semi washed & Honey/Mossto methods has high Cup Points.
<br/>*Castillo, Red Bourbon & Sl34+Gesha are top 3 Quality Beans when compared to Cup Points.
<br/>*Ethiopia, Tanzania, Taiwan, Gautemela, Madagasarcar are the top 5 Countries.
![Page 4](https://github.com/user-attachments/assets/9b4626fa-06dc-494e-8102-5f16737569ae)
