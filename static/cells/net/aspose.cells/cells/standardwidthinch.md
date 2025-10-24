##Cells.StandardWidthInch
Cells property. Gets or sets the default column width in the worksheet in unit of inches
## Cells.StandardWidthInch property
Gets or sets the default column width in the worksheet, in unit of inches.
```csharp
public double StandardWidthInch { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsPropertyStandardWidthInchDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set standard column width in inches
worksheet.Cells.StandardWidthInch = 1.5;
// Set specific column width in inches for demonstration
worksheet.Cells.SetColumnWidthInch(1, 2.0);
// Save the workbook
workbook.Save("StandardWidthInchDemo.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
