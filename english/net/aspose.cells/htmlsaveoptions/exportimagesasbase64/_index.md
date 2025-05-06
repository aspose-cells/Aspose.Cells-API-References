---
title: HtmlSaveOptions.ExportImagesAsBase64
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Specifies whether images are saved in Base64 format to HTML MHTML or EPUB
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportimagesasbase64/
---
## HtmlSaveOptions.ExportImagesAsBase64 property

Specifies whether images are saved in Base64 format to HTML, MHTML or EPUB.

```csharp
public bool ExportImagesAsBase64 { get; set; }
```

### Remarks

When this property is set to true image data is exported directly on the img elements and separate files are not created.

### Examples

```csharp
// Called: ExportImagesAsBase64 = true,
[Test]
        public void Property_ExportImagesAsBase64()
        {
            Workbook workDS = new Workbook(Constants.sourcePath + &quot;CELLSNETCORE362.xlsx&quot;);
            workDS.RemoveUnusedStyles();
            var htmlSaveOptions = new HtmlSaveOptions
            {

                ExportActiveWorksheetOnly = true,
                ExportImagesAsBase64 = true,
                PresentationPreference = true,
            };
             workDS.Save(Constants.destPath + &quot;CELLSNETCORE362.html&quot;, htmlSaveOptions);
            workDS = new Workbook(Constants.destPath + &quot;CELLSNETCORE362.html&quot;);
            Cell cell = workDS.Worksheets[0].Cells[&quot;A8&quot;];
            Assert.AreEqual(cell.GetStyle().Borders[BorderType.TopBorder].LineStyle, CellBorderType.Thin);

        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


