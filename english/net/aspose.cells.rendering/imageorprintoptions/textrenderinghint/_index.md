---
title: ImageOrPrintOptions.TextRenderingHint
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. Specifies the quality of text rendering. The default value is TextRenderingHint.SystemDefault
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/textrenderinghint/
---
## ImageOrPrintOptions.TextRenderingHint property

Specifies the quality of text rendering. The default value is TextRenderingHint.SystemDefault

```csharp
public TextRenderingHint TextRenderingHint { get; set; }
```

### Examples

```csharp
// Called: options.ImageOptions.TextRenderingHint = System.Drawing.Text.TextRenderingHint.AntiAlias;
        public void ImageOrPrintOptions_Property_TextRenderingHint()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @"JAVA41685and41686/";
            Workbook wb = new Workbook(filePath + "aa.xlsx");
            HtmlSaveOptions options = new HtmlSaveOptions();
#if !NETCOREAPP3_1_OR_GREATER
            options.ImageOptions.TextRenderingHint = System.Drawing.Text.TextRenderingHint.AntiAlias;
#endif
            wb.Save(CreateFolder(filePath) + "out.html", options);
        }
```

### See Also

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


