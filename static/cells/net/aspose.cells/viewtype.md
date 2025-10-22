##Enum ViewType
Aspose.Cells.ViewType enum. Represents the view type of the worksheet
## ViewType enumeration
Represents the view type of the worksheet.
```csharp
public enum ViewType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| NormalView | `0` |  |
| PageBreakPreview | `1` |  |
| PageLayoutView | `2` |  |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ViewTypeDemo
{
public static void ViewTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set the view type of the worksheet to PageBreakPreview
worksheet.ViewType = ViewType.PageBreakPreview;
// Save the workbook
workbook.Save("ViewTypeExample.xlsx");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
