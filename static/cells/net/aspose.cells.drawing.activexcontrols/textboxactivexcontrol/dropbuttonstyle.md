##TextBoxActiveXControl.DropButtonStyle
TextBoxActiveXControl property. Specifies the symbol displayed on the drop button
## TextBoxActiveXControl.DropButtonStyle property
Specifies the symbol displayed on the drop button
```csharp
public DropButtonStyle DropButtonStyle { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class TextBoxActiveXControlPropertyDropButtonStyleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a TextBox ActiveX Control
Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddActiveXControl(
ControlType.TextBox, 1, 1, 100, 50, 100, 50);
ActiveXControl control = shape.ActiveXControl;
// Cast to TextBoxActiveXControl to access TextBox specific properties
TextBoxActiveXControl textBoxControl = (TextBoxActiveXControl)control;
// Set the DropButtonStyle property
textBoxControl.DropButtonStyle = DropButtonStyle.Arrow;
// Save the workbook
workbook.Save("TextBoxActiveXControlDropButtonStyleDemo.xlsx");
}
}
}
```
### See Also
* enum [DropButtonStyle](../../dropbuttonstyle/)
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
