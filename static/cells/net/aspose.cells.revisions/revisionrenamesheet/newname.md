##RevisionRenameSheet.NewName
RevisionRenameSheet property. Gets the new name of the worksheet
## RevisionRenameSheet.NewName property
Gets the new name of the worksheet.
```csharp
public string NewName { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;
namespace AsposeCellsExamples
{
public class RevisionRenameSheetPropertyNewNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a worksheet and rename it to trigger a revision
Worksheet sheet = workbook.Worksheets[0];
string originalName = sheet.Name;
string newName = "RenamedSheet";
sheet.Name = newName;
// Save to memory stream to generate revisions
System.IO.MemoryStream ms = new System.IO.MemoryStream();
workbook.Save(ms, SaveFormat.Xlsx);
// Reopen the workbook to access revision logs
workbook = new Workbook(ms);
// Check revision logs for rename operation
foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
{
foreach (Revision rv in log.Revisions)
{
if (rv.Type == RevisionType.RenameSheet)
{
RevisionRenameSheet renameSheet = (RevisionRenameSheet)rv;
Console.WriteLine("Sheet renamed from '{0}' to '{1}'",
renameSheet.OldName, renameSheet.NewName);
// Demonstrate NewName property usage
if (renameSheet.NewName == newName)
{
Console.WriteLine("NewName property verification successful");
}
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
