---
title: ImageOrPrintOptions.ImageOrPrintOptions
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions constructor. Ctor
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/imageorprintoptions/
---
## ImageOrPrintOptions constructor

Ctor.

```csharp
public ImageOrPrintOptions()
```

### Examples

```csharp
// Called: ImageOrPrintOptions saveOptions = new ImageOrPrintOptions();
[Test, ExpectedException(typeof(CellsException))]
#endif
        public void ImageOrPrintOptions_Constructor()
        {
            Workbook workbook = new Workbook(Constants.TemplatePath + &quot;CELLSNET-47963.xlsb&quot;);

            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.PageSetup.PrintArea = &quot;A41:I80&quot;;

            ImageOrPrintOptions saveOptions = new ImageOrPrintOptions();
            saveOptions.OnePagePerSheet = true;
            saveOptions.ImageType = ImageType.Png;

            SheetRender sheetRenderer = new SheetRender(worksheet, saveOptions);

            sheetRenderer.ToImage(0, new MemoryStream());
        }
```

### See Also

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


