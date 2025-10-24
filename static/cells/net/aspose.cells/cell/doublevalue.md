##Cell.DoubleValue
Cell property. Gets the double value contained in the cell
## Cell.DoubleValue property
Gets the double value contained in the cell.
```csharp
public double DoubleValue { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellPropertyDoubleValueDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set different value types in cells
cells["A1"].PutValue(1); // Int value
cells["A2"].PutValue(true); // Bool value
cells["A3"].PutValue("abc"); // String value
cells["A4"].PutValue(false); // Bool value
cells["A5"].PutValue(2.56); // Double value
// Demonstrate DoubleValue property
Console.WriteLine("Double value from cell A5: " + cells["A5"].DoubleValue);
// Verify other value types can be read as double
Console.WriteLine("Int as double from A1: " + cells["A1"].DoubleValue);
Console.WriteLine("Bool as double from A2: " + cells["A2"].DoubleValue);
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
