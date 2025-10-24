##RevisionInsertSheet.SheetPosition
RevisionInsertSheet property. Gets the zero based position of the new sheet in the sheet tab bar
## RevisionInsertSheet.SheetPosition property
Gets the zero based position of the new sheet in the sheet tab bar.
```csharp
public int SheetPosition { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;
namespace AsposeCellsExamples
{
public class RevisionInsertSheetPropertySheetPositionDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
workbook.Settings.Shared = true;
Worksheet insertedSheet = workbook.Worksheets.Insert(0, SheetType.Worksheet);
insertedSheet.Name = "NewSheet";
workbook.Save("revisions_sample.xlsx");
Workbook reopenedWorkbook = new Workbook("revisions_sample.xlsx");
foreach (RevisionLog log in reopenedWorkbook.Worksheets.RevisionLogs)
{
foreach (Revision revision in log.Revisions)
{
if (revision.Type == RevisionType.InsertSheet)
{
RevisionInsertSheet ris = (RevisionInsertSheet)revision;
Console.WriteLine($"Sheet Name: {ris.Name}, Position: {ris.SheetPosition}");
}
}
}
}
}
}
```
### See Also
* class [RevisionInsertSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)
