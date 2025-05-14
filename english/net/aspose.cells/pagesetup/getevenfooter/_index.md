---
title: PageSetup.GetEvenFooter
second_title: Aspose.Cells for .NET API Reference
description: PageSetup method. Gets a script formatting the even footer of an Excel file
type: docs
url: /net/aspose.cells/pagesetup/getevenfooter/
---
## PageSetup.GetEvenFooter method

Gets a script formatting the even footer of an Excel file.

```csharp
public string GetEvenFooter(int section)
```

| Parameter | Type | Description |
| --- | --- | --- |
| section | Int32 | 0: Left Section, 1: Center Section, 2: Right Section. |

### Examples

```csharp
// Called: Assert.AreEqual("EvenFooter", ps.GetEvenFooter(0));
public void PageSetup_Method_GetEvenFooter()
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


