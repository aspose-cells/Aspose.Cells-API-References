##Cells.SetRowHeightInch
Cells method. Sets row height in unit of inches
## Cells.SetRowHeightInch method
Sets row height in unit of inches.
```csharp
public void SetRowHeightInch(int row, double inches)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index. |
| inches | Double | Number of inches. It should be between 0 and 409.5/72. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodSetRowHeightInchWithInt32DoubleDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set default style
Style style = workbook.DefaultStyle;
style.Font.Name = "Tahoma";
style.Font.Size = 16;
style.Font.IsBold = true;
workbook.DefaultStyle = style;
// Set row heights in inches
for (int i = 0; i < 10; i++)
{
cells.SetRowHeightInch(i, 0.5 + (i * 0.2)); // Demonstrates SetRowHeightInch(Int32, Double)
}
// Save the workbook
workbook.Save("RowHeightsInInches.xlsx");
Console.WriteLine("Row heights set successfully in inches.");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
