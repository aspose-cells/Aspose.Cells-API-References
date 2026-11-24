---
title: "ChartTextFrame.TextVerticalAlignment"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartTextFrame-Eigenschaft. Gibt die vertikale Textausrichtung zurück oder legt sie fest"
type: docs
url: /de/net/aspose.cells.charts/charttextframe/textverticalalignment/
---
## ChartTextFrame.TextVerticalAlignment property

Liest und legt die vertikale Ausrichtung des Textes fest.

```csharp
public TextAlignmentType TextVerticalAlignment { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyTextVerticalAlignmentDemo
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
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ein Säulendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Setze den Titel und konfiguriere die vertikale Ausrichtung
            chart.Title.Text = "Sample Chart";
            chart.Title.TextVerticalAlignment = TextAlignmentType.Top;

            // Anzeigeeinheiten-Label konfigurieren
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Hundreds;
            chart.ValueAxis.DisplayUnitLabel.Text = "Values in Hundreds";
            chart.ValueAxis.DisplayUnitLabel.TextVerticalAlignment = TextAlignmentType.Center;

            // Speichere die Arbeitsmappe
            workbook.Save("ChartTextVerticalAlignmentDemo.xlsx");

            Console.WriteLine("Demo executed successfully. Output file: ChartTextVerticalAlignmentDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


