##SheetSet.Visible
SheetSet property. Gets a set with visible sheets of the workbook in their original order
## SheetSet.Visible property
Gets a set with visible sheets of the workbook in their original order.
```csharp
public static SheetSet Visible { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class SheetSetPropertyVisibleDemo
{
public static void Run()
{
// Create a new workbook with two worksheets
Workbook workbook = new Workbook();
workbook.Worksheets.Add("Sheet2");
// Hide the second worksheet
workbook.Worksheets[1].IsVisible = false;
// Set up save options to only export visible sheets
PptxSaveOptions saveOptions = new PptxSaveOptions
{
SheetSet = SheetSet.Visible
};
// Save the workbook (only visible sheet will be exported)
workbook.Save("VisibleSheetsOnly.pptx", saveOptions);
Console.WriteLine("Workbook saved with only visible sheets exported.");
}
}
}
```
### See Also
* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
