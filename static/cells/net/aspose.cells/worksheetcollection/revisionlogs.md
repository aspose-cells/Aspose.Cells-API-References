##WorksheetCollection.RevisionLogs
WorksheetCollection property. Represents revision logs
## WorksheetCollection.RevisionLogs property
Represents revision logs.
```csharp
public RevisionLogCollection RevisionLogs { get; }
```
### Examples
```csharp
using Aspose.Cells;
using Aspose.Cells.Revisions;
namespace AsposeCellsExamples
{
public class WorksheetCollectionPropertyRevisionLogsDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
workbook.Settings.Shared = true;
Worksheet sheet = workbook.Worksheets[0];
sheet.Cells["A1"].PutValue("Original");
sheet.Cells["A1"].PutValue("Revised");
workbook.Worksheets.RevisionLogs.HighlightChanges(new HighlightChangesOptions(true, true));
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [RevisionLogCollection](../../../aspose.cells.revisions/revisionlogcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
