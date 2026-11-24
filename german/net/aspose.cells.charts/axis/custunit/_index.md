---
title: "Axis.CustUnit"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Axis-Eigenschaft. Gibt einen benutzerdefinierten Wert für die Anzeigeeinheit an."
type: docs
url: /de/net/aspose.cells.charts/axis/custunit/
---
## Axis.CustUnit property

Gibt einen benutzerdefinierten Wert für die Anzeigeeinheit an.

```csharp
[Obsolete("Use Axis.CustomUnit property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int CustUnit { get; set; }
```

### Hinweise

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Bitte verwenden Sie stattdessen die Eigenschaft Axis.CustomUnit. Diese Eigenschaft wird 12 Monate nach Januar 2023 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisPropertyCustUnitDemo
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
            worksheet.Cells["A5"].PutValue("D");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(1000000);
            worksheet.Cells["B3"].PutValue(2000000);
            worksheet.Cells["B4"].PutValue(3000000);
            worksheet.Cells["B5"].PutValue(4000000);

            // Fügen Sie ein Diagramm hinzu und setzen Sie dessen Datenbereich
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Hole die Werte-Achse
            Axis valueAxis = chart.ValueAxis;

            // Aktuellen CustUnit‑Wert anzeigen (veraltete Eigenschaft)
            Console.WriteLine("Current CustUnit value: " + valueAxis.CustUnit);

            // Neuen benutzerdefinierten Einheitwert festlegen (1.000.000)
            valueAxis.CustUnit = 1000000;
            valueAxis.IsDisplayUnitLabelShown = true;

            // Neuen CustUnit‑Wert anzeigen
            Console.WriteLine("New CustUnit value: " + valueAxis.CustUnit);

            // Ergebnis speichern
            workbook.Save("AxisPropertyCustUnitDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


