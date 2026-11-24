---
title: "ChartTextFrame.Characters"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartTextFrame-Methode. Gibt ein Characters-Objekt zurück, das einen Zeichenbereich im Text darstellt"
type: docs
url: /de/net/aspose.cells.charts/charttextframe/characters/
---
## ChartTextFrame.Characters method

Gibt ein Characters‑Objekt zurück, das einen Zeichenbereich innerhalb des Textes darstellt.

```csharp
public FontSetting Characters(int startIndex, int length)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startIndex | Int32 | Der Index des Beginns des Zeichens. |
| Länge | Int32 | Die Anzahl der Zeichen. |

### Rückgabewert

Characters-Objekt.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFrameMethodCharactersWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Diagramm erstellen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Greife auf Datenbeschriftungen zu und setze die Schriftgröße für bestimmte Zeichen
            chart.NSeries[0].Points[0].DataLabels.ShowValue = true;
            chart.NSeries[0].Points[0].DataLabels.Characters(0, 5).Font.Size = 14;
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


