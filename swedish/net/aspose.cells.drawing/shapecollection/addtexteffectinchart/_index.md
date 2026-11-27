---
title: "ShapeCollection.AddTextEffectInChart"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection‑metod. Infogar ett WordArt‑objekt i diagrammet"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/addtexteffectinchart/
---
## ShapeCollection.AddTextEffectInChart method

Infogar ett WordArt-objekt i diagrammet.

```csharp
public Shape AddTextEffectInChart(MsoPresetTextEffect effect, string text, string fontName, 
    int size, bool fontBold, bool fontItalic, int top, int left, int height, int width)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| effekt | MsoPresetTextEffect | Typen av mso förinställd texteffekt. |
| text | String | WordArt-texten. |
| fontName | String | Typsnittets namn. |
| storlek | Int32 | Typsnittsstorleken |
| fontBold | Boolean | Anger om teckensnittet är fetstil. |
| fontItalic | Boolean | Anger om teckensnittet är kursiv. |
| top | Int32 | Representerar det vertikala offsetet för formen från det övre vänstra hörnet i enheter av 1/4000 av diagramområdet. |
| vänster | Int32 | Representerar det vertikala offsetet för formen från det övre vänstra hörnet i enheter av 1/4000 av diagramområdet. |
| höjd | Int32 | Representerar formens höjd, i enheter av 1/4000 av diagramområdet. |
| bredd | Int32 | Representerar formens bredd, i enheter av 1/4000 av diagramområdet. |

### Returvärde

Returnerar ett Shape-objekt som representerar det nya WordArt-objektet.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddTextEffectInChartWithMsoPresetTextEffectStringStrinDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första kalkylbladet och lägg till exempeldata
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            
            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);
            
            // Lägg till WordArt i diagrammet
            Shape wordart = chart.Shapes.AddTextEffectInChart(
                MsoPresetTextEffect.TextEffect2,
                "SAMPLE TEXT", 
                "Arial Black", 
                36, 
                false, 
                false,
                100,  // Left position
                100,  // Top position
                300,  // Width
                200); // Height
                
            // Anpassa WordArt-utseendet
            wordart.FillFormat.Transparency = 0.7;
            wordart.LineFormat.IsVisible = false;
            
            // Spara arbetsboken
            workbook.Save("WordArtInChart.xlsx");
        }
    }
}
```

### Se även

* class [Shape](../../shape/)
* enum [MsoPresetTextEffect](../../msopresettexteffect/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


