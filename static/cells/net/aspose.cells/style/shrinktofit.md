##Style.ShrinkToFit
Style property. Represents if text automatically shrinks to fit in the available column width
## Style.ShrinkToFit property
Represents if text automatically shrinks to fit in the available column width.
```csharp
public bool ShrinkToFit { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StylePropertyShrinkToFitDemo
{
public static void Run()
{
// Create a workbook object
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Access cells collection
Cells cells = worksheet.Cells;
// Set some text in cell A1 that's longer than the column width
cells["A1"].PutValue("This is a long text that needs shrinking to fit");
// Set column width to be smaller than the text length
cells.SetColumnWidth(0, 10);
// Get the style of cell A1
Style style = cells["A1"].GetStyle();
// Set ShrinkToFit to true
style.ShrinkToFit = true;
// Apply the style to cell A1
cells["A1"].SetStyle(style);
// Save the workbook
workbook.Save("ShrinkToFitDemo.xlsx");
Console.WriteLine("ShrinkToFit demo completed successfully.");
}
}
}
```
### See Also
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
