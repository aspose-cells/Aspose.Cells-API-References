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
public void RevisionLogCollection_Method_HighlightChanges()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");

    workbook.Worksheets.RevisionLogs.HighlightChanges(new Aspose.Cells.Revisions.HighlightChangesOptions(true, true));
    Worksheet sheet = workbook.Worksheets[workbook.Worksheets.Count - 1];
    Assert.AreEqual("18", sheet.Cells["A18"].StringValue);
    Cell cell = workbook.Worksheets[0].Cells["B6"];
    Style style = cell.GetStyle(false);
    Assert.IsTrue(Util.CompareColor(Color.FromArgb(255, 128, 128), style.Borders[BorderType.TopBorder].Color));
    workbook.Save(Constants.destPath + "dest.xlsx");
}
```

### See Also

* class [HighlightChangesOptions](../../highlightchangesoptions/)
* class [RevisionLogCollection](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


