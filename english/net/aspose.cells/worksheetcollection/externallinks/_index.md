---
title: WorksheetCollection.ExternalLinks
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection property. Represents external links in a workbook
type: docs
url: /net/aspose.cells/worksheetcollection/externallinks/
---
## WorksheetCollection.ExternalLinks property

Represents external links in a workbook.

```csharp
public ExternalLinkCollection ExternalLinks { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(3, workbook.Worksheets.ExternalLinks.Count);
[Test]
	    public void Property_ExternalLinks()
	    {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Formula/CELLSNET45158.xlsm&quot;);
            Assert.AreEqual(3, workbook.Worksheets.ExternalLinks.Count);
            foreach (Worksheet worksheet in workbook.Worksheets)
            {
                foreach (Aspose.Cells.Pivot.PivotTable pivot in worksheet.PivotTables)
                {
                    pivot.ChangeDataSource(new[] { pivot.DataSource[0].Replace(&quot;TEST&quot;, &quot;ASPOSE&quot;) });
                }
            }
            Assert.AreEqual(3, workbook.Worksheets.ExternalLinks.Count);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsm);
            Assert.AreEqual(3, workbook.Worksheets.ExternalLinks.Count);
	    }
```

### See Also

* class [ExternalLinkCollection](../../externallinkcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


