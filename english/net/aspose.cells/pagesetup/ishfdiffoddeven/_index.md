---
title: PageSetup.IsHFDiffOddEven
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. True means that the header/footer of the odd pages is different with odd pages
type: docs
url: /net/aspose.cells/pagesetup/ishfdiffoddeven/
---
## PageSetup.IsHFDiffOddEven property

True means that the header/footer of the odd pages is different with odd pages.

```csharp
public bool IsHFDiffOddEven { get; set; }
```

### Examples

```csharp
// Called: ps.IsHFDiffOddEven = true;
public void PageSetup_Property_IsHFDiffOddEven()
{
    Workbook workbook = new Workbook();
    PageSetup ps = workbook.Worksheets[0].PageSetup;
    ps.IsHFDiffFirst = true;
    ps.IsHFDiffOddEven = true;
    ps.SetEvenFooter(0, "EvenFooter");
    ps.SetFooter(0, "Footer");
    ps.SetFirstPageFooter(0, "FirstPageFooter");
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    ps = workbook.Worksheets[0].PageSetup;
    Assert.IsTrue(ps.IsHFDiffFirst);
    Assert.IsTrue(ps.IsHFDiffOddEven);
    Assert.AreEqual("EvenFooter", ps.GetEvenFooter(0));
    Assert.AreEqual("Footer", ps.GetFooter(0));
    Assert.AreEqual("FirstPageFooter", ps.GetFirstPageFooter(0));
    Workbook tmp = new Workbook();
    tmp.Copy(workbook);
    ps = tmp.Worksheets[0].PageSetup;
    Assert.IsTrue(ps.IsHFDiffFirst);
    Assert.IsTrue(ps.IsHFDiffOddEven);
    Assert.AreEqual("EvenFooter", ps.GetEvenFooter(0));
    Assert.AreEqual("Footer", ps.GetFooter(0));
}
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


