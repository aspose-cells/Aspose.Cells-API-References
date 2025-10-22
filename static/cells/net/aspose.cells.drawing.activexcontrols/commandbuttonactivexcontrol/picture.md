##CommandButtonActiveXControl.Picture
CommandButtonActiveXControl property. Gets and sets the data of the picture
## CommandButtonActiveXControl.Picture property
Gets and sets the data of the picture.
```csharp
public byte[] Picture { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class CommandButtonActiveXControlPropertyPictureDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a shape to host the ActiveX control with all required parameters
Shape shape = worksheet.Shapes.AddActiveXControl(
ControlType.CommandButton,
1,  // top row
1,  // left column
0,  // top position
0,  // left position
100, // width
30); // height
CommandButtonActiveXControl button = (CommandButtonActiveXControl)shape.ActiveXControl;
// Set properties
button.Caption = "Click Me";
button.PicturePosition = ControlPicturePositionType.AboveCenter;
// Set the picture (empty byte array represents no picture)
button.Picture = new byte[0];
// Save the workbook
workbook.Save("CommandButtonWithPicture.xlsx");
// Verify the picture property
Console.WriteLine("Picture is null: " + (button.Picture == null));
}
}
}
```
### See Also
* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
