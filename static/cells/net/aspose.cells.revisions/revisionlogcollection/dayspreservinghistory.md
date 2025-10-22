##RevisionLogCollection.DaysPreservingHistory
RevisionLogCollection property. Gets and sets the number of days the spreadsheet application will keep the change history for this workbook
## RevisionLogCollection.DaysPreservingHistory property
Gets and sets the number of days the spreadsheet application will keep the change history for this workbook.
```csharp
public int DaysPreservingHistory { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RevisionLogCollectionPropertyDaysPreservingHistoryDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
workbook.Settings.Shared = true;
workbook.Worksheets[0].Cells["A1"].PutValue("Test Value");
// Set DaysPreservingHistory property
workbook.Worksheets.RevisionLogs.DaysPreservingHistory = 40;
string outputPath = "output_DaysPreservingHistory.xlsx";
workbook.Save(outputPath);
// Reload to verify the property
Workbook loadedWorkbook = new Workbook(outputPath);
Console.WriteLine("DaysPreservingHistory: " +
loadedWorkbook.Worksheets.RevisionLogs.DaysPreservingHistory);
}
}
}
```
### See Also
* class [RevisionLogCollection](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)
