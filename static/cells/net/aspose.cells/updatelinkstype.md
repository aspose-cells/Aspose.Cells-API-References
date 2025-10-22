##Enum UpdateLinksType
Aspose.Cells.UpdateLinksType enum. Represents how to update links to other workbooks when the workbook is opened
## UpdateLinksType enumeration
Represents how to update links to other workbooks when the workbook is opened.
```csharp
public enum UpdateLinksType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| UserSet | `0` | Prompt user to update. |
| Never | `1` | Do not update, and do not prompt user. |
| Always | `2` | Always update. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class UpdateLinksTypeDemo
{
public static void UpdateLinksTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the workbook settings
WorkbookSettings settings = workbook.Settings;
// Set the UpdateLinksType to Always update
settings.UpdateLinksType = UpdateLinksType.Always;
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("External Link Example");
worksheet.Cells["A2"].PutValue("Data");
// Save the workbook
workbook.Save("UpdateLinksTypeExample.xlsx");
// Output the current UpdateLinksType setting
Console.WriteLine("UpdateLinksType is set to: " + settings.UpdateLinksType);
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
