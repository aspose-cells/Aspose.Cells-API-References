---
title: PageSetup.SetEvenFooter
second_title: Aspose.Cells for .NET API Reference
description: PageSetup method. Sets a script formatting the even page footer of an Excel file. Only effect in Excel 2007 when IsHFDiffOddEven is true
type: docs
url: /net/aspose.cells/pagesetup/setevenfooter/
---
## PageSetup.SetEvenFooter method

Sets a script formatting the even page footer of an Excel file. Only effect in Excel 2007 when IsHFDiffOddEven is true.

```csharp
public void SetEvenFooter(int section, string footerScript)
```

| Parameter | Type | Description |
| --- | --- | --- |
| section | Int32 | 0: Left Section, 1: Center Section, 2: Right Section. |
| footerScript | String | Footer format script. |

### Examples

```csharp
// Called: ps.SetEvenFooter(0, &amp;quot;EvenFooter&amp;quot;);
[Test]
        public void Method_String_()
        {
            Workbook workbook = new Workbook();
            PageSetup ps = workbook.Worksheets[0].PageSetup;
            ps.IsHFDiffFirst = true;
            ps.IsHFDiffOddEven = true;
            ps.SetEvenFooter(0, &quot;EvenFooter&quot;);
            ps.SetFooter(0, &quot;Footer&quot;);
            ps.SetFirstPageFooter(0, &quot;FirstPageFooter&quot;);
            workbook.Save(Constants.destPath + &quot;CellsJava43425.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsJava43425.xlsx&quot;);
            ps = workbook.Worksheets[0].PageSetup;
            Assert.IsTrue(ps.IsHFDiffFirst);
            Assert.IsTrue(ps.IsHFDiffOddEven);
            Assert.AreEqual(&quot;EvenFooter&quot;, ps.GetEvenFooter(0));
            Assert.AreEqual(&quot;Footer&quot;, ps.GetFooter(0));
            Assert.AreEqual(&quot;FirstPageFooter&quot;, ps.GetFirstPageFooter(0));
            Workbook tmp = new Workbook();
            tmp.Copy(workbook);
            ps = tmp.Worksheets[0].PageSetup;
            Assert.IsTrue(ps.IsHFDiffFirst);
            Assert.IsTrue(ps.IsHFDiffOddEven);
            Assert.AreEqual(&quot;EvenFooter&quot;, ps.GetEvenFooter(0));
            Assert.AreEqual(&quot;Footer&quot;, ps.GetFooter(0));
        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


