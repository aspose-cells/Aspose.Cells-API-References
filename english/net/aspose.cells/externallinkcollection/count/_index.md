---
title: ExternalLinkCollection.Count
second_title: Aspose.Cells for .NET API Reference
description: ExternalLinkCollection property. Gets the number of elements actually contained in the collection
type: docs
url: /net/aspose.cells/externallinkcollection/count/
---
## ExternalLinkCollection.Count property

Gets the number of elements actually contained in the collection.

```csharp
public int Count { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(3, workbook.Worksheets.ExternalLinks.Count);
	    public void ExternalLinkCollection_Property_Count()
	    {
            Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsm");
            Assert.AreEqual(3, workbook.Worksheets.ExternalLinks.Count);
            foreach (Worksheet worksheet in workbook.Worksheets)
            {
                foreach (Aspose.Cells.Pivot.PivotTable pivot in worksheet.PivotTables)
                {
                    pivot.ChangeDataSource(new[] { pivot.DataSource[0].Replace("TEST", "ASPOSE") });
                }
            }
            Assert.AreEqual(3, workbook.Worksheets.ExternalLinks.Count);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsm);
            Assert.AreEqual(3, workbook.Worksheets.ExternalLinks.Count);
	    }
```

### See Also

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


