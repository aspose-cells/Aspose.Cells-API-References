---
title: LineFormat
second_title: Aspose.Cells för .NET API-referens
description: Representerar alla inställningar för linjen.
type: docs
weight: 2220
url: /sv/net/aspose.cells.drawing/lineformat/
---
## LineFormat class

Representerar alla inställningar för linjen.

```csharp
public class LineFormat : FillFormat
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [BeginArrowheadLength](../../aspose.cells.drawing/lineformat/beginarrowheadlength) { get; set; } | Hämtar och ställer in startpilens längdtyp för linjen. |
| [BeginArrowheadStyle](../../aspose.cells.drawing/lineformat/beginarrowheadstyle) { get; set; } | Hämtar och ställer in startpiltypen för linjen. |
| [BeginArrowheadWidth](../../aspose.cells.drawing/lineformat/beginarrowheadwidth) { get; set; } | Hämtar och ställer in startpilens breddtyp för linjen. |
| [CapType](../../aspose.cells.drawing/lineformat/captype) { get; set; } | Anger slutbeteckningar. |
| [CompoundType](../../aspose.cells.drawing/lineformat/compoundtype) { get; set; } | Anger linjesammansättningstypen. |
| [DashStyle](../../aspose.cells.drawing/lineformat/dashstyle) { get; set; } | Anger linjestrecktypen. |
| [EndArrowheadLength](../../aspose.cells.drawing/lineformat/endarrowheadlength) { get; set; } | Hämtar och ställer in slutpilens längdtyp för linjen. |
| [EndArrowheadStyle](../../aspose.cells.drawing/lineformat/endarrowheadstyle) { get; set; } | Hämtar och ställer in slutpiltypen för linjen. |
| [EndArrowheadWidth](../../aspose.cells.drawing/lineformat/endarrowheadwidth) { get; set; } | Hämtar och ställer in ändpilens breddtyp för linjen. |
| [FillType](../../aspose.cells.drawing/fillformat/filltype) { get; set; } | Hämtar och ställer in fyllningstyp |
| [GradientColor1](../../aspose.cells.drawing/fillformat/gradientcolor1) { get; } | Returnerar gradientfärg 1 för den angivna fyllningen. |
| [GradientColor2](../../aspose.cells.drawing/fillformat/gradientcolor2) { get; } | Returnerar gradientfärg 2 för den angivna fyllningen. |
| [GradientColorType](../../aspose.cells.drawing/fillformat/gradientcolortype) { get; } | Returnerar gradientfärgtypen för den angivna fyllningen. |
| [GradientDegree](../../aspose.cells.drawing/fillformat/gradientdegree) { get; } | Returnerar gradientgraden för den angivna fyllningen. Gäller endast Excel 2007. |
| [GradientFill](../../aspose.cells.drawing/fillformat/gradientfill) { get; } | Blir[`GradientFill`](../fillformat/gradientfill) objekt. |
| [GradientStyle](../../aspose.cells.drawing/fillformat/gradientstyle) { get; } | Returnerar gradientstilen för den angivna fyllningen. |
| [GradientVariant](../../aspose.cells.drawing/fillformat/gradientvariant) { get; } | Returnerar gradientvarianten för den angivna fyllningen. Gäller endast Excel 2007. |
| [ImageData](../../aspose.cells.drawing/fillformat/imagedata) { get; set; } | Hämtar och ställer in bildbildsdata. |
| [JoinType](../../aspose.cells.drawing/lineformat/jointype) { get; set; } | Anger linjekopplingstypen. |
| [Pattern](../../aspose.cells.drawing/fillformat/pattern) { get; set; } | Representerar ett områdes visningsmönster. |
| [PatternFill](../../aspose.cells.drawing/fillformat/patternfill) { get; } | Blir[`PatternFill`](../fillformat/patternfill) objekt. |
| [PictureFormatType](../../aspose.cells.drawing/fillformat/pictureformattype) { get; set; } | Hämtar och ställer in bildformatstypen. |
| [PresetColor](../../aspose.cells.drawing/fillformat/presetcolor) { get; } | Returnerar den förinställda övertoningsfärgen för den angivna fyllningen. |
| [Scale](../../aspose.cells.drawing/fillformat/scale) { get; set; } | Hämtar och ställer in bildformatsskalan. |
| [SolidFill](../../aspose.cells.drawing/fillformat/solidfill) { get; } | Blir[`SolidFill`](../fillformat/solidfill) objekt. |
| [Texture](../../aspose.cells.drawing/fillformat/texture) { get; set; } | Representerar texturtypen för den angivna fyllningen. |
| [TextureFill](../../aspose.cells.drawing/fillformat/texturefill) { get; } | Blir[`TextureFill`](../fillformat/texturefill) objekt. |
| [Transparency](../../aspose.cells.drawing/fillformat/transparency) { get; set; } | Returnerar eller ställer in graden av transparens för området som ett värde från 0,0 (opak) till 1,0 (clear). |
| [Weight](../../aspose.cells.drawing/lineformat/weight) { get; set; } | Hämtar eller ställer in linjens vikt i poängenhet. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/lineformat/equals)(object) | Avgör om denna instans har samma värde som en annan specificerad[`LineFormat`](../lineformat) objekt. |
| override [GetHashCode](../../aspose.cells.drawing/lineformat/gethashcode)() | Hämtar hashkoden. |
| [SetOneColorGradient](../../aspose.cells.drawing/fillformat/setonecolorgradient)(Color, double, GradientStyleType, int) | Ställer in den angivna fyllningen till en enfärgsgradient. Gäller endast Excel 2007. |
| [SetPresetColorGradient](../../aspose.cells.drawing/fillformat/setpresetcolorgradient)(GradientPresetType, GradientStyleType, int) | Ställer in den angivna fyllningen till en förinställd färggradient. Gäller endast Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient)(Color, Color, GradientStyleType, int) | Ställer in den angivna fyllningen till en tvåfärgsgradient. Gäller endast Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient)(Color, double, Color, double, GradientStyleType, int) | Ställer in den angivna fyllningen till en tvåfärgsgradient. Gäller endast Excel 2007. |

### Exempel

```csharp

[C#]
//Instantiering av ett arbetsboksobjekt
Workbook workbook = new Workbook();
ShapeCollection shapes = workbook.Worksheets[0].Shapes;
Shape shape = shapes.AddRectangle(1, 0, 1, 0, 50, 100);
LineFormat lineFmt = shape.Line;

//gör dina affärer

```

### Se även

* class [FillFormat](../fillformat)
* namnutrymme [Aspose.Cells.Drawing](../../aspose.cells.drawing)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
