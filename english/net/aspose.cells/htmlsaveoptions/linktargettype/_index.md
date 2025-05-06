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
[Test]
        public void Property_LinkTargetType()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;NET47046/&quot;;

            Aspose.Cells.Workbook wb = new Workbook(filePath + &quot;Sample_2SpreadSheet.xlsx&quot;);

            Aspose.Cells.HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions(SaveFormat.Html);
            htmlSaveOptions.ExportWorksheetCSSSeparately = true;
            htmlSaveOptions.ExportDataOptions = HtmlExportDataOptions.All;
            htmlSaveOptions.LinkTargetType = HtmlLinkTargetType.Blank;

            wb.Save(CreateFolder(filePath) + &quot;out.html&quot;, htmlSaveOptions);
        }
```

### See Also

* enum [HtmlLinkTargetType](../../htmllinktargettype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


