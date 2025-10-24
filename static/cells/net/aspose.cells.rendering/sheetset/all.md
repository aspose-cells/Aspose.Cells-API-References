##SheetSet.All
SheetSet property. Gets a set with all sheets of the workbook in their original order
## SheetSet.All property
Gets a set with all sheets of the workbook in their original order.
```csharp
public static SheetSet All { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class SheetSetPropertyAllDemo
{
public static void Run()
{
// Create a workbook with two worksheets
Workbook workbook = new Workbook();
workbook.Worksheets.Add("Sheet2");
// Set some sample data in both sheets
workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
workbook.Worksheets[1].Cells["A1"].PutValue("Sheet2 Data");
// Save all sheets to markdown
MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
saveOptions.SheetSet = SheetSet.All;
workbook.Save("output.md", saveOptions);
Console.WriteLine("All sheets saved to markdown successfully.");
}
}
}
```
### See Also
* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
