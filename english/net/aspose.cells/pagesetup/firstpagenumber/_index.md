---
title: PageSetup.FirstPageNumber
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Represents the first page number that will be used when this sheet is printed
type: docs
url: /net/aspose.cells/pagesetup/firstpagenumber/
---
## PageSetup.FirstPageNumber property

Represents the first page number that will be used when this sheet is printed.

```csharp
public int FirstPageNumber { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[2].PageSetup.FirstPageNumber, 3);
[Test]
        public void Property_FirstPageNumber()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet40345.xls&quot;);
            Assert.AreEqual(workbook.Worksheets[0].PageSetup.IsAutoFirstPageNumber, true);
            Assert.AreEqual(workbook.Worksheets[1].PageSetup.IsAutoFirstPageNumber, false);
            Assert.AreEqual(workbook.Worksheets[2].PageSetup.FirstPageNumber, 3);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            Assert.AreEqual(workbook.Worksheets[0].PageSetup.IsAutoFirstPageNumber, true);
            Assert.AreEqual(workbook.Worksheets[1].PageSetup.IsAutoFirstPageNumber, false);
            Assert.AreEqual(workbook.Worksheets[2].PageSetup.FirstPageNumber, 3);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            Assert.AreEqual(workbook.Worksheets[0].PageSetup.IsAutoFirstPageNumber, true);
            Assert.AreEqual(workbook.Worksheets[1].PageSetup.IsAutoFirstPageNumber, false);
            Assert.AreEqual(workbook.Worksheets[2].PageSetup.FirstPageNumber, 3);
            workbook = Util.ReSave(workbook, SaveFormat.SpreadsheetML);
            Assert.AreEqual(workbook.Worksheets[0].PageSetup.IsAutoFirstPageNumber, true);
            Assert.AreEqual(workbook.Worksheets[1].PageSetup.IsAutoFirstPageNumber, false);
            Assert.AreEqual(workbook.Worksheets[2].PageSetup.FirstPageNumber, 3);
            workbook = Util.ReSave(workbook, SaveFormat.Ods);
            Assert.AreEqual(workbook.Worksheets[0].PageSetup.IsAutoFirstPageNumber, true);
            Assert.AreEqual(workbook.Worksheets[1].PageSetup.IsAutoFirstPageNumber, false);
            Assert.AreEqual(workbook.Worksheets[2].PageSetup.FirstPageNumber, 3);
            workbook = Util.ReSave(workbook, SaveFormat.Html);
            //Assert.AreEqual(workbook.Worksheets[0].PageSetup.IsAutoFirstPageNumber, true);
            //Assert.AreEqual(workbook.Worksheets[1].PageSetup.IsAutoFirstPageNumber, false);
            //Assert.AreEqual(workbook.Worksheets[2].PageSetup.FirstPageNumber, 3);
        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


