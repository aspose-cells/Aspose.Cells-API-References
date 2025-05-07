---
title: CopyOptions.ExtendToAdjacentRange
second_title: Aspose.Cells for .NET API Reference
description: CopyOptions property. Indicates whether extend ranges when copying the range to adjacent range
type: docs
url: /net/aspose.cells/copyoptions/extendtoadjacentrange/
---
## CopyOptions.ExtendToAdjacentRange property

Indicates whether extend ranges when copying the range to adjacent range.

```csharp
public bool ExtendToAdjacentRange { get; set; }
```

### Remarks

If it's true, only extends the range of the hyperlink,not adding a new hyperlink when copying hyperlinks to adjacent rows.

### Examples

```csharp
// Called: options.ExtendToAdjacentRange = true;
[Test]
        public void Property_ExtendToAdjacentRange()
        {

            Aspose.Cells.Workbook aWkAsp = new Aspose.Cells.Workbook(Constants.sourcePath + "CellsNet45220.xls");
            Assert.AreEqual(aWkAsp.Worksheets[0].Hyperlinks.Count,2);

            aWkAsp.Worksheets[0].Cells.InsertRows(5, 1);
            aWkAsp.Worksheets[0].Cells.CopyRows(aWkAsp.Worksheets[0].Cells, 4, 5, 1);
            Assert.AreEqual(aWkAsp.Worksheets[0].Hyperlinks.Count,4);

            aWkAsp = new Aspose.Cells.Workbook(Constants.sourcePath + "CellsNet45220.xls");
            Assert.AreEqual(aWkAsp.Worksheets[0].Hyperlinks.Count, 2);
            CopyOptions options = new CopyOptions();
            options.ExtendToAdjacentRange = true;
            aWkAsp.Worksheets[0].Cells.InsertRows(5, 1);
            aWkAsp.Worksheets[0].Cells.CopyRows(aWkAsp.Worksheets[0].Cells, 4, 5, 1, options);
            Assert.AreEqual(aWkAsp.Worksheets[0].Hyperlinks.Count, 2);

        }
```

### See Also

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


