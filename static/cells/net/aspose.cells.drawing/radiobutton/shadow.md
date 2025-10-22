##RadioButton.Shadow
RadioButton property. Indicates whether the combobox has 3D shading
## RadioButton.Shadow property
Indicates whether the combobox has 3-D shading.
```csharp
public bool Shadow { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class RadioButtonPropertyShadowDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
RadioButton radio = worksheet.Shapes.AddRadioButton(0, 0, 100, 50, 0, 0);
radio.Text = "Option 1";
radio.Shadow = true;
workbook.Save("RadioButtonShadowDemo.xlsx", SaveFormat.Xlsx);
Workbook loadedWorkbook = new Workbook("RadioButtonShadowDemo.xlsx");
RadioButton loadedRadio = (RadioButton)loadedWorkbook.Worksheets[0].Shapes[0];
Console.WriteLine("Shadow visible: " + loadedRadio.Shadow);
}
}
}
```
### See Also
* class [RadioButton](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
