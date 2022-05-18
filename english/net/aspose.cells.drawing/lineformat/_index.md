---
title: LineFormat
second_title: Aspose.Cells for .NET API Reference
description: 
type: docs
weight: 2210
url: /net/aspose.cells.drawing/lineformat/
---
## LineFormat class

Represents all setting of the line.

```csharp
public class LineFormat : FillFormat
```

## Properties

| Name | Description |
| --- | --- |
| [BeginArrowheadLength](../../aspose.cells.drawing/lineformat/beginarrowheadlength) { get; set; } | Gets and sets the begin arrow length type of the line. |
| [BeginArrowheadStyle](../../aspose.cells.drawing/lineformat/beginarrowheadstyle) { get; set; } | Gets and sets the begin arrow type of the line. |
| [BeginArrowheadWidth](../../aspose.cells.drawing/lineformat/beginarrowheadwidth) { get; set; } | Gets and sets the begin arrow width type of the line. |
| [CapType](../../aspose.cells.drawing/lineformat/captype) { get; set; } | Specifies the ending caps. |
| [CompoundType](../../aspose.cells.drawing/lineformat/compoundtype) { get; set; } | Specifies the line compound type. |
| [DashStyle](../../aspose.cells.drawing/lineformat/dashstyle) { get; set; } | Specifies the line dash type. |
| [EndArrowheadLength](../../aspose.cells.drawing/lineformat/endarrowheadlength) { get; set; } | Gets and sets the end arrow length type of the line. |
| [EndArrowheadStyle](../../aspose.cells.drawing/lineformat/endarrowheadstyle) { get; set; } | Gets and sets the end arrow type of the line. |
| [EndArrowheadWidth](../../aspose.cells.drawing/lineformat/endarrowheadwidth) { get; set; } | Gets and sets the end arrow width type of the line. |
| [FillType](../../aspose.cells.drawing/fillformat/filltype) { get; set; } | Gets and sets fill type |
| [GradientColor1](../../aspose.cells.drawing/fillformat/gradientcolor1) { get; } | Returns the gradient color 1 for the specified fill. |
| [GradientColor2](../../aspose.cells.drawing/fillformat/gradientcolor2) { get; } | Returns the gradient color 2 for the specified fill. |
| [GradientColorType](../../aspose.cells.drawing/fillformat/gradientcolortype) { get; } | Returns the gradient color type for the specified fill. |
| [GradientDegree](../../aspose.cells.drawing/fillformat/gradientdegree) { get; } | Returns the gradient degree for the specified fill. Only applies for Excel 2007. |
| [GradientFill](../../aspose.cells.drawing/fillformat/gradientfill) { get; } | Gets [`GradientFill`](../fillformat/gradientfill) object. |
| [GradientStyle](../../aspose.cells.drawing/fillformat/gradientstyle) { get; } | Returns the gradient style for the specified fill. |
| [GradientVariant](../../aspose.cells.drawing/fillformat/gradientvariant) { get; } | Returns the gradient variant for the specified fill. Only applies for Excel 2007. |
| [ImageData](../../aspose.cells.drawing/fillformat/imagedata) { get; set; } | Gets and sets the picture image data. |
| [JoinType](../../aspose.cells.drawing/lineformat/jointype) { get; set; } | Specifies the line join type. |
| [Pattern](../../aspose.cells.drawing/fillformat/pattern) { get; set; } | Represents an area's display pattern. |
| [PatternFill](../../aspose.cells.drawing/fillformat/patternfill) { get; } | Gets [`PatternFill`](../fillformat/patternfill) object. |
| [PictureFormatType](../../aspose.cells.drawing/fillformat/pictureformattype) { get; set; } | Gets and sets the picture format type. |
| [PresetColor](../../aspose.cells.drawing/fillformat/presetcolor) { get; } | Returns the gradient preset color for the specified fill. |
| [Scale](../../aspose.cells.drawing/fillformat/scale) { get; set; } | Gets and sets the picture format scale. |
| [SolidFill](../../aspose.cells.drawing/fillformat/solidfill) { get; } | Gets [`SolidFill`](../fillformat/solidfill) object. |
| [Texture](../../aspose.cells.drawing/fillformat/texture) { get; set; } | Represents the texture type for the specified fill. |
| [TextureFill](../../aspose.cells.drawing/fillformat/texturefill) { get; } | Gets [`TextureFill`](../fillformat/texturefill) object. |
| [Transparency](../../aspose.cells.drawing/fillformat/transparency) { get; set; } | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [Weight](../../aspose.cells.drawing/lineformat/weight) { get; set; } | Gets or sets the weight of the line in unit of points. |

## Methods

| Name | Description |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/lineformat/equals)(object) | Determines whether this instance has the same value as another specified [`LineFormat`](../lineformat) object. |
| override [GetHashCode](../../aspose.cells.drawing/lineformat/gethashcode)() | Gets the hash code. |
| [SetOneColorGradient](../../aspose.cells.drawing/fillformat/setonecolorgradient)(Color, double, GradientStyleType, int) | Sets the specified fill to a one-color gradient. Only applies for Excel 2007. |
| [SetPresetColorGradient](../../aspose.cells.drawing/fillformat/setpresetcolorgradient)(GradientPresetType, GradientStyleType, int) | Sets the specified fill to a preset-color gradient. Only applies for Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient)(Color, Color, GradientStyleType, int) | Sets the specified fill to a two-color gradient. Only applies for Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient)(Color, double, Color, double, GradientStyleType, int) | Sets the specified fill to a two-color gradient. Only applies for Excel 2007. |

### Examples

```csharp

[C#]
//Instantiating a Workbook object
Workbook workbook = new Workbook();
ShapeCollection shapes = workbook.Worksheets[0].Shapes;
Shape shape = shapes.AddRectangle(1, 0, 1, 0, 50, 100);
LineFormat lineFmt = shape.Line;

//do your business

```

### See Also

* class [FillFormat](../fillformat)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing)
* assembly [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
