---
title: "ChartArea.X"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartArea-Eigenschaft. Gibt den horizontalen Versatz von seiner oberen linken Spalten-Ecke in Einheiten von 1/4000 des Diagrammbereichs zurück oder legt ihn fest."
type: docs
url: /de/net/aspose.cells.charts/chartarea/x/
---
## ChartArea.X property

Gibt den horizontalen Versatz von seiner oberen linken Spalten-Ecke in Einheiten von 1/4000 des Diagrammbereichs zurück oder legt ihn fest.

```csharp
[Obsolete("Use ChartArea.XRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int X { get; set; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die ChartArea.XRatioToChart-Eigenschaft. X = XRatioToChart * 4000. Diese Eigenschaft wird 12 Monate später, seit Februar 2025, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartAreaPropertyXDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Diagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Diagrammbereich konfigurieren
            Aspose.Cells.Charts.ChartArea chartArea = chart.ChartArea;
            chartArea.X = 10; // Demonstrating X property usage
            chartArea.Y = 10;
            chartArea.Width = 400;
            chartArea.Height = 300;

            // Ausgabe speichern
            workbook.Save("ChartAreaXDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


