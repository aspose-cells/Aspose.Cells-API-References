---
title: HtmlSaveOptions.ExportActiveWorksheetOnly
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates if only exporting the active worksheet to html file. If true then only the active worksheet will be exported to html file If false then the whole workbook will be exported to html file. The default value is false
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportactiveworksheetonly/
---
## HtmlSaveOptions.ExportActiveWorksheetOnly property

Indicates if only exporting the active worksheet to html file. If true then only the active worksheet will be exported to html file; If false then the whole workbook will be exported to html file. The default value is false.

```csharp
public bool ExportActiveWorksheetOnly { get; set; }
```

### Examples

```csharp
// Called: options.ExportActiveWorksheetOnly = true;
[Test]
        public void Property_ExportActiveWorksheetOnly()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;JAVA42204/&quot;;
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ImageOptions.ImageType = ImageType.Png;
            options.ExportImagesAsBase64 = true;
            options.ImageOptions.Transparent = true;
            options.ExportActiveWorksheetOnly = true;

            Workbook book = new Workbook(filePath + &quot;so-copy.xls&quot;);
            book.CalculateFormula();
            book.Worksheets.ActiveSheetIndex = 1;
            book.Save(CreateFolder(filePath) + &quot;out.html&quot;, options);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


