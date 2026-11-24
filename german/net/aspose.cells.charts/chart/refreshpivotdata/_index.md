---
title: "Chart.RefreshPivotData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Chart-Methode. Aktualisiert die Diagrammdaten aus der Pivot-Tabelle."
type: docs
url: /de/net/aspose.cells.charts/chart/refreshpivotdata/
---
## Chart.RefreshPivotData method

Aktualisiert die Diagrammdaten aus der Pivot-Tabelle.

```csharp
public void RefreshPivotData()
```

### Hinweise

Wir sammeln Daten aus der Pivot-Datenquelle für den Pivot-Tabellenbericht. Diese Methode wird nur verwendet, um alle Daten für ein Pivot-Diagramm zu sammeln.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodRefreshPivotDataDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Füge Beispieldaten zum ersten Arbeitsblatt hinzu
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Cells["A1"].PutValue("Product");
            dataSheet.Cells["B1"].PutValue("Sales");
            dataSheet.Cells["A2"].PutValue("A");
            dataSheet.Cells["B2"].PutValue(100);
            dataSheet.Cells["A3"].PutValue("B");
            dataSheet.Cells["B3"].PutValue(200);
            dataSheet.Cells["A4"].PutValue("C");
            dataSheet.Cells["B4"].PutValue(300);

            // Erstelle eine Pivot-Tabelle
            Worksheet pivotSheet = workbook.Worksheets.Add("Pivot");
            pivotSheet.PivotTables.Add("A1", dataSheet.Cells["A1:B4"].Name, "PivotTable1");

            // Füge ein Diagramm hinzu
            int chartIndex = pivotSheet.Charts.Add(ChartType.Column, 5, 0, 15, 8);
            Aspose.Cells.Charts.Chart chart = pivotSheet.Charts[chartIndex];
            
            // Pivot-Diagrammdatenquelle festlegen
            chart.PivotSource = "Pivot!PivotTable1";
            
            // Pivot-Daten im Diagramm aktualisieren
            chart.RefreshPivotData();
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotChartWithRefresh.xlsx");
        }
    }
}
```

### Siehe auch

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


