##Range.Worksheet
Range property. Gets the Worksheetobject which contains this range
## Range.Worksheet property
Gets the `Worksheet`object which contains this range.
```csharp
public Worksheet Worksheet { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RangePropertyWorksheetDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Create a named range
worksheet.Cells["A1"].PutValue("Test");
worksheet.Cells["B1"].PutValue("Data");
worksheet.Cells["A2"].PutValue(10);
worksheet.Cells["B2"].PutValue(20);
// Define a named range
int index = workbook.Worksheets.Names.Add("MyRange");
Name name = workbook.Worksheets.Names[index];
name.RefersTo = "=Sheet1!$A$1:$B$2";
// Get the range by name (fully qualify Range to avoid ambiguity)
Aspose.Cells.Range range = workbook.Worksheets.GetRangeByName("MyRange");
// Demonstrate Worksheet property usage
Console.WriteLine("Range belongs to worksheet: " + range.Worksheet.Name);
// Use Worksheet property to modify cells
range.Worksheet.Cells["A1"].PutValue("Updated");
// Save the workbook
workbook.Save("RangePropertyWorksheetDemo.xlsx");
}
}
}
```
### See Also
* class [Worksheet](../../worksheet/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
