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

### Remarks

NOTE: This member is now obsolete. Instead, please use [`FitToViewPort`](../../svgimageoptions/fittoviewport/). This property will be removed 12 months later since April 2025. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: opts.SVGFitToViewPort = true;
public void ImageOrPrintOptions_Property_SVGFitToViewPort()
{
    string filePath = Constants.PivotTableSourcePath + @"NET44262_";
    Workbook workbook = new Workbook(filePath + "Event+list+-+Generated.xlsx");

    Worksheet worksheet = workbook.Worksheets["PerMonth"];
    worksheet.Charts[0].RefreshPivotData();

    ImageOrPrintOptions opts = new ImageOrPrintOptions();
    opts.ImageType = ImageType.Svg;
    opts.OnePagePerSheet = true;
    opts.SVGFitToViewPort = true;

    SheetRender sr = new SheetRender(worksheet, opts);
    sr.ToImage(0, Constants.PivotTableDestPath + @"example.svg");
}
```

### See Also

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


