---
title: PageSetup.SetFitToPages
second_title: Aspose.Cells for .NET API Reference
description: PageSetup method. Sets the number of pages the worksheet will be scaled to when its printed
type: docs
url: /net/aspose.cells/pagesetup/setfittopages/
---
## PageSetup.SetFitToPages method

Sets the number of pages the worksheet will be scaled to when it's printed.

```csharp
public void SetFitToPages(int wide, int tall)
```

| Parameter | Type | Description |
| --- | --- | --- |
| wide | Int32 | Pages wide. |
| tall | Int32 | Pages tall. |

### Examples

```csharp
// Called: setup.SetFitToPages(2, 3);
public void PageSetup_Method_SetFitToPages()
{
    Workbook workbook = new Workbook();
    PageSetup setup = workbook.Worksheets[0].PageSetup;
    setup.SetFitToPages(2, 3);
    Assert.IsFalse(setup.IsPercentScale);
    Assert.AreEqual(2, setup.FitToPagesWide);
    Assert.AreEqual(3, setup.FitToPagesTall);
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    setup = workbook.Worksheets[0].PageSetup;
    Assert.IsFalse(setup.IsPercentScale);
    Assert.AreEqual(2, setup.FitToPagesWide);
    Assert.AreEqual(3, setup.FitToPagesTall);
    workbook.Save(Constants.destPath + "example.xlsb");
    workbook = new Workbook(Constants.destPath + "example.xlsb");
    setup = workbook.Worksheets[0].PageSetup;
    Assert.IsFalse(setup.IsPercentScale);
    Assert.AreEqual(2, setup.FitToPagesWide);
    Assert.AreEqual(3, setup.FitToPagesTall);
    workbook.Save(Constants.destPath + "example.xls");
    workbook = new Workbook(Constants.destPath + "example.xls");
    setup = workbook.Worksheets[0].PageSetup;
    Assert.IsFalse(setup.IsPercentScale);
    Assert.AreEqual(2, setup.FitToPagesWide);
    Assert.AreEqual(3, setup.FitToPagesTall);
}
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


