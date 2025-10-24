##RevisionAutoFormat.CellArea
RevisionAutoFormat property. Gets the location where the formatting was applied
## RevisionAutoFormat.CellArea property
Gets the location where the formatting was applied.
```csharp
public CellArea CellArea { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Revisions;
using System;
public class RevisionAutoFormatPropertyCellAreaDemo
{
public static void Run()
{
// Create a new workbook with revision tracking
Workbook workbook = new Workbook();
try
{
// Access the revision logs collection
RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
// Find the first RevisionAutoFormat instance
RevisionAutoFormat revisionFormat = null;
foreach (RevisionLog revisionLog in revisionLogs)
{
foreach (Revision revision in revisionLog.Revisions)
{
if (revision is RevisionAutoFormat)
{
revisionFormat = (RevisionAutoFormat)revision;
break;
}
}
if (revisionFormat != null) break;
}
if (revisionFormat != null)
{
// Demonstrate the CellArea property (read-only)
CellArea area = revisionFormat.CellArea;
Console.WriteLine($"Formatting applied to area: StartRow={area.StartRow}, " +
$"StartColumn={area.StartColumn}, EndRow={area.EndRow}, " +
$"EndColumn={area.EndColumn}");
}
else
{
Console.WriteLine("No auto-format revisions found in the workbook");
}
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
}
}
}
```
### See Also
* struct [CellArea](../../../aspose.cells/cellarea/)
* class [RevisionAutoFormat](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)
