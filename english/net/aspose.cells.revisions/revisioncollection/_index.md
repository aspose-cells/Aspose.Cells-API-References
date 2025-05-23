---
title: Class RevisionCollection
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Revisions.RevisionCollection class. Represents all revision logs
type: docs
url: /net/aspose.cells.revisions/revisioncollection/
---
## RevisionCollection class

Represents all revision logs.

```csharp
public class RevisionCollection : CollectionBase<Revision>
```

## Properties

| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.revisions/revisioncollection/item/) { get; } | Gets [`Revision`](../revision/) by the index. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methods

| Name | Description |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Revision) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Revision, IComparer&lt;Revision&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Revision, IComparer&lt;Revision&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Revision) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Revision[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Revision[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Revision[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Revision&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Revision&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Revision&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Revision&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Revision&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Revision&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Revision&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Revision&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Revision&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Revision&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Revision) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Revision, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Revision, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Revision) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Revision, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Revision, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Examples

```csharp
// Called: RevisionCollection revisions = revisionLog.Revisions;
public static void Revisions_Type_RevisionCollection()
        {
            // Create a new workbook
            Workbook workbook = new Workbook("HighlightedChangesWorkbook_original.xlsx");

            // Access the revision logs of the workbook
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            // Check if there are any revision logs
            if (revisionLogs.Count > 0)
            {
                // Access the first revision log
                RevisionLog revisionLog = revisionLogs[0];

                // Access the metadata table of the revision log
                RevisionHeader metadataTable = revisionLog.MetadataTable;

                // Access the revisions in the revision log
                RevisionCollection revisions = revisionLog.Revisions;

                // Display some information about the revisions
                Console.WriteLine("Number of revisions: " + revisions.Count);
                Console.WriteLine("Metadata Table: " + metadataTable.ToString());
            }
            else
            {
                Console.WriteLine("No revision logs found.");
            }

            // Save the workbook
            workbook.Save("RevisionLogExample.xlsx");
        }
```

### See Also

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


