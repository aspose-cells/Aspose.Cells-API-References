##Class RevisionLogCollection
Aspose.Cells.Revisions.RevisionLogCollection class. Represents all revision logs
## RevisionLogCollection class
Represents all revision logs.
```csharp
public class RevisionLogCollection : CollectionBase<RevisionLog>
```
## Properties
| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [DaysPreservingHistory](../../aspose.cells.revisions/revisionlogcollection/dayspreservinghistory/) { get; set; } | Gets and sets the number of days the spreadsheet application will keep the change history for this workbook. |
| [Item](../../aspose.cells.revisions/revisionlogcollection/item/) { get; } | Gets [`RevisionLog`](../revisionlog/) by index. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
## Methods
| Name | Description |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(RevisionLog) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(RevisionLog, IComparer&lt;RevisionLog&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, RevisionLog, IComparer&lt;RevisionLog&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(RevisionLog) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(RevisionLog[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(RevisionLog[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, RevisionLog[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;RevisionLog&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;RevisionLog&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;RevisionLog&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;RevisionLog&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;RevisionLog&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;RevisionLog&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;RevisionLog&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;RevisionLog&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;RevisionLog&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;RevisionLog&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [HighlightChanges](../../aspose.cells.revisions/revisionlogcollection/highlightchanges/)(HighlightChangesOptions) | Highlights changes of shared workbook. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(RevisionLog) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(RevisionLog, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(RevisionLog, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(RevisionLog) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(RevisionLog, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(RevisionLog, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;
namespace AsposeCellsExamples
{
public class RevisionsClassRevisionLogCollectionDemo
{
public static void Run()
{
Workbook wb = new Workbook("example.xlsx");
if (!wb.HasRevisions)
{
Console.WriteLine("Workbook has no revisions");
return;
}
RevisionLogCollection revisionLogs = wb.Worksheets.RevisionLogs;
Console.WriteLine($"Found {revisionLogs.Count} revision logs");
foreach (RevisionLog log in revisionLogs)
{
foreach (Revision revision in log.Revisions)
{
if (revision.Type == RevisionType.ChangeCells)
{
RevisionCellChange cellChange = (RevisionCellChange)revision;
Console.WriteLine($"Cell change at {cellChange.CellName} (Row {cellChange.Row})");
if (cellChange.OldFormula != null)
{
Console.WriteLine($"Old formula: {cellChange.OldFormula}");
}
}
}
}
}
}
}
```
### See Also
* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [RevisionLog](../revisionlog/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)
