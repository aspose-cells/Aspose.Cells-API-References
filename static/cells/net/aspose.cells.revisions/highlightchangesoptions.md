##Class HighlightChangesOptions
Aspose.Cells.Revisions.HighlightChangesOptions class. Represents options of highlighting revsions or changes of shared Excel files
## HighlightChangesOptions class
Represents options of highlighting revsions or changes of shared Excel files.
```csharp
public class HighlightChangesOptions
```
## Constructors
| Name | Description |
| --- | --- |
| [HighlightChangesOptions](highlightchangesoptions/)(bool, bool) | Represents options of highlighting revsions or changes of shared Excel files. |
### Examples
```csharp
using Aspose.Cells;
using Aspose.Cells.Revisions;
using System;
namespace AsposeCellsExamples
{
public class HighlightChangesOptionsDemo
{
public static void HighlightChangesExample()
{
// Instantiate a Workbook object
Workbook workbook = new Workbook("HighlightedChangesWorkbook_original.xlsx");
// Get the revision logs
RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
// Set the number of days to preserve the history
revisionLogs.DaysPreservingHistory = 30;
// Create HighlightChangesOptions
HighlightChangesOptions options = new HighlightChangesOptions(true, true);
// Highlight changes
revisionLogs.HighlightChanges(options);
// Save the workbook with highlighted changes
workbook.Save("HighlightedChangesWorkbook.xlsx");
workbook.Save("HighlightedChangesWorkbook.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)
