---
title: HtmlSaveOptions.ExportDataOptions
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicating the rule of exporting html file data.The default value is All
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportdataoptions/
---
## HtmlSaveOptions.ExportDataOptions property

Indicating the rule of exporting html file data.The default value is All.

```csharp
public HtmlExportDataOptions ExportDataOptions { get; set; }
```

### Examples

```csharp
// Called: htmlSaveOptions.ExportDataOptions = HtmlExportDataOptions.All;
[Test]
        public void Property_ExportDataOptions()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;JAVA41323NET43639NET43645/&quot;;

            Workbook wb = new Workbook(filePath + &quot;Excel issue.xlsx&quot;);
            HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions();
            htmlSaveOptions.ExportDataOptions = HtmlExportDataOptions.All;
            wb.Save(CreateFolder(filePath) + &quot;out.html&quot;, htmlSaveOptions);
            wb.Save(CreateFolder(filePath) + &quot;out.pdf&quot;);
        }
```

### See Also

* enum [HtmlExportDataOptions](../../htmlexportdataoptions/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


