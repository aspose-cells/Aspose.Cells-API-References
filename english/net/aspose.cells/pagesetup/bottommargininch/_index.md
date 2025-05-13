---
title: PageSetup.BottomMarginInch
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Represents the size of the bottom margin in unit of inches
type: docs
url: /net/aspose.cells/pagesetup/bottommargininch/
---
## PageSetup.BottomMarginInch property

Represents the size of the bottom margin, in unit of inches.

```csharp
public double BottomMarginInch { get; set; }
```

### Examples

```csharp
// Called: setup.BottomMarginInch = 0.4;
public void PageSetup_Property_BottomMarginInch()
{
    Workbook workbook = new Workbook();
    PageSetup setup = workbook.Worksheets[0].PageSetup;
    setup.HeaderMarginInch = 0.1;
    setup.FooterMarginInch = 0.2;
    setup.TopMarginInch = 0.3;
    setup.BottomMarginInch = 0.4;
    setup.LeftMarginInch = 0.5;
    setup.RightMarginInch = 0.6;
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    Assert.AreEqual(setup.HeaderMarginInch, 0.1);
    Assert.AreEqual(setup.FooterMarginInch, 0.2);
    Assert.AreEqual(setup.TopMarginInch, 0.3);
    Assert.AreEqual(setup.BottomMarginInch, 0.4);
    Assert.AreEqual(setup.LeftMarginInch, 0.5);
    Assert.AreEqual(setup.RightMarginInch, 0.6);
    workbook.Save(Constants.destPath + "example.xlsb");
    workbook = new Workbook(Constants.destPath + "example.xlsb");
    Assert.AreEqual(setup.HeaderMarginInch, 0.1);
    Assert.AreEqual(setup.FooterMarginInch, 0.2);
    Assert.AreEqual(setup.TopMarginInch, 0.3);
    Assert.AreEqual(setup.BottomMarginInch, 0.4);
    Assert.AreEqual(setup.LeftMarginInch, 0.5);
    Assert.AreEqual(setup.RightMarginInch, 0.6);

    workbook.Save(Constants.destPath + "example.xlsb");
    workbook = new Workbook(Constants.destPath + "example.xlsb");
    Assert.AreEqual(setup.HeaderMarginInch, 0.1);
    Assert.AreEqual(setup.FooterMarginInch, 0.2);
    Assert.AreEqual(setup.TopMarginInch, 0.3);
    Assert.AreEqual(setup.BottomMarginInch, 0.4);
    Assert.AreEqual(setup.LeftMarginInch, 0.5);
    Assert.AreEqual(setup.RightMarginInch, 0.6);
}
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


