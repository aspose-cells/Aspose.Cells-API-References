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
// Called: options.ExportImagesAsBase64 = false;
[Test]
        public void Property_ExportImagesAsBase64()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @"JAVA42849/";

            HtmlSaveOptions options = new HtmlSaveOptions(SaveFormat.Html);
            options.DisableDownlevelRevealedComments = true;
            options.ExcludeUnusedStyles = true;
            options.ExportActiveWorksheetOnly = true;
            options.ExportDocumentProperties = false;
            options.ExportFrameScriptsAndProperties = false;
            options.ExportImagesAsBase64 = false;
            options.ExportPrintAreaOnly = true;
            options.ExportSimilarBorderStyle = true;
            options.ExportWorkbookProperties = false;
            options.ExportWorksheetCSSSeparately = false;
            options.ExportWorksheetProperties = false;
            options.ParseHtmlTagInCell = true;
            options.HtmlCrossStringType = HtmlCrossType.FitToCell;

            Workbook wb = new Workbook(filePath + "AXDI_Restricted_Test.xlsx");
            wb.Save(CreateFolder(filePath) + "out.html");
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


