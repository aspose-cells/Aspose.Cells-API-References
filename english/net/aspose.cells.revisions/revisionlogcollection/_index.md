---
title: Class RevisionLogCollection
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Revisions.RevisionLogCollection class. Represents all revision logs
type: docs
url: /net/aspose.cells.revisions/revisionlogcollection/
---
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
// Called: RevisionLogCollection rlc = wb.Worksheets.RevisionLogs;
public void Revisions_Type_RevisionLogCollection()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    Assert.IsTrue(wb.HasRevisions, "Workbook.HasRevision");
    RevisionLogCollection rlc = wb.Worksheets.RevisionLogs;
    Assert.AreEqual(3, rlc.Count, "Revision logs count");
    int matched = 0;
    foreach (RevisionLog log in rlc)
    {
        RevisionCollection rvs = log.Revisions;
        foreach (Revision rv in rvs)
        {
            if (rv.Type == RevisionType.ChangeCells)
            {
                RevisionCellChange rcc = (RevisionCellChange)rv;
                string fml = rcc.OldFormula;
                if (fml != null)
                {
                    if (rcc.Row == 0)
                    {
                        Assert.AreEqual("Sheet2!A1", fml, rcc.CellName);
                        matched++;
                    }
                    else if (rcc.Row == 1)
                    {
                        Assert.AreEqual("Sheet2!#REF!", fml, rcc.CellName);
                        matched++;
                    }
                }
            }
        }
    }
    Assert.AreEqual(2, matched, "Changed formula count");
}
```

### See Also

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [RevisionLog](../revisionlog/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


