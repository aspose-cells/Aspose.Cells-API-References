---
title: "ShapeCollection.AddTextEffectInChart"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeCollection-Methode. Fügt ein WordArt-Objekt in das Diagramm ein."
type: docs
url: /de/net/aspose.cells.drawing/shapecollection/addtexteffectinchart/
---
## ShapeCollection.AddTextEffectInChart method

Fügt ein WordArt-Objekt zum Diagramm ein.

```csharp
public Shape AddTextEffectInChart(MsoPresetTextEffect effect, string text, string fontName, 
    int size, bool fontBold, bool fontItalic, int top, int left, int height, int width)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Effekt | MsoPresetTextEffect | Der mso-Voreinstellungstext-Effekttyp. |
| Text | String | Der WordArt-Text. |
| fontName | String | Der Schriftname. |
| Größe | Int32 | Die Schriftgröße |
| fontBold | Boolean | Gibt an, ob die Schrift fett ist. |
| fontItalic | Boolean | Gibt an, ob die Schrift kursiv ist. |
| oben | Int32 | Stellt den vertikalen Versatz der Form vom oberen linken Eckpunkt in Einheiten von 1/4000 des Diagrammbereichs dar. |
| links | Int32 | Stellt den vertikalen Versatz der Form vom oberen linken Eckpunkt in Einheiten von 1/4000 des Diagrammbereichs dar. |
| Höhe | Int32 | Stellt die Höhe der Form in Einheiten von 1/4000 des Diagrammbereichs dar. |
| Breite | Int32 | Stellt die Breite der Form in Einheiten von 1/4000 des Diagrammbereichs dar. |

### Rückgabewert

Gibt ein Shape-Objekt zurück, das das neue WordArt-Objekt darstellt.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu und füge Beispieldaten hinzu
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            
            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);
            
            // WordArt zum Diagramm hinzufügen
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
                
            // Das Erscheinungsbild von WordArt anpassen
            wordart.FillFormat.Transparency = 0.7;
            wordart.LineFormat.IsVisible = false;
            
            // Speichere die Arbeitsmappe
            workbook.Save("WordArtInChart.xlsx");
        }
    }
}
```

### Siehe auch

* class [Shape](../../shape/)
* enum [MsoPresetTextEffect](../../msopresettexteffect/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


