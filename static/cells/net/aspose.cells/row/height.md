##Row.Height
Row property. Gets and sets the row height in unit of Points
## Row.Height property
Gets and sets the row height in unit of Points.
```csharp
public double Height { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RowPropertyHeightDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set row height for the first row
Row row = worksheet.Cells.Rows[0];
row.Height = 30;
// Add some data to the row
worksheet.Cells["A1"].PutValue("Row with custom height");
// Verify and display the row height
Console.WriteLine("Row 1 Height: " + row.Height);
// Save the workbook
workbook.Save("RowHeightDemo.xlsx");
}
}
}
```
### See Also
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
