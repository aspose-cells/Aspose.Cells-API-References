##WorkbookDesigner.ClearDataSource
WorkbookDesigner method. Clears all data sources
## WorkbookDesigner.ClearDataSource method
Clears all data sources.
```csharp
public void ClearDataSource()
```
### Examples
```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class Person
{
public string Name { get; set; }
public int Age { get; set; }
public Person(string name, int age)
{
Name = name;
Age = age;
}
}
public class WorkbookDesignerMethodClearDataSourceDemo
{
public static void Run()
{
WorkbookDesigner designer = new WorkbookDesigner();
Worksheet worksheet = designer.Workbook.Worksheets[0];
// Create sample data
List<Person> persons = new List<Person>
{
new Person("John", 30),
new Person("Mary", 25),
new Person("Peter", 35)
};
// Set up smart markers
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("&=Person.Name");
worksheet.Cells["B2"].PutValue("&=Person.Age");
// First data binding
designer.SetDataSource("Person", persons);
designer.Process();
// Clear data source and rebind
designer.ClearDataSource();
designer.SetDataSource("Person", persons);
designer.Process();
// Save the result
designer.Workbook.Save("ClearedDataSourceOutput.xlsx");
}
}
}
```
### See Also
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
