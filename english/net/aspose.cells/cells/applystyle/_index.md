---
title: Cells.ApplyStyle
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Applies formats for a whole worksheet
type: docs
url: /net/aspose.cells/cells/applystyle/
---
## Cells.ApplyStyle method

Applies formats for a whole worksheet.

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The style object which will be applied. |
| flag | StyleFlag | Flags which indicates applied formatting properties. |

### Examples

```csharp
// Called: wb.Worksheets[0].Cells.ApplyStyle(style, flag);
public void Cells_Method_ApplyStyle()
{
    Workbook wb = new Workbook(Constants.HtmlPath + "example.xlsx");
    Style style= wb.CreateStyle();
    StyleFlag flag = new StyleFlag();
    flag.WrapText = true;
    style.IsTextWrapped=true;
    wb.Worksheets[0].Cells.ApplyStyle(style, flag);
    HtmlSaveOptions saveOptions = new HtmlSaveOptions();
    saveOptions.HideOverflowWrappedText = true;
    wb.Save(_destFilesPath + "example.html", saveOptions);
    string text = File.ReadAllText(_destFilesPath + "example.html");
    Assert.IsTrue(text.IndexOf("overflow:hidden;white-space:nowrap;'>（供来访客户推荐）注") > -1);
}
```

### See Also

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


