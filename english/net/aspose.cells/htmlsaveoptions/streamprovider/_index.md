---
title: HtmlSaveOptions.StreamProvider
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Gets or sets the IStreamProvider for exporting objects
type: docs
url: /net/aspose.cells/htmlsaveoptions/streamprovider/
---
## HtmlSaveOptions.StreamProvider property

Gets or sets the IStreamProvider for exporting objects.

```csharp
public IStreamProvider StreamProvider { get; set; }
```

### Examples

```csharp
// Called: saveOptions.StreamProvider = this;
private HtmlSaveOptions Property_StreamProvider(bool embedResources)
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

* interface [IStreamProvider](../../istreamprovider/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


