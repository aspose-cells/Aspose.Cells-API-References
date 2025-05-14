---
title: PageSetup.IsAutoFirstPageNumber
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Indicates whether the first the page number is automatically assigned
type: docs
url: /net/aspose.cells/pagesetup/isautofirstpagenumber/
---
## PageSetup.IsAutoFirstPageNumber property

Indicates whether the first the page number is automatically assigned.

```csharp
public bool IsAutoFirstPageNumber { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[1].PageSetup.IsAutoFirstPageNumber, false);
public void PageSetup_Property_IsAutoFirstPageNumber()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
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


