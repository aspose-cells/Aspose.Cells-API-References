##Cells.AddRange
Cells method. Adds a range object reference to cells
## Cells.AddRange method
Adds a range object reference to cells
```csharp
public void AddRange(Range rangeObject)
```
| Parameter | Type | Description |
| --- | --- | --- |
| rangeObject | Range | The range object will be contained in the cells |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodAddRangeWithRangeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set some sample data in the range
cells["A1"].PutValue("A1");
cells["A2"].PutValue("A2");
cells["B1"].PutValue("B1");
cells["B2"].PutValue("B2");
// Create a range and add it using AddRange
Aspose.Cells.Range range = cells.CreateRange("A1", "B2");
cells.AddRange(range);
// Modify the worksheet to demonstrate range expansion
cells.InsertRow(1);
cells.InsertColumn(1);
Console.WriteLine($"Range now has {range.RowCount} rows and {range.ColumnCount} columns");
}
}
}
```
### See Also
* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
