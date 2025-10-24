##Cell.DateTimeValue
Cell property. Gets the DateTime value contained in the cell
## Cell.DateTimeValue property
Gets the DateTime value contained in the cell.
```csharp
public DateTime DateTimeValue { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellPropertyDateTimeValueDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set a DateTime value in cell A1
DateTime testDate = new DateTime(2023, 12, 25);
cells["A1"].PutValue(testDate);
// Format the cell to display date
Style style = cells["A1"].GetStyle();
style.Custom = "yyyy-MM-dd";
cells["A1"].SetStyle(style);
// Retrieve and verify the DateTimeValue
DateTime retrievedDate = cells["A1"].DateTimeValue;
Console.WriteLine("Original DateTime: " + testDate.ToString("yyyy-MM-dd"));
Console.WriteLine("Retrieved DateTime: " + retrievedDate.ToString("yyyy-MM-dd"));
// Set another DateTime value in cell B1
DateTime anotherDate = new DateTime(2024, 1, 1);
cells["B1"].PutValue(anotherDate);
// Display the DateTimeValue from B1
Console.WriteLine("B1 DateTime: " + cells["B1"].DateTimeValue.ToString("yyyy-MM-dd"));
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
