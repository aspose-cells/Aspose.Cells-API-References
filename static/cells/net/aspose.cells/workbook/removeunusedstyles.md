##Workbook.RemoveUnusedStyles
Workbook method. Remove all unused styles
## Workbook.RemoveUnusedStyles method
Remove all unused styles.
```csharp
public void RemoveUnusedStyles()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodRemoveUnusedStylesDemo
{
public static void Run()
{
// Create a new workbook
Workbook wb = new Workbook();
// Access first worksheet
Worksheet sheet = wb.Worksheets[0];
// Add some sample data with styles
for (int i = 0; i < 10; i++)
{
Cell cell = sheet.Cells[i, 0];
cell.PutValue("Item " + (i + 1));
// Apply different styles to cells
Style style = wb.CreateStyle();
style.Font.Name = "Arial";
style.Font.Size = 10 + i;
style.Font.IsBold = i % 2 == 0;
cell.SetStyle(style);
}
// Remove some cells to leave unused styles
sheet.Cells.DeleteRows(5, 5);
// Save before removing unused styles
wb.Save("BeforeRemoveUnusedStyles.xlsx");
// Remove unused styles
wb.RemoveUnusedStyles();
// Save after removing unused styles
wb.Save("AfterRemoveUnusedStyles.xlsx");
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
