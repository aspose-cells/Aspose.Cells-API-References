---
title: HtmlSaveOptions.Encoding
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. If not setuse Encoding.UTF8 as default enconding type
type: docs
url: /net/aspose.cells/htmlsaveoptions/encoding/
---
## HtmlSaveOptions.Encoding property

If not set,use Encoding.UTF8 as default enconding type.

```csharp
public Encoding Encoding { get; set; }
```

### Examples

```csharp
// Called: htmlSaveOptions.Encoding = System.Text.Encoding.Unicode;
[Test]
        public void Property_Encoding()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @"NET43884/";
            Aspose.Cells.Workbook wb = new Workbook(filePath + "2.xlsx");
            HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions();
            htmlSaveOptions.Encoding = System.Text.Encoding.Unicode;
            htmlSaveOptions.ExportDataOptions = HtmlExportDataOptions.All;
            wb.Save(CreateFolder(filePath) + "out.html", htmlSaveOptions);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


