---
title: "Klassen FillFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.FillFormat-klass. Inkapslar objektet som representerar fyllningsformat för en form"
type: docs
url: /sv/net/aspose.cells.drawing/fillformat/
---
## FillFormat class

Inkapslar objektet som representerar fyllningsformatering för en form.

```csharp
public class FillFormat
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [FillType](../../aspose.cells.drawing/fillformat/filltype/) { get; set; } | Hämtar och anger fyllningstyp |
| [GradientColor1](../../aspose.cells.drawing/fillformat/gradientcolor1/) { get; } | Returnerar gradientfärg 1 för den angivna fyllningen. |
| [GradientColor2](../../aspose.cells.drawing/fillformat/gradientcolor2/) { get; } | Returnerar gradientfärg 2 för den angivna fyllningen. |
| [GradientColorType](../../aspose.cells.drawing/fillformat/gradientcolortype/) { get; } | Returnerar gradientfärgens typ för den angivna fyllningen. |
| [GradientDegree](../../aspose.cells.drawing/fillformat/gradientdegree/) { get; } | Returnerar gradientens grad för den angivna fyllningen. Gäller endast för Excel 2007. |
| [GradientFill](../../aspose.cells.drawing/fillformat/gradientfill/) { get; } | Hämtar [`GradientFill`](./gradientfill/) objekt. |
| [GradientStyle](../../aspose.cells.drawing/fillformat/gradientstyle/) { get; } | Returnerar gradientstilen för den angivna fyllningen. |
| [GradientVariant](../../aspose.cells.drawing/fillformat/gradientvariant/) { get; } | Returnerar gradientvarianten för den angivna fyllningen. Gäller endast för Excel 2007. |
| [ImageData](../../aspose.cells.drawing/fillformat/imagedata/) { get; set; } | Hämtar och anger bildens bilddata. |
| [Pattern](../../aspose.cells.drawing/fillformat/pattern/) { get; set; } | Representerar ett områdes displaymönster. |
| [PatternFill](../../aspose.cells.drawing/fillformat/patternfill/) { get; } | Hämtar [`PatternFill`](./patternfill/) objekt. |
| [PictureFormatType](../../aspose.cells.drawing/fillformat/pictureformattype/) { get; set; } | Hämtar och anger bildformattypen. |
| [PresetColor](../../aspose.cells.drawing/fillformat/presetcolor/) { get; } | Returnerar den förinställda gradientfärgen för den angivna fyllningen. |
| [Scale](../../aspose.cells.drawing/fillformat/scale/) { get; set; } | Hämtar och anger skalan för bildformatet. |
| [SetType](../../aspose.cells.drawing/fillformat/settype/) { get; set; } | (**Obsolete.**) Hämtar fyllformatets inställningstyp. |
| [SolidFill](../../aspose.cells.drawing/fillformat/solidfill/) { get; } | Hämtar [`SolidFill`](./solidfill/) objekt. |
| [Texture](../../aspose.cells.drawing/fillformat/texture/) { get; set; } | Representerar texturtypen för den angivna fyllningen. |
| [TextureFill](../../aspose.cells.drawing/fillformat/texturefill/) { get; } | Hämtar [`TextureFill`](./texturefill/) objektet. |
| [Transparency](../../aspose.cells.drawing/fillformat/transparency/) { get; set; } | Returnerar eller anger graden av transparens för området som ett värde från 0,0 (opak) till 1,0 (klar). |
| [Type](../../aspose.cells.drawing/fillformat/type/) { get; set; } | (**Obsolete.**) Hämtar och anger fyllningstypen. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fillformat/equals/)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/fillformat/gethashcode/)() | Hämtar hash‑koden. |
| [SetOneColorGradient](../../aspose.cells.drawing/fillformat/setonecolorgradient/)(Color, double, GradientStyleType, int) | Ställer in den angivna fyllningen till en enfärgsgradient. Gäller endast för Excel 2007. |
| [SetPresetColorGradient](../../aspose.cells.drawing/fillformat/setpresetcolorgradient/)(GradientPresetType, GradientStyleType, int) | Ställer in den angivna fyllningen till en förinställd färggradient. Gäller endast för Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient/#settwocolorgradient_1)(Color, Color, GradientStyleType, int) | Ställer in den angivna fyllningen till en tvåfärgsgradient. Gäller endast för Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient/#settwocolorgradient)(Color, double, Color, double, GradientStyleType, int) | Ställer in den angivna fyllningen till en tvåfärgsgradient. Gäller endast för Excel 2007. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassFillFormatDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");
            
            // Lägg till ett stapeldiagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Lägg till dataserier i diagrammet
            int seriesIndex = chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";
            
            // Applicera gradientfyllning på serieområdet
            chart.NSeries[seriesIndex].Area.FillFormat.SetOneColorGradient(System.Drawing.Color.Lime, 1, 
                GradientStyleType.Horizontal, 1);
            
            // Spara arbetsboken
            workbook.Save("FillFormatDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


