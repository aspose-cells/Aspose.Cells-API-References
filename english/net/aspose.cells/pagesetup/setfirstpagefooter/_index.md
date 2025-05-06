---
title: PageSetup.SetFirstPageFooter
second_title: Aspose.Cells for .NET API Reference
description: PageSetup method. Sets a script formatting the first page footer of an Excel file
type: docs
url: /net/aspose.cells/pagesetup/setfirstpagefooter/
---
## PageSetup.SetFirstPageFooter method

Sets a script formatting the first page footer of an Excel file.

```csharp
public void SetFirstPageFooter(int section, string footerScript)
```

| Parameter | Type | Description |
| --- | --- | --- |
| section | Int32 | 0: Left Section, 1: Center Section, 2: Right Section. |
| footerScript | String | Footer format script. |

### Examples

```csharp
// Called: setup.SetFirstPageFooter(0, &amp;quot;FirstPageFooter&amp;quot;);
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


