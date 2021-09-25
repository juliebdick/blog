# Lab 5 Reflection
discusses the assumptions you made to convert your scenario into this data modeling framework. Include with your post a discussion of the PNG exports of your Draw.io ER diagram and Vertabelo schema. Are you satisfied with your resulting data representation? What are some complications that you could encounter implementing this model?

In my ERD, the entities were the owner, site, item, customer, account, and order. I used these entities because they are nouns that have attributes and are connected to each other by relations. One owner lists zero or more items. Zero or more items get listed on one and only one site. One customer creates one account. Many accounts get registered on the one and only one site. The customer, through their account, starts zero or more orders. One customer selects zero or more items, and the one and only one site puts zero or more items on the order. The ERD below is a representation of the above narration that I made in [LucidChart](https://www.lucidchart.com/pages/).
<br>
![I made an ERD in LucidChart](/blog/images/ERD.png)
<br>
Making the ERD in Lucid Chart was straightforward and comprehendible. The relation lines were easy to change and made sense because there is only one cardinality relation on either side of the relationship diamond, resulting in two total cardinality relations between and two entities.

In my schema, I translated the chart from my ERD into tables. Each entity and relationship is represented by a table, and the table's rows are attributes with data types. Each table that was an entity has a primary key, and each table that was a relationship has two foreign keys, one for each entity it connects. Below is the schema I made in [Vertabelo](https://www.vertabelo.com/).
<br>
![I made a Schema in Vertabelo](/blog/images/SQLSchema.png)
<br>
Making the schema was much more difficult than making the ERD. I'm not sure I made the foreign keys correctly. Navigating the relationship between the relationship table and the entity table was confusing. Drawing the relationship line from the relationship to the entity (as I did in the ERD) has a different effect on the foreign keys than drawing the line from the entity to the relationship. Doing it the former way would make the foreign key appear in the entity table, so to make the foreign keys appear in the relationship table, I drew the line in the latter way. Changing the cardinalities was also more difficult than in LucidChart. There are two cardinality relations on each side of the relationship table, resulting in four cardinalities between any two entity tables. I still do not understand this.
