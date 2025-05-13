---
title: WorksheetCollection.RevisionLogs
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection property. Represents revision logs
type: docs
url: /net/aspose.cells/worksheetcollection/revisionlogs/
---
## WorksheetCollection.RevisionLogs property

Represents revision logs.

```csharp
public RevisionLogCollection RevisionLogs { get; }
```

### Examples

```csharp
// Called: workbook.Worksheets.RevisionLogs.HighlightChanges(new Aspose.Cells.Revisions.HighlightChangesOptions(true, true));
public void WorksheetCollection_Property_RevisionLogs()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");

    workbook.Worksheets.RevisionLogs.HighlightChanges(new Aspose.Cells.Revisions.HighlightChangesOptions(true, true));
    Worksheet sheet = workbook.Worksheets[workbook.Worksheets.Count - 1];
    Assert.AreEqual("18", sheet.Cells["A18"].StringValue);
    workbook.Save(Constants.destPath + "dest.xlsx");
}
```

### See Also

* class [RevisionLogCollection](../../../aspose.cells.revisions/revisionlogcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


