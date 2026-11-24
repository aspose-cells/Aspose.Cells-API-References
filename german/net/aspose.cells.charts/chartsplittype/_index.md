---
title: "Aufzählung ChartSplitType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.ChartSplitType enum. Beschreibt, wie die beiden Abschnitte eines Kreis‑aus‑Kreis‑Diagramms oder eines Balken‑aus‑Kreis‑Diagramms aufgeteilt werden"
type: docs
url: /de/net/aspose.cells.charts/chartsplittype/
---
## ChartSplitType enumeration

Stellt dar, wie die beiden Abschnitte eines Kreis‑im‑Kreis‑Diagramms oder eines Balken‑im‑Kreis‑Diagramms aufgeteilt werden.

```csharp
public enum ChartSplitType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Position | `0` | Stellt die Datenpunkte dar. Die Datenpunkte werden zwischen dem Kreisdiagramm und dem zweiten Diagramm aufgeteilt, indem die letzte Teilungsposition der Datenpunkte im zweiten Diagramm gesetzt wird. |
| Value | `1` | Stellt die Datenpunkte dar, die zwischen dem Kreisdiagramm und dem zweiten Diagramm aufgeteilt werden, indem die Datenpunkte mit einem Wert kleiner als Split Position im zweiten Diagramm platziert werden. |
| PercentValue | `2` | Stellt die Datenpunkte dar, die zwischen dem Kreisdiagramm und dem zweiten Diagramm aufgeteilt werden, indem die Punkte mit einem Prozentsatz kleiner als Split Position Prozent im zweiten Diagramm platziert werden. |
| Custom | `3` | Stellt die Datenpunkte dar, die zwischen dem Kreisdiagramm und dem zweiten Diagramm gemäß den benutzerdefinierten Teilungswerten aufgeteilt werden. |
| Auto | `4` | Stellt die Datenpunkte dar, die mit dem Standardmechanismus für diesen Diagrammtyp aufgeteilt werden. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartsClassChartSplitTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Beispieldaten für das Diagramm hinzufügen
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["A2"].PutValue("A");
                worksheet.Cells["A3"].PutValue("B");
                worksheet.Cells["A4"].PutValue("C");
                worksheet.Cells["A5"].PutValue("D");

                worksheet.Cells["B1"].PutValue("Value");
                worksheet.Cells["B2"].PutValue(10);
                worksheet.Cells["B3"].PutValue(20);
                worksheet.Cells["B4"].PutValue(30);
                worksheet.Cells["B5"].PutValue(40);

                // Ein Kreisdiagramm hinzufügen
                int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
                Chart chart = worksheet.Charts[chartIndex];

                // Diagrammdatenbereich festlegen
                chart.NSeries.Add("B2:B5", true);
                chart.NSeries.CategoryData = "A2:A5";

                // Verschiedene ChartSplitType‑Werte demonstrieren
                chart.NSeries[0].SplitType = ChartSplitType.Position;
                Console.WriteLine($"Current SplitType: {chart.NSeries[0].SplitType}");

                // Zu einem anderen Teilungstyp wechseln
                chart.NSeries[0].SplitType = ChartSplitType.PercentValue;
                Console.WriteLine($"Updated SplitType: {chart.NSeries[0].SplitType}");

                // Speichere die Arbeitsmappe
                workbook.Save("ChartSplitTypeDemo.xlsx");
                Console.WriteLine("ChartSplitType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in ChartSplitType demonstration: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


