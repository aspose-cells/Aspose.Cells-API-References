---
title: PageSetup.GetEvenHeader
second_title: Aspose.Cells for .NET API Reference
description: PageSetup method. Gets a script formatting the even header of an Excel file
type: docs
url: /net/aspose.cells/pagesetup/getevenheader/
---
## PageSetup.GetEvenHeader method

Gets a script formatting the even header of an Excel file.

```csharp
public string GetEvenHeader(int section)
```

| Parameter | Type | Description |
| --- | --- | --- |
| section | Int32 | 0: Left Section, 1: Center Section, 2: Right Section. |

### Examples

```csharp
// Called: Assert.AreEqual(setup.GetEvenHeader(1), "EvenHeader");
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook();
            PageSetup setup = workbook.Worksheets[0].PageSetup;
            setup.SetFirstPageFooter(0, "FirstPageFooter");
            setup.IsHFDiffFirst = true;
            setup.IsHFDiffOddEven = true;
            setup.SetEvenHeader(1, "EvenHeader");
            setup.SetEvenFooter(2, "EvenFooter");
            workbook.Save(Constants.destPath + "dest.xlsx");
            workbook = new Workbook(Constants.destPath + "dest.xlsx");
            setup = workbook.Worksheets[0].PageSetup;
            Assert.AreEqual(setup.GetFirstPageFooter(0), "FirstPageFooter");
            Assert.AreEqual(setup.GetEvenHeader(1), "EvenHeader");
            Assert.AreEqual(setup.GetEvenFooter(2), "EvenFooter");
            workbook.Save(Constants.destPath + "dest.xlsb");
            workbook = new Workbook(Constants.destPath + "dest.xlsb");
            setup = workbook.Worksheets[0].PageSetup;
            Assert.AreEqual(setup.GetFirstPageFooter(0), "FirstPageFooter");
            Assert.AreEqual(setup.GetEvenHeader(1), "EvenHeader");
            Assert.AreEqual(setup.GetEvenFooter(2), "EvenFooter");
            workbook.Save(Constants.destPath + "dest.xls");
            workbook = new Workbook(Constants.destPath + "dest.xls");
            setup = workbook.Worksheets[0].PageSetup;
            Assert.IsTrue(setup.IsHFDiffFirst);
            Assert.IsTrue(setup.IsHFDiffOddEven);
            Assert.AreEqual(setup.GetFirstPageFooter(0), "FirstPageFooter");
            Assert.AreEqual(setup.GetEvenHeader(1), "EvenHeader");
            Assert.AreEqual(setup.GetEvenFooter(2), "EvenFooter");
        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


