# JPAEntityMappings3

Excersise explanation: 
4) Run the project and investigate the generated table. Explain the content of each column (especially the
DTYPE column) and how it relates to the object model.

Answer:
The table generated shows the column content of all the information in the project. It isn't generated in their own class specifik tables but takes all the classes and adds their info into one big table.
ID, DTYPE, PRICE, DISCOUNT and QUANTITYFORDISCOUNT.
DTYPE Calculates a discount from the priceitem and the quantity which means: if you buy 3 items you get a discount of 20%.

Excercise explanation:
5) What we have done so far is using the default Inheritance Strategy which is SINGLE_TABLE.
Add a @Inheritance annotation on top of the DiscountType class and select
InheritanceType.JOINED for the strategy.
Regenerate the tables and explain the purpose/content of each table and each column (especially the DTYPE
column) and how they relate to the object model.

Answer:
The customer table has the columns: ID, DTYPE, PRICE, DISCOUNT
The DiscountType table has the columns: ID, DTYPE, DISCOUNT, QUANTITYFORDISCOUNT
The DiscountQuantity table has the columns: ID, QUANTITYFORDISCOUNT
The DiscountFixed table has the columns: ID

The Customer tables purpose is to show what kind of discounttype the person has, how many items that has been bought and how expensive it is.

The DiscountType tables purpose is to find out what kind of discount the customer will get and how much the discount will be.

The DiscountQuantity tables purpose is to show the quantity of the discount.

The DiscountFixed tables purpose is to fix the discount to show the right value, though it only has an ID.
# jpamappings3
# jpamappings3
# jpamappings3
# jpamappings3
