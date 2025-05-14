---
title: PageSetup.HeaderMarginInch
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Represents the distance from the top of the page to the header in unit of inches
type: docs
url: /net/aspose.cells/pagesetup/headermargininch/
---
## PageSetup.HeaderMarginInch property

Represents the distance from the top of the page to the header, in unit of inches.

```csharp
public double HeaderMarginInch { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(setup.HeaderMarginInch, 0.1);
public void PageSetup_Property_HeaderMarginInch()
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


