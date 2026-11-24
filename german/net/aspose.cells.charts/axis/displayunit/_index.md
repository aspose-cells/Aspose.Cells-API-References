---
title: "Axis.DisplayUnit"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Achsen-Eigenschaft. Stellt die Einheitensbeschriftung für die angegebene Achse dar"
type: docs
url: /de/net/aspose.cells.charts/axis/displayunit/
---
## Axis.DisplayUnit property

Stellt die Einheitbeschriftung für die angegebene Achse dar

```csharp
public DisplayUnitType DisplayUnit { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyDisplayUnitDemo
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
            worksheet.Cells["B2"].PutValue(10000);
            worksheet.Cells["B3"].PutValue(20000);
            worksheet.Cells["B4"].PutValue(30000);

            // Ein Säulendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Setze die Anzeigeeinheit für die Werteachse auf Tausend
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Thousands;

            // Speichere die Arbeitsmappe
            workbook.Save("AxisPropertyDisplayUnitDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* enum [DisplayUnitType](../../displayunittype/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


