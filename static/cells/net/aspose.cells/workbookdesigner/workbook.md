##WorkbookDesigner.Workbook
WorkbookDesigner property. Gets and sets the Workbook object
## WorkbookDesigner.Workbook property
Gets and sets the `Workbook` object.
```csharp
public Workbook Workbook { get; set; }
```
### Examples
```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class Person1
{
public string Name { get; set; }
public int Age { get; set; }
public Person1(string name, int age)
{
Name = name;
Age = age;
}
}
public class WorkbookDesignerPropertyWorkbookDemo
{
public static void Run()
{
// Create a new workbook designer
WorkbookDesigner designer = new WorkbookDesigner();
// Set the workbook property with a new workbook
designer.Workbook = new Workbook();
// Add a worksheet and some template markers
Worksheet worksheet = designer.Workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("&Person.Name");
worksheet.Cells["B1"].PutValue("&Person.Age");
// Create data source
List<Person1> persons = new List<Person1>
{
new Person1("John", 25),
new Person1("Mary", 30)
};
// Set data source and process
designer.SetDataSource("Person", persons);
designer.Process();
// Output results
Console.WriteLine("A2: " + worksheet.Cells["A2"].StringValue); // Should output "John"
Console.WriteLine("B2: " + worksheet.Cells["B2"].IntValue);   // Should output 25
Console.WriteLine("A3: " + worksheet.Cells["A3"].StringValue); // Should output "Mary"
Console.WriteLine("B3: " + worksheet.Cells["B3"].IntValue);   // Should output 30
// Save the workbook
designer.Workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Workbook](../../workbook/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
