---
title: PageSetup.GetFirstPageFooter
second_title: Aspose.Cells for .NET API Reference
description: PageSetup method. Gets a script formatting the first page footer of an Excel file
type: docs
url: /net/aspose.cells/pagesetup/getfirstpagefooter/
---
## PageSetup.GetFirstPageFooter method

Gets a script formatting the first page footer of an Excel file.

```csharp
public string GetFirstPageFooter(int section)
```

| Parameter | Type | Description |
| --- | --- | --- |
| section | Int32 | 0: Left Section, 1: Center Section, 2: Right Section. |

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[0].PageSetup.GetFirstPageFooter(1), "first");
public void PageSetup_Method_GetFirstPageFooter()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    Assert.AreEqual(workbook.Worksheets[0].PageSetup.GetFirstPageFooter(1), "first");
    Assert.AreEqual(workbook.Worksheets[0].PageSetup.GetEvenFooter(1), "even");
    Assert.AreEqual(workbook.Worksheets[0].PageSetup.GetFooter(1), "odd");
    workbook.Save(Constants.destPath + "example.xls");
}
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


