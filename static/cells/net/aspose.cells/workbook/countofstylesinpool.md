##Workbook.CountOfStylesInPool
Workbook property. Gets number of the styles in the style pool
## Workbook.CountOfStylesInPool property
Gets number of the styles in the style pool.
```csharp
public int CountOfStylesInPool { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookPropertyCountOfStylesInPoolDemo
{
public static void Run()
{
// Create a new workbook
Workbook wb = new Workbook();
// Get initial count of styles in the pool
int initialStyleCount = wb.CountOfStylesInPool;
Console.WriteLine($"Initial styles in pool: {initialStyleCount}");
// Add some styles by modifying cells
Worksheet sheet = wb.Worksheets[0];
Cells cells = sheet.Cells;
// Style 1
Style style1 = wb.CreateStyle();
style1.Font.Name = "Arial";
style1.Font.Size = 12;
cells["A1"].SetStyle(style1);
// Style 2
Style style2 = wb.CreateStyle();
style2.Font.Color = System.Drawing.Color.Red;
style2.Pattern = BackgroundType.Solid;
cells["B1"].SetStyle(style2);
// Get updated count of styles
int updatedStyleCount = wb.CountOfStylesInPool;
Console.WriteLine($"Styles after modifications: {updatedStyleCount}");
// Save to demonstrate style persistence
wb.Save("output.html", SaveFormat.Html);
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
