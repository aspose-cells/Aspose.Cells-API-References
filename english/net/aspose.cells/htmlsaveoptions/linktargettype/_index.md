---
title: HtmlSaveOptions.LinkTargetType
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicating the type of target attribute in a link. The default value is HtmlLinkTargetType.Parent
type: docs
url: /net/aspose.cells/htmlsaveoptions/linktargettype/
---
## HtmlSaveOptions.LinkTargetType property

Indicating the type of target attribute in `<a>` link. The default value is HtmlLinkTargetType.Parent.

```csharp
public HtmlLinkTargetType LinkTargetType { get; set; }
```

### Examples

```csharp
// Called: htmlSaveOptions.LinkTargetType = HtmlLinkTargetType.Blank;
public void HtmlSaveOptions_Property_LinkTargetType()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"NET43905/";
    Aspose.Cells.Workbook wb = new Workbook(filePath + "2.xlsx");
    HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions();
    htmlSaveOptions.Encoding = System.Text.Encoding.Unicode;
    htmlSaveOptions.ExportDataOptions = HtmlExportDataOptions.All;

    htmlSaveOptions.LinkTargetType = HtmlLinkTargetType.Blank;
    wb.Save(CreateFolder(filePath) + "out.html", htmlSaveOptions);
}
```

### See Also

* enum [HtmlLinkTargetType](../../htmllinktargettype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


