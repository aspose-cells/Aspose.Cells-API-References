---
title: "Legend.Position"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Legend-Eigenschaft. Gibt den Legendenpositionstyp zurück oder legt ihn fest."
type: docs
url: /de/net/aspose.cells.charts/legend/position/
---
## Legend.Position property

Liest oder setzt den Legendenpositionstyp.

```csharp
public LegendPositionType Position { get; set; }
```

### Hinweise

Standardposition ist rechts. Wenn die Legende sich auf der linken oder rechten Seite des Diagramms befindet, hat das Setzen der Legend.X-Eigenschaft keine Wirkung. Wenn die Legende sich oben oder unten am Diagramm befindet, hat das Setzen der Legend.Y-Eigenschaft keine Wirkung.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendPropertyPositionDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Beispieldaten zum Diagramm hinzufügen
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Füge ein Diagramm hinzu
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Legendenposition festlegen
            chart.Legend.Position = LegendPositionType.Left;

            // Speichere die Arbeitsmappe
            workbook.Save("LegendPositionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [LegendPositionType](../../legendpositiontype/)
* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


