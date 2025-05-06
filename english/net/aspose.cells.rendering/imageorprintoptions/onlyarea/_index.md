---
title: ImageOrPrintOptions.OnlyArea
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. If this property is true  one Area will be output and no scale will take effect
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/onlyarea/
---
## ImageOrPrintOptions.OnlyArea property

If this property is true , one Area will be output, and no scale will take effect.

```csharp
public bool OnlyArea { get; set; }
```

### Examples

```csharp
// Called: OnlyArea = true
[Test]
        public void Property_OnlyArea()
        {
            var workbook = new Workbook();
            workbook.Worksheets[0].PageSetup.PrintArea = &quot;A1:A1&quot;;
            workbook.Worksheets[0].Cells[&quot;A1&quot;].PutValue(&quot;&quot;);
            var test = workbook.Worksheets[0].Cells[&quot;A1&quot;].Characters(0, 0);


            var opt = new ImageOrPrintOptions
            {
                PrintingPage = PrintingPageType.IgnoreBlank,
                //ImageFormat = ImageFormat.Png,
                ImageType = ImageType.Png,
                OnePagePerSheet = true,
                OnlyArea = true
            };
            var sh1 = new SheetRender(workbook.Worksheets[0], opt);
#if !NETCOREAPP2_0
            var image = sh1.ToImage(0);
#else
            sh1.ToImage(0, Constants.destPath + &quot;CELLSNET46207.png&quot;);
#endif
        }
```

### See Also

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


