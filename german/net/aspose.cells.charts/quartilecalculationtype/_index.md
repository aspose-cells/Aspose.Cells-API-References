---
title: "Enum QuartileCalculationType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.QuartileCalculationType-Enum. Stellt Methoden zur Quartilsberechnung dar."
type: docs
url: /de/net/aspose.cells.charts/quartilecalculationtype/
---
## QuartileCalculationType enumeration

Stellt Methoden zur Quartilsberechnung dar.

```csharp
public enum QuartileCalculationType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Exclusive | `0` | Die Quartilsberechnung schließt den Median ein, wenn der Datensatz in Quartile aufgeteilt wird. |
| Inclusive | `1` | Die Quartilsberechnung schließt den Median aus, wenn der Datensatz in Quartile aufgeteilt wird. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class QuartileCalculationTypeDemo
    {
        public static void QuartileCalculationTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Beispieldaten für das Diagramm hinzu
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["A5"].PutValue("Q4");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.BoxWhisker, 7, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Serie zum Diagramm hinzufügen
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Greife auf die Layout‑Eigenschaften der Serie zu
            SeriesLayoutProperties layoutProperties = chart.NSeries[0].LayoutProperties;

            // Setze den Quartilsberechnungstyp
            layoutProperties.QuartileCalculation = QuartileCalculationType.Exclusive;

            // Speichere die Arbeitsmappe
            workbook.Save("QuartileCalculationTypeExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


