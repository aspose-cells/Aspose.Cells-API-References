##ListBoxActiveXControl.SpecialEffect
ListBoxActiveXControl property. Gets and sets the special effect of the control
## ListBoxActiveXControl.SpecialEffect property
Gets and sets the special effect of the control.
```csharp
public ControlSpecialEffectType SpecialEffect { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class ListBoxActiveXControlPropertySpecialEffectDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a ListBox ActiveX control
var shape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 1, 1, 100, 100, 100, 100);
ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;
// Set SpecialEffect property
listBox.SpecialEffect = ControlSpecialEffectType.Sunken;
// Verify and output the SpecialEffect value
Console.WriteLine("ListBox SpecialEffect: " + listBox.SpecialEffect);
// Save the workbook
workbook.Save("ListBoxSpecialEffectDemo.xlsx");
}
}
}
```
### See Also
* enum [ControlSpecialEffectType](../../controlspecialeffecttype/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
