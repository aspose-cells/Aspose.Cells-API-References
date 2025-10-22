##ListObject.TableStyleName
ListObject property. Gets and sets the table style name
## ListObject.TableStyleName property
Gets and sets the table style name.
```csharp
public string TableStyleName { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class ListObjectPropertyTableStyleNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["A3"].PutValue("Alice");
worksheet.Cells["B3"].PutValue(25);
// Create a list object/table
int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
ListObject table = worksheet.ListObjects[index];
// Set and display the table style
table.TableStyleName = "TableStyleLight15";
Console.WriteLine("Table style name: " + table.TableStyleName);
// Save the workbook
workbook.Save("TableStyleDemo.xlsx");
}
}
}
```
### See Also
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
