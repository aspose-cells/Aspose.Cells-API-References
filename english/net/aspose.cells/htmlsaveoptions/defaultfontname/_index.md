---
title: HtmlSaveOptions.DefaultFontName
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Specify the default font name for exporting html the default font will be used when the font of style is not existing If this property is null Aspose.Cells will use universal font which have the same family with the original font the default value is null
type: docs
url: /net/aspose.cells/htmlsaveoptions/defaultfontname/
---
## HtmlSaveOptions.DefaultFontName property

Specify the default font name for exporting html, the default font will be used when the font of style is not existing, If this property is null, Aspose.Cells will use universal font which have the same family with the original font, the default value is null.

```csharp
public string DefaultFontName { get; set; }
```

### Examples

```csharp
// Called: options.DefaultFontName = "aaaaa";
[Test]
        public void Property_DefaultFontName()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @"NET44561/";
            Workbook wb = new Workbook(filePath + "a.xlsx");
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.DefaultFontName = "aaaaa";
            wb.Save(CreateFolder(filePath) + "out.html", options);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


