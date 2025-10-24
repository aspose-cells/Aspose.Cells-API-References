##ActiveXControlBase.ForeOleColor
ActiveXControlBase property. Gets and sets the ole color of the foreground
## ActiveXControlBase.ForeOleColor property
Gets and sets the ole color of the foreground.
```csharp
public virtual int ForeOleColor { get; set; }
```
### Remarks
Not applies to Image control.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class ActiveXControlBasePropertyForeOleColorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a CheckBox ActiveX control with all required parameters
var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 1, 100, 30, 100, 30);
CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;
// Set basic properties
checkBox.Caption = "Sample CheckBox";
checkBox.IsAutoSize = true;
// Demonstrate ForeOleColor property
checkBox.ForeOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Red);
checkBox.BackOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.LightGray);
// Save the workbook
workbook.Save("ActiveXControlForeOleColorDemo.xlsx");
}
}
}
```
### See Also
* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
