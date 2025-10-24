##Style.Name
Style property. Gets or sets the name of the style
## Style.Name property
Gets or sets the name of the style.
```csharp
public string Name { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class StylePropertyNameDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create and apply first named style
Style style1 = workbook.CreateStyle();
style1.Number = 7;
style1.Name = "Sales";
worksheet.Cells["A1"].SetStyle(style1);
worksheet.Cells["A1"].PutValue("Sales Data");
// Create and apply second named style
Style style2 = workbook.CreateStyle();
style2.Font.Size = 14;
style2.Font.IsBold = true;
style2.Font.IsItalic = true;
style2.Font.Color = System.Drawing.Color.Yellow;
style2.ForegroundColor = System.Drawing.Color.Blue;
style2.Pattern = BackgroundType.Solid;
style2.Name = "Header";
worksheet.Cells["B1"].SetStyle(style2);
worksheet.Cells["B1"].PutValue("Header Text");
// Save the workbook
workbook.Save("StylePropertyNameDemo.xlsx");
}
}
}
```
### See Also
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
