---
title: HtmlSaveOptions.ParseHtmlTagInCell
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates whether html tagsuch as div/div in cell should be parsed as cell value or preserved as it is. The default value is true
type: docs
url: /net/aspose.cells/htmlsaveoptions/parsehtmltagincell/
---
## HtmlSaveOptions.ParseHtmlTagInCell property

Indicates whether html tag(such as `<div></div>`) in cell should be parsed as cell value or preserved as it is. The default value is true.

```csharp
public bool ParseHtmlTagInCell { get; set; }
```

### Examples

```csharp
// Called: htmlSaveOptions.ParseHtmlTagInCell = true;
public void HtmlSaveOptions_Property_ParseHtmlTagInCell()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"JAVA41790/";
    Workbook workbook = new Workbook(filePath + "hyperlink_test.xlsx");
    HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions(SaveFormat.Html);
    htmlSaveOptions.ParseHtmlTagInCell = true;
    workbook.Save(CreateFolder(filePath) + "out.html", htmlSaveOptions);
}
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


