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
// Called: saveOptions.ExportImagesAsBase64 = true;
private HtmlSaveOptions HtmlSaveOptions_Property_ExportImagesAsBase64(bool embedResources)
            {
                HtmlSaveOptions saveOptions = new HtmlSaveOptions();

                saveOptions.ExportHiddenWorksheet = false;
                saveOptions.ExportActiveWorksheetOnly = true;
                saveOptions.ExportDataOptions = HtmlExportDataOptions.All;

                if (embedResources)
                {
                    saveOptions.ExportImagesAsBase64 = true;
                }
                else
                {
                    saveOptions.StreamProvider = this;
                }

                return saveOptions;
            }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


