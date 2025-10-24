##RevisionRenameSheet.OldName
RevisionRenameSheet property. Gets the old name of the worksheet
## RevisionRenameSheet.OldName property
Gets the old name of the worksheet.
```csharp
public string OldName { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;
namespace AsposeCellsExamples
{
public class RevisionRenameSheetPropertyOldNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a worksheet and rename it to trigger a revision
Worksheet sheet = workbook.Worksheets[0];
string originalName = sheet.Name;
sheet.Name = "RenamedSheet";
// Access the revision logs
foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
{
foreach (Revision rv in log.Revisions)
{
if (rv.Type == RevisionType.RenameSheet)
{
RevisionRenameSheet rsnm = (RevisionRenameSheet)rv;
Console.WriteLine("Sheet renamed from: {0} to: {1}", rsnm.OldName, rsnm.NewName);
}
}
}
}
}
}
```
### See Also
* class [RevisionRenameSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)
