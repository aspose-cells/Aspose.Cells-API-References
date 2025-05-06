---
title: RevisionLogCollection.HighlightChanges
second_title: Aspose.Cells for .NET API Reference
description: RevisionLogCollection method. Highlights changes of shared workbook
type: docs
url: /net/aspose.cells.revisions/revisionlogcollection/highlightchanges/
---
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
// Called: workbook.Worksheets.RevisionLogs.HighlightChanges(new Aspose.Cells.Revisions.HighlightChangesOptions(true, true));
[Test]
        public void Method_HighlightChangesOptions_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSJAVA45414.xlsx&quot;);

            workbook.Worksheets.RevisionLogs.HighlightChanges(new Aspose.Cells.Revisions.HighlightChangesOptions(true, true));
            Worksheet sheet = workbook.Worksheets[workbook.Worksheets.Count - 1];
            Assert.AreEqual(&quot;18&quot;, sheet.Cells[&quot;A18&quot;].StringValue);
            workbook.Save(Constants.destPath + &quot;dest.xlsx&quot;);
        }
```

### See Also

* class [HighlightChangesOptions](../../highlightchangesoptions/)
* class [RevisionLogCollection](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


