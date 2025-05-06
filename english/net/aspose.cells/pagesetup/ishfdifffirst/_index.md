---
title: PageSetup.IsHFDiffFirst
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. True means that the header/footer of the first page is different with other pages
type: docs
url: /net/aspose.cells/pagesetup/ishfdifffirst/
---
## PageSetup.IsHFDiffFirst property

True means that the header/footer of the first page is different with other pages.

```csharp
public bool IsHFDiffFirst { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(ps.IsHFDiffFirst);
[Test]
        public void Property_IsHFDiffFirst()
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


