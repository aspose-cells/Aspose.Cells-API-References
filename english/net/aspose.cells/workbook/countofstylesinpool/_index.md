---
title: Workbook.CountOfStylesInPool
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Gets number of the styles in the style pool
type: docs
url: /net/aspose.cells/workbook/countofstylesinpool/
---
## Workbook.CountOfStylesInPool property

Gets number of the styles in the style pool.

```csharp
public int CountOfStylesInPool { get; }
```

### Examples

```csharp
// Called: int stylePoolCountBefore = wb.CountOfStylesInPool;
public void Workbook_Property_CountOfStylesInPool()
{
    Workbook wb = new Workbook(Constants.HtmlPath + "example.xlsm");

    int stylePoolCountBefore = wb.CountOfStylesInPool;

    wb.Save(_destFilesPath + "example.html", SaveFormat.Html);

    int stylePoolCountAfter = wb.CountOfStylesInPool;

    if (stylePoolCountAfter > stylePoolCountBefore)
    {
        string cssContent = File.ReadAllText(_destFilesPath + "CELLSNET-50951_files/stylesheet.css");
        for (int i = stylePoolCountBefore; i < stylePoolCountAfter; i++)
        {
            Assert.IsTrue(cssContent.IndexOf(".x" + i) > -1);
        }
    }

    string content = File.ReadAllText(_destFilesPath + "CELLSNET-50951_files/sheet001.htm");
    Assert.IsTrue(content.IndexOf("src=\"cid:6FF548F7-B69F-4D78-9697-B7E47F8C19E3\"") == -1);
    Assert.IsTrue(content.IndexOf("src=\"cid:BF645E31-D7AA-4CED-8BFF-0DCF91A8E3C7\"") == -1);
}
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


