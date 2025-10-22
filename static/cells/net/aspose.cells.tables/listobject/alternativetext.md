##ListObject.AlternativeText
ListObject property. Gets and sets the alternative text
## ListObject.AlternativeText property
Gets and sets the alternative text.
```csharp
public string AlternativeText { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class ListObjectPropertyAlternativeTextDemo
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
// Set alternative text and description
table.AlternativeText = "Test";
table.AlternativeDescription = "aSXADCS";
// Save the workbook
workbook.Save("output.xlsx");
// Reload and verify
Workbook loadedWorkbook = new Workbook("output.xlsx");
ListObject loadedTable = loadedWorkbook.Worksheets[0].ListObjects[0];
Console.WriteLine("AlternativeText: " + loadedTable.AlternativeText);
Console.WriteLine("AlternativeDescription: " + loadedTable.AlternativeDescription);
}
}
}
```
### See Also
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
