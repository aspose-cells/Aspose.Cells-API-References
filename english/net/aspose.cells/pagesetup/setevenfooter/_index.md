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
// Called: ps.SetEvenFooter(0, "EvenFooter");
public void PageSetup_Method_SetEvenFooter()
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


