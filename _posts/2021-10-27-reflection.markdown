issues with live process (lab 7) at port 5001
had to restart 3 times

created hendrix  college. added a majors tab to _Layout.cshtml

could not get the DbSet global change for Student to Students to work, so I had to go manually change all 8 occurrences

added s => s.Age to the OnPostAsync() method in Create.cshtml.cs on Update the Create Page of step 2

public string AgeSort { get; set; } in Index.cshtml.cs

AgeSort = sortOrder == "Age" ? "age_desc" : "Age"; in Index.cshtml.cs
case "Age":
    studentsIQ = studentsIQ.OrderByDescending(s => s.Age);
    break;
Index.cshtml: <a asp-page="./Index" asp-route-sortOrder="@Model.AgeSort">
                    @Html.DisplayNameFor(model => model.Students[0].Age)
                </a>
                had to switch order in <tbody> because column headers were off

about page at end of step 3 not appearing
