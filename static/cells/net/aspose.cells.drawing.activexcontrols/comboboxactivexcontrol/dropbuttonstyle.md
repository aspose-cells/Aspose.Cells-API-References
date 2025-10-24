##ComboBoxActiveXControl.DropButtonStyle
ComboBoxActiveXControl property. Specifies the symbol displayed on the drop button
## ComboBoxActiveXControl.DropButtonStyle property
Specifies the symbol displayed on the drop button
```csharp
public DropButtonStyle DropButtonStyle { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ComboBoxActiveXControlPropertyDropButtonStyleDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;
comboBox.DropButtonStyle = Aspose.Cells.Drawing.ActiveXControls.DropButtonStyle.Ellipsis;
comboBox.ListFillRange = "A1:A3";
worksheet.Cells["A1"].PutValue("Option 1");
worksheet.Cells["A2"].PutValue("Option 2");
worksheet.Cells["A3"].PutValue("Option 3");
Console.WriteLine("DropButtonStyle: " + comboBox.DropButtonStyle);
workbook.Save("ComboBoxDropButtonStyleDemo.xlsx");
}
}
}
```
### See Also
* enum [DropButtonStyle](../../dropbuttonstyle/)
* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
