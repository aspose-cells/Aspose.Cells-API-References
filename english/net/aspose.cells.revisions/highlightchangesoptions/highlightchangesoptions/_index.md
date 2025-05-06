---
title: HighlightChangesOptions.HighlightChangesOptions
second_title: Aspose.Cells for .NET API Reference
description: HighlightChangesOptions constructor. Represents options of highlighting revsions or changes of shared Excel files
type: docs
url: /net/aspose.cells.revisions/highlightchangesoptions/highlightchangesoptions/
---
## HighlightChangesOptions constructor

Represents options of highlighting revsions or changes of shared Excel files.

```csharp
public HighlightChangesOptions(bool highlightOnScreen, bool listOnNewSheet)
```

| Parameter | Type | Description |
| --- | --- | --- |
| highlightOnScreen | Boolean | Indicates whether highlighting changes on screen. |
| listOnNewSheet | Boolean | Indicates whether listing changes on a new worksheet. |

### Examples

```csharp
// Called: workbook.Worksheets.RevisionLogs.HighlightChanges(new Aspose.Cells.Revisions.HighlightChangesOptions(true, true));
[Test]
        public void HighlightChangesOptions_Constructor()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSJAVA45427.xlsx&quot;);

            workbook.Worksheets.RevisionLogs.HighlightChanges(new Aspose.Cells.Revisions.HighlightChangesOptions(true, true));
            Worksheet sheet = workbook.Worksheets[workbook.Worksheets.Count - 1];
            Assert.AreEqual(&quot;18&quot;, sheet.Cells[&quot;A18&quot;].StringValue);
            Cell cell = workbook.Worksheets[0].Cells[&quot;B6&quot;];
            Style style = cell.GetStyle(false);
            Assert.IsTrue(Util.CompareColor(Color.FromArgb(255, 128, 128), style.Borders[BorderType.TopBorder].Color));
            workbook.Save(Constants.destPath + &quot;dest.xlsx&quot;);
        }
```

### See Also

* class [HighlightChangesOptions](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


