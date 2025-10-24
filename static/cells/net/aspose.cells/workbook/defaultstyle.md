##Workbook.DefaultStyle
Workbook property. Gets or sets the default Style object of the workbook
## Workbook.DefaultStyle property
Gets or sets the default [`Style`](../../style/) object of the workbook.
```csharp
public Style DefaultStyle { get; set; }
```
### Remarks
The DefaultStyle property is useful to implement a Style for the whole Workbook.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookPropertyDefaultStyleDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
// Get the default style and modify its font
Style defaultStyle = workbook.DefaultStyle;
defaultStyle.Font.Name = "Tahoma";
defaultStyle.Font.Size = 12;
// Apply the modified style back as default
workbook.DefaultStyle = defaultStyle;
// Create a worksheet and add some text with default style
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("This text uses the default Tahoma font");
// Save the workbook
workbook.Save("DefaultStyleDemo.xlsx");
}
}
}
```
### See Also
* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
