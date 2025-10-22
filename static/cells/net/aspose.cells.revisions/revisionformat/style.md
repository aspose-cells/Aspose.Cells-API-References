##RevisionFormat.Style
RevisionFormat property. Gets the applied style
## RevisionFormat.Style property
Gets the applied style.
```csharp
public Style Style { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Revisions;
using System;
public class RevisionFormatPropertyStyleDemo
{
public static void Run()
{
// Create a new workbook (revision tracking is enabled by default when changes are made)
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data and formatting to create a revision
Cell cell = worksheet.Cells["A1"];
cell.PutValue("Original Value");
// Create a style and apply it to the cell
Style originalStyle = workbook.CreateStyle();
originalStyle.Font.Name = "Arial";
originalStyle.Font.Size = 12;
originalStyle.Font.IsBold = true;
cell.SetStyle(originalStyle);
// Access the revisions through RevisionLogs
RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
foreach (RevisionLog revisionLog in revisionLogs)
{
RevisionCollection revisions = revisionLog.Revisions;
foreach (Revision revision in revisions)
{
if (revision is RevisionFormat revisionFormat)
{
// Display the current style properties from the revision
Style style = revisionFormat.Style;
Console.WriteLine("Revision Style Font: " + style.Font.Name);
Console.WriteLine("Revision Style Font Size: " + style.Font.Size);
Console.WriteLine("Revision Style Is Bold: " + style.Font.IsBold);
// Note: Style property is read-only in RevisionFormat, so we can't modify it directly
// To change formatting, we would need to modify the cell's style directly
}
}
}
// Save the workbook with revisions
workbook.Save("RevisionFormatStyleDemo.xlsx");
}
}
}
```
### See Also
* class [Style](../../../aspose.cells/style/)
* class [RevisionFormat](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)
