##ListBoxActiveXControl.IntegralHeight
ListBoxActiveXControl property. Indicates whether the control will only show complete lines of text without showing any partial lines
## ListBoxActiveXControl.IntegralHeight property
Indicates whether the control will only show complete lines of text without showing any partial lines.
```csharp
public bool IntegralHeight { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ListBoxActiveXControlPropertyIntegralHeightDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
var shape = worksheet.Shapes.AddActiveXControl(
Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox,
10,  // left
10,  // top
200, // width
100, // height
0,   // imageWidth (required parameter)
0    // imageHeight (required parameter)
);
Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBox =
(Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;
// Demonstrate IntegralHeight property
listBox.IntegralHeight = true;
Console.WriteLine("ListBox IntegralHeight set to: " + listBox.IntegralHeight);
// Add sample items
listBox.ListFillRange = "A1:A3";
worksheet.Cells["A1"].PutValue("Apple");
worksheet.Cells["A2"].PutValue("Banana");
worksheet.Cells["A3"].PutValue("Orange");
workbook.Save("ListBoxIntegralHeightDemo.xlsx");
}
}
}
```
### See Also
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
