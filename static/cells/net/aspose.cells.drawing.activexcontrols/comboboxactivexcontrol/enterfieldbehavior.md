##ComboBoxActiveXControl.EnterFieldBehavior
ComboBoxActiveXControl property. Specifies selection behavior when entering the control. True specifies that the selection remains unchanged from last time the control was active. False specifies that all the text in the control will be selected when entering the control
## ComboBoxActiveXControl.EnterFieldBehavior property
Specifies selection behavior when entering the control. True specifies that the selection remains unchanged from last time the control was active. False specifies that all the text in the control will be selected when entering the control.
```csharp
public bool EnterFieldBehavior { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class ComboBoxActiveXControlPropertyEnterFieldBehaviorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add first ComboBox ActiveX Control
Shape shape1 = worksheet.Shapes.AddActiveXControl(
ControlType.ComboBox,
1, 0, 1, 0, 100, 50
);
ComboBoxActiveXControl combo1 = (ComboBoxActiveXControl)shape1.ActiveXControl;
combo1.EnterFieldBehavior = false; // Default behavior (select all text on entry)
combo1.Value = "Select Option";
combo1.BorderStyle = ControlBorderType.Single;
// Add second ComboBox ActiveX Control
Shape shape2 = worksheet.Shapes.AddActiveXControl(
ControlType.ComboBox,
1, 0, 2, 0, 100, 50
);
ComboBoxActiveXControl combo2 = (ComboBoxActiveXControl)shape2.ActiveXControl;
combo2.EnterFieldBehavior = true; // Preserve previous selection
combo2.Value = "Edit Value";
combo2.BorderStyle = ControlBorderType.Single;
// Save the workbook
workbook.Save("ComboBoxActiveXControlDemo.xlsm", SaveFormat.Xlsm);
// Verify property settings
Console.WriteLine("Combo1 EnterFieldBehavior: " + combo1.EnterFieldBehavior);
Console.WriteLine("Combo2 EnterFieldBehavior: " + combo2.EnterFieldBehavior);
}
}
}
```
### See Also
* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
