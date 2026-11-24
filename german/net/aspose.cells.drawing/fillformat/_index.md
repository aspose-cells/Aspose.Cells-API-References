---
title: "Klasse FillFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.FillFormat Klasse. Kapselt das Objekt, das die Füllformatierung für eine Form darstellt"
type: docs
url: /de/net/aspose.cells.drawing/fillformat/
---
## FillFormat class

Kapselt das Objekt, das die Füllformatierung für eine Form darstellt.

```csharp
public class FillFormat
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [FillType](../../aspose.cells.drawing/fillformat/filltype/) { get; set; } | Liest und setzt den Fülltyp |
| [GradientColor1](../../aspose.cells.drawing/fillformat/gradientcolor1/) { get; } | Gibt die Farbverlauffarbe 1 für die angegebene Füllung zurück. |
| [GradientColor2](../../aspose.cells.drawing/fillformat/gradientcolor2/) { get; } | Gibt die Farbverlauffarbe 2 für die angegebene Füllung zurück. |
| [GradientColorType](../../aspose.cells.drawing/fillformat/gradientcolortype/) { get; } | Gibt den Farbverlauftyp für die angegebene Füllung zurück. |
| [GradientDegree](../../aspose.cells.drawing/fillformat/gradientdegree/) { get; } | Gibt den Grad des Farbverlaufs für die angegebene Füllung zurück. Gilt nur für Excel 2007. |
| [GradientFill](../../aspose.cells.drawing/fillformat/gradientfill/) { get; } | Liest das [`GradientFill`](./gradientfill/) Objekt. |
| [GradientStyle](../../aspose.cells.drawing/fillformat/gradientstyle/) { get; } | Gibt den Farbverlaufsstil für die angegebene Füllung zurück. |
| [GradientVariant](../../aspose.cells.drawing/fillformat/gradientvariant/) { get; } | Gibt die Farbverlaufsvariante für die angegebene Füllung zurück. Gilt nur für Excel 2007. |
| [ImageData](../../aspose.cells.drawing/fillformat/imagedata/) { get; set; } | Liest und setzt die Bilddaten. |
| [Pattern](../../aspose.cells.drawing/fillformat/pattern/) { get; set; } | Stellt ein Anzeigemuster eines Bereichs dar. |
| [PatternFill](../../aspose.cells.drawing/fillformat/patternfill/) { get; } | Liest das [`PatternFill`](./patternfill/) Objekt. |
| [PictureFormatType](../../aspose.cells.drawing/fillformat/pictureformattype/) { get; set; } | Liest und setzt den Bildformattyp. |
| [PresetColor](../../aspose.cells.drawing/fillformat/presetcolor/) { get; } | Gibt die voreingestellte Farbverlauffarbe für die angegebene Füllung zurück. |
| [Scale](../../aspose.cells.drawing/fillformat/scale/) { get; set; } | Liest und setzt die Bildformatskalierung. |
| [SetType](../../aspose.cells.drawing/fillformat/settype/) { get; set; } | (**Obsolete.**) Liest den Füllformattyp. |
| [SolidFill](../../aspose.cells.drawing/fillformat/solidfill/) { get; } | Liest das [`SolidFill`](./solidfill/) Objekt. |
| [Texture](../../aspose.cells.drawing/fillformat/texture/) { get; set; } | Stellt den Texturtyp für die angegebene Füllung dar. |
| [TextureFill](../../aspose.cells.drawing/fillformat/texturefill/) { get; } | Liest das [`TextureFill`](./texturefill/) Objekt. |
| [Transparency](../../aspose.cells.drawing/fillformat/transparency/) { get; set; } | Gibt den Transparenzgrad des Bereichs zurück oder legt ihn fest, als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent). |
| [Type](../../aspose.cells.drawing/fillformat/type/) { get; set; } | (**Obsolete.**) Liest und setzt den Fülltyp |

## Methoden

| Name | Beschreibung |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fillformat/equals/)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/fillformat/gethashcode/)() | Liest den Hash‑Code. |
| [SetOneColorGradient](../../aspose.cells.drawing/fillformat/setonecolorgradient/)(Color, double, GradientStyleType, int) | Setzt die angegebene Füllung auf einen einfarbigen Farbverlauf. Gilt nur für Excel 2007. |
| [SetPresetColorGradient](../../aspose.cells.drawing/fillformat/setpresetcolorgradient/)(GradientPresetType, GradientStyleType, int) | Setzt die angegebene Füllung auf einen voreingestellten Farbverlauf. Gilt nur für Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient/#settwocolorgradient_1)(Color, Color, GradientStyleType, int) | Setzt die angegebene Füllung auf einen Zweifarbverlauf. Gilt nur für Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient/#settwocolorgradient)(Color, double, Color, double, GradientStyleType, int) | Setzt die angegebene Füllung auf einen Zweifarbverlauf. Gilt nur für Excel 2007. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten zu Zellen hinzu
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
            
            // Füge ein Säulendiagramm zum Arbeitsblatt hinzu
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Datenreihen zum Diagramm hinzufügen
            int seriesIndex = chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";
            
            // Verwende Farbverlauffüllung für den Serienbereich
            chart.NSeries[seriesIndex].Area.FillFormat.SetOneColorGradient(System.Drawing.Color.Lime, 1, 
                GradientStyleType.Horizontal, 1);
            
            // Speichere die Arbeitsmappe
            workbook.Save("FillFormatDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


