---
title: OoxmlSaveOptions.UpdateZoom
second_title: Aspose.Cells for .NET API Reference
description: OoxmlSaveOptions property. Indicates whether update scaling factor before saving the file if the PageSetup.FitToPagesWide and PageSetup.FitToPagesTall properties control how the worksheet is scaled
type: docs
url: /net/aspose.cells/ooxmlsaveoptions/updatezoom/
---
## OoxmlSaveOptions.UpdateZoom property

Indicates whether update scaling factor before saving the file if the PageSetup.FitToPagesWide and PageSetup.FitToPagesTall properties control how the worksheet is scaled.

```csharp
public bool UpdateZoom { get; set; }
```

### Remarks

The default value is false for performance.

### Examples

```csharp
// Called: saveOptions.UpdateZoom = true;
[Test]
        public void Property_UpdateZoom()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A10"].PutValue("sdfsfd");
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.UpdateZoom = true;
            saveOptions.EnableZip64 = true;
            workbook.Save(Constants.destPath + "SaveOptions01.xlsx", saveOptions);
        }
```

### See Also

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


