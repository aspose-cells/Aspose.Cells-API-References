---
title: "Enum PlotDataByType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.PlotDataByType Enum. Stellt den Typ der Datenplotting nach Zeile oder Spalte dar"
type: docs
url: /de/net/aspose.cells.charts/plotdatabytype/
---
## PlotDataByType enumeration

Stellt den Typ der Datenplot‑Darstellung nach Zeile oder Spalte dar.

```csharp
public enum PlotDataByType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Row | `0` | Nach Zeile sortiert. |
| Column | `1` | Nach Spalte. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartsClassPlotDataByTypeDemo
    {
        public static void Run()
        {
            // Erstellt ein neues Arbeitsbuch für die Demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Beispieldaten zum Arbeitsblatt hinzufügen
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["B1"].PutValue("Value1");
                worksheet.Cells["C1"].PutValue("Value2");
                worksheet.Cells["A2"].PutValue("Row1");
                worksheet.Cells["B2"].PutValue(10);
                worksheet.Cells["C2"].PutValue(20);
                worksheet.Cells["A3"].PutValue("Row2");
                worksheet.Cells["B3"].PutValue(30);
                worksheet.Cells["C3"].PutValue(40);

                // Füge dem Arbeitsblatt ein Diagramm hinzu
                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);
                Chart chart = worksheet.Charts[chartIndex];

                // Lege den Datenbereich des Diagramms fest
                chart.NSeries.Add("B2:C3", true);

                // Demonstration der Verwendung von PlotDataByType Enum-Werten
                PlotDataByType plotType = PlotDataByType.Row;
                Console.WriteLine($"Chart is currently plotting data by: {plotType}");

                // Ändern zu Plot nach Spalte
                plotType = PlotDataByType.Column;
                Console.WriteLine($"Chart is now plotting data by: {plotType}");

                // Speichere die Arbeitsmappe
                workbook.Save("PlotDataByTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with PlotDataByType demonstration.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with PlotDataByType: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


