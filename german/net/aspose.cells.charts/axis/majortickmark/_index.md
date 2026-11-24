---
title: "Axis.MajorTickMark"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Achsen-Eigenschaft. Stellt den Typ der Hauptteilungsmarkierung für die angegebene Achse dar"
type: docs
url: /de/net/aspose.cells.charts/axis/majortickmark/
---
## Axis.MajorTickMark property

Gibt den Typ der Hauptteilstriche für die angegebene Achse an.

```csharp
public TickMarkType MajorTickMark { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMajorTickMarkDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Ein Säulendiagramm hinzufügen
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Setze den Typ der Hauptteilungsmarkierung auf außen
            chart.ValueAxis.MajorTickMark = TickMarkType.Outside;

            // Speichere die Arbeitsmappe
            workbook.Save("AxisPropertyMajorTickMarkDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* enum [TickMarkType](../../tickmarktype/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


