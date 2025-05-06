---
title: PageSetup.SetEvenHeader
second_title: Aspose.Cells for .NET API Reference
description: PageSetup method. Sets a script formatting the even page header of an Excel file. Only effect in Excel 2007 when IsHFDiffOddEven is true
type: docs
url: /net/aspose.cells/pagesetup/setevenheader/
---
## PageSetup.SetEvenHeader method

Sets a script formatting the even page header of an Excel file. Only effect in Excel 2007 when IsHFDiffOddEven is true.

```csharp
public void SetEvenHeader(int section, string headerScript)
```

| Parameter | Type | Description |
| --- | --- | --- |
| section | Int32 | 0: Left Section, 1: Center Section, 2: Right Section. |
| headerScript | String | Header format script. |

### Examples

```csharp
// Called: setup.SetEvenHeader(1, &amp;quot;EvenHeader&amp;quot;);
[Test]
        public void Method_String_()
        {
            Workbook workbook = new Workbook();
            PageSetup setup = workbook.Worksheets[0].PageSetup;
            setup.SetFirstPageFooter(0, &quot;FirstPageFooter&quot;);
            setup.IsHFDiffFirst = true;
            setup.IsHFDiffOddEven = true;
            setup.SetEvenHeader(1, &quot;EvenHeader&quot;);
            setup.SetEvenFooter(2, &quot;EvenFooter&quot;);
            workbook.Save(Constants.destPath + &quot;dest.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;dest.xlsx&quot;);
            setup = workbook.Worksheets[0].PageSetup;
            Assert.AreEqual(setup.GetFirstPageFooter(0), &quot;FirstPageFooter&quot;);
            Assert.AreEqual(setup.GetEvenHeader(1), &quot;EvenHeader&quot;);
            Assert.AreEqual(setup.GetEvenFooter(2), &quot;EvenFooter&quot;);
            workbook.Save(Constants.destPath + &quot;dest.xlsb&quot;);
            workbook = new Workbook(Constants.destPath + &quot;dest.xlsb&quot;);
            setup = workbook.Worksheets[0].PageSetup;
            Assert.AreEqual(setup.GetFirstPageFooter(0), &quot;FirstPageFooter&quot;);
            Assert.AreEqual(setup.GetEvenHeader(1), &quot;EvenHeader&quot;);
            Assert.AreEqual(setup.GetEvenFooter(2), &quot;EvenFooter&quot;);
            workbook.Save(Constants.destPath + &quot;dest.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot;dest.xls&quot;);
            setup = workbook.Worksheets[0].PageSetup;
            Assert.IsTrue(setup.IsHFDiffFirst);
            Assert.IsTrue(setup.IsHFDiffOddEven);
            Assert.AreEqual(setup.GetFirstPageFooter(0), &quot;FirstPageFooter&quot;);
            Assert.AreEqual(setup.GetEvenHeader(1), &quot;EvenHeader&quot;);
            Assert.AreEqual(setup.GetEvenFooter(2), &quot;EvenFooter&quot;);
        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


