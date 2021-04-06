# Virtual Machine (VM) Exercises

## 1st VM Exercise

#### Dataset

- [ ] Add datasets used to the `datasets/` folder

#### Files

- [ ] **Initial**: Add file to the `exercises/`  folder with the name `ex-1-intial.twbx` or `ex-1-intial.pbix`, depending if you are auditioning for a Tableau or Power BI course.
- [ ] **Solution**: Add file to the `exercises/`  folder with the name `ex-1-sol.twbx` or `ex-1-sol.pbix`

#### Learning Objective

*Implement an iterating function to replace numeric columns with a defined measure*

#### Motivation

*In a real-world scenario it's rarely as easy to find a key performance indicator that consists of just summing a column.  Instead, it usually requires more intense calculations to calculate some KPI.  In the video we found the average discount value for each line item.  Since multiple line items can comprise an order, it's more useful to see what the average discount value is for an order itself.  In this example you will calculate this.*

#### Steps to be executed by the student (max 6)

- Create a new measure to be located in the 'Measures Table' called Average Discount per Order.
- Utilize the AVERAGEX function to calculate the discount value for each order (i.e. by grouping each Order Line Item).
- HINT: Use the VALUES expression in the table parameter to filter by the Order ID.  Then use the Sum Discounts measure for the expression.
- Place this new measure in the table and verify the values.  The average discount per order should be higher than that of the order line items.

#### End goal:

![Example 1 Demo](/exercises/example1.png "Exercise 1")

## 2nd VM Exercise

#### Dataset

- [ ] Add datasets used to the `datasets/` folder

#### Files

- [ ] **Initial**: Add file to the `exercises/`  folder with the name `ex-2-intial.twbx` or `ex-2-intial.pbix`, depending if you are auditioning for a Tableau or Power BI course.
- [ ] **Solution**: Add file to the `exercises/`  folder with the name `ex-2-sol.twbx` or `ex-2-sol.pbix`

#### Learning Objective

Further utilize iterating functions to determine the top value for a defined attribute.

#### Motivation

*Once again we are going to dive deeper into iterating functions and show their power.  As managers are curious on replicating well performers, we are going to determine what is the best performing city within each region.  Through the use of the iterating function we can determine this.*

#### Steps to be executed by the student (max 6)

- Create a new measure to be located in the 'Measures Table' called Max Sales City.
- Utilize the MAXX function to find the highest sales cumulative grouped by city for each region.
- Hint: For the table attribute use the VALUES function to group by city.  For the Expression use the predefined measure of Total Sales.
- Utilize the CALCULATE function (in conjunction with the TOPN function) to determine what city correlates to this max value.
- Add both these attributes to the sales table and verify the results using the map below.

#### End goal:

![Example 2 Demo](/exercises/example2.png "Exercise 2")

