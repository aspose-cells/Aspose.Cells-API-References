##Cell.IsNumericValue
Cell property. Indicates whether the value of this cell is numericint double and datetime
## Cell.IsNumericValue property
Indicates whether the value of this cell is numeric(int, double and datetime)
```csharp
public bool IsNumericValue { get; }
```
### Remarks
Also applies to formula cell to check the calculated result
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellPropertyIsNumericValueDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add different types of data to cells
Cell cell1 = worksheet.Cells["A1"];
cell1.PutValue(123.45); // Numeric value
Cell cell2 = worksheet.Cells["A2"];
cell2.PutValue("Hello World"); // String value
// Check if cells contain numeric values
Console.WriteLine("Cell A1 IsNumericValue: " + cell1.IsNumericValue);
Console.WriteLine("Cell A2 IsNumericValue: " + cell2.IsNumericValue);
// Demonstrate usage with conditional logic
if (cell1.IsNumericValue)
{
Console.WriteLine("Cell A1 contains a numeric value: " + cell1.DoubleValue);
}
if (!cell2.IsNumericValue)
{
Console.WriteLine("Cell A2 does not contain a numeric value");
}
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
