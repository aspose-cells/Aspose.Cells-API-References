---
title: PageSetup.FitToPagesTall
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Represents the number of pages tall the worksheet will be scaled to when its printed. The default value is 1
type: docs
url: /net/aspose.cells/pagesetup/fittopagestall/
---
## PageSetup.FitToPagesTall property

Represents the number of pages tall the worksheet will be scaled to when it's printed. The default value is 1.

```csharp
public int FitToPagesTall { get; set; }
```

### Remarks

You have to set FitToPagesWide as zero if you want to fit all rows on one page.

### Examples

```csharp
// Called: Assert.AreEqual(3, setup.FitToPagesTall);
[Test]
        public void Property_FitToPagesTall()
        {
            Workbook workbook = new Workbook();
            PageSetup setup = workbook.Worksheets[0].PageSetup;
            setup.SetFitToPages(2, 3);
            Assert.IsFalse(setup.IsPercentScale);
            Assert.AreEqual(2, setup.FitToPagesWide);
            Assert.AreEqual(3, setup.FitToPagesTall);
            workbook.Save(Constants.destPath + "FitPage01.xlsx");
            workbook = new Workbook(Constants.destPath + "FitPage01.xlsx");
            setup = workbook.Worksheets[0].PageSetup;
            Assert.IsFalse(setup.IsPercentScale);
            Assert.AreEqual(2, setup.FitToPagesWide);
            Assert.AreEqual(3, setup.FitToPagesTall);
            workbook.Save(Constants.destPath + "FitPage01.xlsb");
            workbook = new Workbook(Constants.destPath + "FitPage01.xlsb");
            setup = workbook.Worksheets[0].PageSetup;
            Assert.IsFalse(setup.IsPercentScale);
            Assert.AreEqual(2, setup.FitToPagesWide);
            Assert.AreEqual(3, setup.FitToPagesTall);
            workbook.Save(Constants.destPath + "FitPage01.xls");
            workbook = new Workbook(Constants.destPath + "FitPage01.xls");
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


