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
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSNET-47923.xlsx&quot;);

            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsx);
            saveOptions.UpdateZoom = true;

            using(MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, saveOptions);
                ms.Position = 0;

                Workbook reloadedWb = new Workbook(ms);
                Assert.AreEqual(95, reloadedWb.Worksheets[0].PageSetup.Zoom);
            }
        }
```

### See Also

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


