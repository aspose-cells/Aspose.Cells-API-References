##RevisionLog.MetadataTable
RevisionLog property. Gets table that contains metadata about a list of specific changes that have taken place for this workbook
## RevisionLog.MetadataTable property
Gets table that contains metadata about a list of specific changes that have taken place for this workbook.
```csharp
public RevisionHeader MetadataTable { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;
namespace AsposeCellsExamples
{
public class RevisionLogPropertyMetadataTableDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Make some changes to create revision history
worksheet.Cells["A1"].PutValue("Original Value");
workbook.Save("RevisionDemo.xlsx", SaveFormat.Xlsx);
// Modify the cell to create a revision
worksheet.Cells["A1"].PutValue("Modified Value");
workbook.Save("RevisionDemo_modified.xlsx", SaveFormat.Xlsx);
// Reopen the modified workbook to access revision logs
workbook = new Workbook("RevisionDemo_modified.xlsx");
// Access revision logs
RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
if (revisionLogs.Count > 0)
{
RevisionLog revisionLog = revisionLogs[0];
RevisionHeader metadata = revisionLog.MetadataTable;
Console.WriteLine("Revision Metadata:");
Console.WriteLine("Saved Time: " + metadata.SavedTime);
Console.WriteLine("Modified By: " + metadata.UserName);
Console.WriteLine("Number of Revisions: " + revisionLog.Revisions.Count);
}
else
{
Console.WriteLine("No revision history found");
}
}
}
}
```
### See Also
* class [RevisionHeader](../../revisionheader/)
* class [RevisionLog](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)
