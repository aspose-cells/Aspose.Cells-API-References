##Revision.Type
Revision property. Represents the type of revision
## Revision.Type property
Represents the type of revision.
```csharp
public virtual RevisionType Type { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;
namespace AsposeCellsExamples
{
public class RevisionPropertyTypeDemo
{
public static void Run()
{
Workbook wb = new Workbook("example.xlsx");
if (!wb.HasRevisions)
{
Console.WriteLine("No revisions found");
return;
}
foreach (RevisionLog log in wb.Worksheets.RevisionLogs)
{
foreach (Revision rv in log.Revisions)
{
if (rv.Type == RevisionType.ChangeCells)
{
RevisionCellChange change = (RevisionCellChange)rv;
Console.WriteLine($"Cell {change.CellName} (Row {change.Row}):");
Console.WriteLine($"Old formula: {change.OldFormula ?? "N/A"}");
}
}
}
}
}
}
```
### See Also
* enum [RevisionType](../../revisiontype/)
* class [Revision](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)
