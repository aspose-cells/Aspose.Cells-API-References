---
title: PageSetup.FooterMarginInch
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Represents the distance from the bottom of the page to the footer in unit of inches
type: docs
url: /net/aspose.cells/pagesetup/footermargininch/
---
## PageSetup.FooterMarginInch property

Represents the distance from the bottom of the page to the footer, in unit of inches.

```csharp
public double FooterMarginInch { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(setup.FooterMarginInch, 0.2);
[Test]
        public void Property_FooterMarginInch()
        {
            Workbook workbook = new Workbook();
            PageSetup setup = workbook.Worksheets[0].PageSetup;
            setup.HeaderMarginInch = 0.1;
            setup.FooterMarginInch = 0.2;
            setup.TopMarginInch = 0.3;
            setup.BottomMarginInch = 0.4;
            setup.LeftMarginInch = 0.5;
            setup.RightMarginInch = 0.6;
            workbook.Save(Constants.destPath + "Margin01.xlsx");
            workbook = new Workbook(Constants.destPath + "Margin01.xlsx");
            Assert.AreEqual(setup.HeaderMarginInch, 0.1);
            Assert.AreEqual(setup.FooterMarginInch, 0.2);
            Assert.AreEqual(setup.TopMarginInch, 0.3);
            Assert.AreEqual(setup.BottomMarginInch, 0.4);
            Assert.AreEqual(setup.LeftMarginInch, 0.5);
            Assert.AreEqual(setup.RightMarginInch, 0.6);
            workbook.Save(Constants.destPath + "Margin01.xlsb");
            workbook = new Workbook(Constants.destPath + "Margin01.xlsb");
            Assert.AreEqual(setup.HeaderMarginInch, 0.1);
            Assert.AreEqual(setup.FooterMarginInch, 0.2);
            Assert.AreEqual(setup.TopMarginInch, 0.3);
            Assert.AreEqual(setup.BottomMarginInch, 0.4);
            Assert.AreEqual(setup.LeftMarginInch, 0.5);
            Assert.AreEqual(setup.RightMarginInch, 0.6);

            workbook.Save(Constants.destPath + "Margin01.xlsb");
            workbook = new Workbook(Constants.destPath + "Margin01.xlsb");
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


