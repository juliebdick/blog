# Lab 8 Reflection

## Challenges

During this [Entity Framework Lab](https://github.com/juliebdick/csci340lab8.2), I immediately ran into issues with Visual Studios on this lab. When I tried to run the bare project, my lab 7 project would appear in the browser instead of the new project. It took me three days to figure out that the lab 7 process was live at port 5001 since I had run it the first time.

After that obstacle, it was mostly smooth sailing. The most confusing parts of the tutorial were the Create, Read, update, and Delete step and the Migrations step. These definitely became easier by the end of the tutorial, but when they were new, it took me a while to complete. Something I was unable to figure out was the DbSet global change. When we were changing "Student" to "Students," I had to manually change all eight occurrences. I am still unsure as to what I was doing wrong.

In sorting and filtering, my column headers got off. The "Age" header was over last name, and the "Last Name" header was over age. Though when I sorted by one of those headers, the table would sort by the correct corresponding column. It turned out it was simple fix by changing the order of the parameters in the Student Index.cshtml.

When I got to the end of step three, I struggled with my About page. When I clicked on it in the browser, nothing would happen. I thought when I made an About.cshtml file, the About.cshtml.cs file would automatically appear, but it did not and I made the latter file manually. I must have created the file in the wrong location because my first try, the .cshtml.cs file did not appear underneath the .cshtml file. But on my second try, I got it to work.


## Changes

I did a few things outside of the tutorial. Besides making the project with the name Hendrix College instead of Contoso University, I added a majors navigation item to _Layout.cshtml to produce a Majors tab on the site. This provides a spot for future implementation about the different majors offered at the school, and for the entire site to be specified to Hendrix. The name of the project being changed was something that appeared in every file in the project.

To add an "Age" field to the student entity, I included "s => s.Age" to the OnPostAsync() method in the Students/Create.cshtml.cs. This was done during the updating of the create page on step two.
To add "I" and "W" options to grades, I included the two letters in the Grade enum of Enrollment.cs.
I was also able to allow the table to be sorted by age as well as last name and date. To do this, I added an AgeSort string to Students/Index.cshtml.cs and included the string as one of the variables in the OnGetAsync Task.


## Concluding Thoughts

The easiest parts of the tutorial were the following steps: Read related Data, Update related Data, and Handle concurrency conflicts. These were probably the easiest because by that point in the tutorial, I was very comfortable with Visual Studios and I understood the Razor Pages lingo more. Working with multiple tables was more intriguing than working with a single table, but it was more difficult because there are many moving parts. There are multiple entities that need to be scaffolded, and many parts that need edited. This was a useful lesson because my team's final project will have 1 or more tables at all times.

I feel better now about building our final project than I did after lab 7 because I was more successful in understanding this lab and understanding Visual Studios. In this lab, we learned how to make a database by initializing the data in Visual Studios. So I am curious as to how my team will take inputted Excel files and merge them in our database because our site will receive different data every time it is used. Something else to note is that it is exciting that we were able to sort the tables in the lab with live feedback because we will need to do the same thing in our project.
