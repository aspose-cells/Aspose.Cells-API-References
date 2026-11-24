---
title: "Chart.ValueAxis"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Chart-Eigenschaft. Gibt die Y‑Achse des Diagramms zurück"
type: docs
url: /de/net/aspose.cells.charts/chart/valueaxis/
---
## Chart.ValueAxis property

Ermittelt die Y-Achse des Diagramms.

```csharp
public Axis ValueAxis { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyValueAxisDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100000000);
            worksheet.Cells["B3"].PutValue(200000000);
            worksheet.Cells["B4"].PutValue(300000000);

            // Fügen Sie ein Diagramm hinzu und setzen Sie dessen Datenbereich
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // ValueAxis-Eigenschaften konfigurieren
            chart.ValueAxis.DisplayUnit = DisplayUnitType.HundredMillions;
            chart.ValueAxis.Title.Text = "Values (in 100 millions)";
            chart.ValueAxis.MajorUnit = 1;

            // Speichere die Arbeitsmappe
            workbook.Save("ChartPropertyValueAxisDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Axis](../../axis/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


