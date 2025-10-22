##RevisionLogCollection.HighlightChanges
RevisionLogCollection method. Highlights changes of shared workbook
## RevisionLogCollection.HighlightChanges method
Highlights changes of shared workbook.
```csharp
public void HighlightChanges(HighlightChangesOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| options | HighlightChangesOptions | Set the options for filtering which changes should be tracked. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;
namespace AsposeCellsExamples
{
public class RevisionLogCollectionMethodHighlightChangesWithHighlightChangesOptionsDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data and revisions
worksheet.Cells["A1"].PutValue("Original Value");
worksheet.Cells["A1"].PutValue("Modified Value");
// Highlight changes with options
HighlightChangesOptions options = new HighlightChangesOptions(true, true);
workbook.Worksheets.RevisionLogs.HighlightChanges(options);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [HighlightChangesOptions](../../highlightchangesoptions/)
* class [RevisionLogCollection](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)
