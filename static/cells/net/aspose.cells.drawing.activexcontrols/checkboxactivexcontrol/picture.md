##CheckBoxActiveXControl.Picture
CheckBoxActiveXControl property. Gets and sets the data of the picture
## CheckBoxActiveXControl.Picture property
Gets and sets the data of the picture.
```csharp
public byte[] Picture { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing; // Added missing namespace AsposeCellsExamples
using Aspose.Cells.Drawing.ActiveXControls;
using System;
using System.IO;
public class CheckBoxActiveXControlPropertyPictureDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add CheckBox ActiveX control
Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 2, 0, 2, 0, 100, 30);
CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;
// Configure basic properties
checkBox.Caption = "Custom CheckBox";
checkBox.GroupName = "Group1";
checkBox.Value = CheckValueType.UnChecked; // Fixed enum value casing
// Display initial Picture state
Console.WriteLine("Initial Picture bytes: " + (checkBox.Picture == null ? "null" : checkBox.Picture.Length + " bytes"));
try
{
// Load image file
byte[] imageBytes = File.ReadAllBytes("checkbox_image.png");
// Set control picture and position
checkBox.Picture = imageBytes;
checkBox.PicturePosition = ControlPicturePositionType.LeftTop;
Console.WriteLine("Picture set successfully - " + checkBox.Picture.Length + " bytes");
}
catch (Exception ex)
{
Console.WriteLine("Error setting picture: " + ex.Message);
}
// Save modified workbook
workbook.Save("CheckBoxWithPicture.xlsx");
}
}
}
```
### See Also
* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
