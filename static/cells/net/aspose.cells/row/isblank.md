##Row.IsBlank
Row property. Indicates whether the row contains any data
## Row.IsBlank property
Indicates whether the row contains any data
```csharp
public bool IsBlank { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RowPropertyIsBlankDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Get first row (initially blank)
Row row1 = worksheet.Cells.Rows[0];
Console.WriteLine("Row 1 IsBlank: " + row1.IsBlank); // True
// Add data to first row
worksheet.Cells["A1"].PutValue("Test");
Console.WriteLine("Row 1 IsBlank after adding data: " + row1.IsBlank); // False
// Create another blank row
Row row2 = worksheet.Cells.Rows[1];
Console.WriteLine("Row 2 IsBlank: " + row2.IsBlank); // True
// Compare row blank status
Console.WriteLine("Rows have same IsBlank status: " + (row1.IsBlank == row2.IsBlank)); // False
}
}
}
```
### See Also
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
