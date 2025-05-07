---
title: HtmlSaveOptions.ExportObjectListener
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Gets or sets the ExportObjectListener for exporting objects
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportobjectlistener/
---
## HtmlSaveOptions.ExportObjectListener property

Gets or sets the ExportObjectListener for exporting objects.

```csharp
[Obsolete("Use HtmlSaveOptions.IStreamProvider property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IExportObjectListener ExportObjectListener { get; set; }
```

### Remarks

NOTE: This property is now obsolete. Instead, please use HtmlSaveOptions.IStreamProvider property. This property will be removed 12 months later since August 2015. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: ExportObjectListener = new CustomExportObjectListener()
public static void Property_ExportObjectListener()
        {
            // Custom implementation of IExportObjectListener
            // Save HTML file with custom listener
            Workbook workbook = new Workbook(); // Build your workbook here
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                ExportObjectListener = new CustomExportObjectListener()
            };
            using (Stream stream = new FileStream("ExportObjectEventExample.html", FileMode.Create))
            {
                workbook.Save(stream, saveOptions); // Save the workbook to stream
            }
        }
```

### See Also

* interface [IExportObjectListener](../../iexportobjectlistener/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


