---
title: ImageOrPrintOptions.OutputBlankPageWhenNothingToPrint
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. Indicates whether to output a blank page when there is nothing to print
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/outputblankpagewhennothingtoprint/
---
## ImageOrPrintOptions.OutputBlankPageWhenNothingToPrint property

Indicates whether to output a blank page when there is nothing to print.

```csharp
public bool OutputBlankPageWhenNothingToPrint { get; set; }
```

### Remarks

Default is false.

### Examples

```csharp
// Called: options.OutputBlankPageWhenNothingToPrint = true;
[Test]
        public void Property_OutputBlankPageWhenNothingToPrint()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet477732.xlsm&quot;);
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Bmp;
            options.OutputBlankPageWhenNothingToPrint = true;

            for (int i = 0; i &lt; workbook.Worksheets.Count; i++)
            {
                if (workbook.Worksheets[i].IsVisible)
                {
                    using (Stream stream = File.Open(Path.Combine(Constants.destPath, &quot;{i}.png&quot;),
                        FileMode.OpenOrCreate, FileAccess.ReadWrite))
                    {
                        SheetRender renderer = new SheetRender(workbook.Worksheets[i], options);
                        renderer.ToImage(0, stream);
                    }
                }
            }
        }
```

### See Also

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


