---
title: Worksheet.PageSetup
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Represents the page setup description in this sheet
type: docs
url: /net/aspose.cells/worksheet/pagesetup/
---
## Worksheet.PageSetup property

Represents the page setup description in this sheet.

```csharp
public PageSetup PageSetup { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[2].PageSetup.FirstPageNumber, 3);
[Test]
        public void Property_PageSetup()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet40345.xls");
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

* class [PageSetup](../../pagesetup/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


