---
title: "Classe FillFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.FillFormat classe. Incapsula l'oggetto che rappresenta la formattazione di riempimento per una forma."
type: docs
url: /it/net/aspose.cells.drawing/fillformat/
---
## FillFormat class

Incapsula l'oggetto che rappresenta la formattazione di riempimento per una forma.

```csharp
public class FillFormat
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [FillType](../../aspose.cells.drawing/fillformat/filltype/) { get; set; } | Ottiene e imposta il tipo di riempimento |
| [GradientColor1](../../aspose.cells.drawing/fillformat/gradientcolor1/) { get; } | Restituisce il colore gradiente 1 per il riempimento specificato. |
| [GradientColor2](../../aspose.cells.drawing/fillformat/gradientcolor2/) { get; } | Restituisce il colore gradiente 2 per il riempimento specificato. |
| [GradientColorType](../../aspose.cells.drawing/fillformat/gradientcolortype/) { get; } | Restituisce il tipo di colore gradiente per il riempimento specificato. |
| [GradientDegree](../../aspose.cells.drawing/fillformat/gradientdegree/) { get; } | Restituisce il grado del gradiente per il riempimento specificato. Valido solo per Excel 2007. |
| [GradientFill](../../aspose.cells.drawing/fillformat/gradientfill/) { get; } | Ottiene l'oggetto [`GradientFill`](./gradientfill/). |
| [GradientStyle](../../aspose.cells.drawing/fillformat/gradientstyle/) { get; } | Restituisce lo stile del gradiente per il riempimento specificato. |
| [GradientVariant](../../aspose.cells.drawing/fillformat/gradientvariant/) { get; } | Restituisce la variante del gradiente per il riempimento specificato. Valido solo per Excel 2007. |
| [ImageData](../../aspose.cells.drawing/fillformat/imagedata/) { get; set; } | Ottiene e imposta i dati dell'immagine. |
| [Pattern](../../aspose.cells.drawing/fillformat/pattern/) { get; set; } | Rappresenta il modello di visualizzazione di un'area. |
| [PatternFill](../../aspose.cells.drawing/fillformat/patternfill/) { get; } | Ottiene l'oggetto [`PatternFill`](./patternfill/). |
| [PictureFormatType](../../aspose.cells.drawing/fillformat/pictureformattype/) { get; set; } | Ottiene e imposta il tipo di formato immagine. |
| [PresetColor](../../aspose.cells.drawing/fillformat/presetcolor/) { get; } | Restituisce il colore predefinito del gradiente per il riempimento specificato. |
| [Scale](../../aspose.cells.drawing/fillformat/scale/) { get; set; } | Ottiene e imposta la scala del formato immagine. |
| [SetType](../../aspose.cells.drawing/fillformat/settype/) { get; set; } | (**Obsolete.**) Ottiene il tipo di set del formato di riempimento. |
| [SolidFill](../../aspose.cells.drawing/fillformat/solidfill/) { get; } | Ottiene l'oggetto [`SolidFill`](./solidfill/). |
| [Texture](../../aspose.cells.drawing/fillformat/texture/) { get; set; } | Rappresenta il tipo di texture per il riempimento specificato. |
| [TextureFill](../../aspose.cells.drawing/fillformat/texturefill/) { get; } | Ottiene l'oggetto [`TextureFill`](./texturefill/). |
| [Transparency](../../aspose.cells.drawing/fillformat/transparency/) { get; set; } | Restituisce o imposta il grado di trasparenza dell'area come valore da 0,0 (opaco) a 1,0 (trasparente). |
| [Type](../../aspose.cells.drawing/fillformat/type/) { get; set; } | (**Obsolete.**) Ottiene e imposta il tipo di riempimento. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fillformat/equals/)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/fillformat/gethashcode/)() | Ottiene il codice hash. |
| [SetOneColorGradient](../../aspose.cells.drawing/fillformat/setonecolorgradient/)(Color, double, GradientStyleType, int) | Imposta il riempimento specificato a un gradiente a un colore. Valido solo per Excel 2007. |
| [SetPresetColorGradient](../../aspose.cells.drawing/fillformat/setpresetcolorgradient/)(GradientPresetType, GradientStyleType, int) | Imposta il riempimento specificato a un gradiente con colore predefinito. Valido solo per Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient/#settwocolorgradient_1)(Color, Color, GradientStyleType, int) | Imposta il riempimento specificato a un gradiente a due colori. Valido solo per Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient/#settwocolorgradient)(Color, double, Color, double, GradientStyleType, int) | Imposta il riempimento specificato a un gradiente a due colori. Valido solo per Excel 2007. |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio alle celle
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
            
            // Aggiungi un grafico a colonne al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Aggiungi serie di dati al grafico
            int seriesIndex = chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";
            
            // Applica il riempimento gradiente all'area della serie
            chart.NSeries[seriesIndex].Area.FillFormat.SetOneColorGradient(System.Drawing.Color.Lime, 1, 
                GradientStyleType.Horizontal, 1);
            
            // Salva la cartella di lavoro
            workbook.Save("FillFormatDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


