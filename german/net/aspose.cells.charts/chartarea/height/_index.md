---
title: "ChartArea.Height"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartArea-Eigenschaft. Liest oder setzt den vertikalen Versatz von seiner unteren rechten Zeilen­ecke in Einheiten von 1/4000 des Diagrammbereichs"
type: docs
url: /de/net/aspose.cells.charts/chartarea/height/
---
## ChartArea.Height property

Liest oder setzt den vertikalen Versatz von seiner unteren‑rechten Zeilen­ecke, in Einheiten von 1/4000 des Diagrammbereichs.

```csharp
[Obsolete("Use ChartArea.HeightRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int Height { get; set; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die ChartArea.HeightRatioToChart‑Eigenschaft. Height = HeightRatioToChart * 4000. Diese Eigenschaft wird 12 Monate später, seit Februar 2025, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartAreaPropertyHeightDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Zugriff auf den Diagrammbereich
            ChartArea chartArea = chart.ChartArea;

            // Demonstriere die Height-Eigenschaft
            Console.WriteLine("Original Chart Area Height: " + chartArea.Height);
            
            // Ändere die Höhe
            chartArea.Height = 500;
            Console.WriteLine("Modified Chart Area Height: " + chartArea.Height);

            // Speichere die Arbeitsmappe
            workbook.Save("ChartAreaHeightDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


