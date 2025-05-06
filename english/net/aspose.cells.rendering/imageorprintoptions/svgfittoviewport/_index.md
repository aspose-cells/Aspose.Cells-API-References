---
title: ImageOrPrintOptions.SVGFitToViewPort
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. if this property is true the generated svg will fit to view port
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/svgfittoviewport/
---
## ImageOrPrintOptions.SVGFitToViewPort property

if this property is true, the generated svg will fit to view port.

```csharp
[Obsolete("Use SvgImageOptions.FitToViewPort property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool SVGFitToViewPort { get; set; }
```

### Examples

```csharp
// Called: opts.SVGFitToViewPort = true;
[Test]
        public void Property_SVGFitToViewPort()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET44262_&quot;;
            Workbook workbook = new Workbook(filePath + &quot;Event+list+-+Generated.xlsx&quot;);

            Worksheet worksheet = workbook.Worksheets[&quot;PerMonth&quot;];
            worksheet.Charts[0].RefreshPivotData();

            ImageOrPrintOptions opts = new ImageOrPrintOptions();
            opts.ImageType = ImageType.Svg;
            opts.OnePagePerSheet = true;
            opts.SVGFitToViewPort = true;

            SheetRender sr = new SheetRender(worksheet, opts);
            sr.ToImage(0, Constants.PivotTableDestPath + @&quot;NET44262out.svg&quot;);
        }
```

### See Also

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


