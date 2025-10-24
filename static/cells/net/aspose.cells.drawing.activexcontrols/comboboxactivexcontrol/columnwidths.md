##ComboBoxActiveXControl.ColumnWidths
ComboBoxActiveXControl property. Gets and sets the width of the column
## ComboBoxActiveXControl.ColumnWidths property
Gets and sets the width of the column.
```csharp
public double ColumnWidths { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ComboBoxActiveXControlPropertyColumnWidthsDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
var shape = worksheet.Shapes.AddActiveXControl(
Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox,
5, 0, 100, 20, 100, 20);
var comboBox = (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;
comboBox.ColumnCount = 3;
comboBox.ListRows = 5;
// Set column widths (using double value for single column width)
comboBox.ColumnWidths = 100;
// Set list items through ListFillRange
worksheet.Cells["A1"].PutValue("Product\tPrice\tStock");
worksheet.Cells["A2"].PutValue("Laptop\t$999\t50");
worksheet.Cells["A3"].PutValue("Phone\t$699\t120");
worksheet.Cells["A4"].PutValue("Tablet\t$399\t75");
comboBox.ListFillRange = "A1:A4";
workbook.Save("ComboBoxColumnWidthsDemo.xlsx");
}
}
}
```
### See Also
* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
