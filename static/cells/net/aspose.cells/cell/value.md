##Cell.Value
Cell property. Gets/sets the value contained in this cell
## Cell.Value property
Gets/sets the value contained in this cell.
```csharp
public object Value { get; set; }
```
### Remarks
Possible type:
null,
Boolean,
DateTime,
Double,
Integer
String.
For int value, it may be returned as an Integer object or a Double object. And there is no guarantee that the returned value will be kept as the same type of object always.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellPropertyValueDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set values using Value property
cells[0, 0].Value = "Product ID";
cells[0, 1].Value = "Product Name";
// Demonstrate null values
cells[0, 2].Value = null;
cells[1, 0].Value = null;
cells[1, 1].Value = null;
cells[1, 2].Value = null;
// Display values
Console.WriteLine("Cell[0,0] Value: " + cells[0, 0].Value);
Console.WriteLine("Cell[0,1] Value: " + cells[0, 1].Value);
Console.WriteLine("Cell[0,2] Value: " + (cells[0, 2].Value == null ? "null" : cells[0, 2].Value));
Console.WriteLine("Cell[1,0] Value: " + (cells[1, 0].Value == null ? "null" : cells[1, 0].Value));
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
