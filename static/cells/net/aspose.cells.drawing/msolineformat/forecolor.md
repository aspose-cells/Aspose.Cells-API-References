##MsoLineFormat.ForeColor
MsoLineFormat property. Gets and sets the border line fore color
## MsoLineFormat.ForeColor property
Gets and sets the border line fore color.
```csharp
public Color ForeColor { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class MsoLineFormatPropertyForeColorDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 200, 100);
// Set line format properties including ForeColor
textBox.LineFormat.ForeColor = Color.Red;
textBox.LineFormat.Style = MsoLineStyle.Single;
textBox.LineFormat.IsVisible = true;
textBox.LineFormat.Weight = 2;
workbook.Save("MsoLineFormatForeColorDemo.xlsx", SaveFormat.Xlsx);
// Verify the saved color
Workbook loadedWorkbook = new Workbook("MsoLineFormatForeColorDemo.xlsx");
Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
Console.WriteLine("Line ForeColor: " + loadedShape.LineFormat.ForeColor.ToString());
}
}
}
```
### See Also
* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
