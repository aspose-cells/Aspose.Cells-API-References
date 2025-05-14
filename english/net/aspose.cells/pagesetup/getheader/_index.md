---
title: PageSetup.GetHeader
second_title: Aspose.Cells for .NET API Reference
description: PageSetup method. Gets a script formatting the header of an Excel file
type: docs
url: /net/aspose.cells/pagesetup/getheader/
---
## PageSetup.GetHeader method

Gets a script formatting the header of an Excel file.

```csharp
public string GetHeader(int section)
```

| Parameter | Type | Description |
| --- | --- | --- |
| section | Int32 | 0: Left Section, 1: Center Section, 2: Right Section. |

### Examples

```csharp
// Called: Assert.AreEqual(page.GetHeader(2), "&8Report ID: TEST01\n你好Public");
public void PageSetup_Method_GetHeader()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"JAVA43421/";
    string savePath = CreateFolder(filePath);

    HtmlLoadOptions htmlLoadOptions = new HtmlLoadOptions();
    Workbook wb = new Workbook(filePath + "test1.html", htmlLoadOptions);
    PageSetup page = wb.Worksheets[0].PageSetup;
    Assert.AreEqual(page.GetHeader(2), "&8Report ID: TEST01\n你好Public");
    Assert.AreEqual(page.GetFooter(0), "&8Report By: SYSTEM");
    wb.Save(savePath + "out.xlsx");
}
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


