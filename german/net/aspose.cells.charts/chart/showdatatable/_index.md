---
title: "Chart.ShowDataTable"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Diagramm-Eigenschaft. Gibt einen Wert zurück oder legt ihn fest, der angibt, ob das Diagramm eine Datentabelle anzeigt."
type: docs
url: /de/net/aspose.cells.charts/chart/showdatatable/
---
## Chart.ShowDataTable property

Liest oder setzt einen Wert, der angibt, ob das Diagramm eine Datentabelle anzeigt.

```csharp
public bool ShowDataTable { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyShowDataTableDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Workbook
            Workbook workbook = new Workbook();
            Worksheet dataSheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            dataSheet.Cells["B1"].PutValue("Column 1");
            dataSheet.Cells["C1"].PutValue("Column 2");
            dataSheet.Cells["A2"].PutValue("Item 1");
            dataSheet.Cells["A3"].PutValue("Item 2");
            dataSheet.Cells["A4"].PutValue("Item 3");
            
            dataSheet.Cells["B2"].PutValue(10);
            dataSheet.Cells["B3"].PutValue(20);
            dataSheet.Cells["B4"].PutValue(30);
            dataSheet.Cells["C2"].PutValue(15);
            dataSheet.Cells["C3"].PutValue(25);
            dataSheet.Cells["C4"].PutValue(35);

            // Diagrammblatt hinzufügen
            int chartIndex = workbook.Worksheets.Add(SheetType.Chart);
            Worksheet chartSheet = workbook.Worksheets[chartIndex];
            
            // Diagramm erstellen
            chartSheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 1, 20, 10);
            Aspose.Cells.Charts.Chart chart = chartSheet.Charts[0];
            
            // Datenquelle festlegen
            chart.NSeries.Add("Sheet1!B2:C4", true);
            chart.NSeries.CategoryData = "Sheet1!A2:A4";
            
            // Anzeige der Datentabelle aktivieren
            chart.ShowDataTable = true;
            
            // Speichere die Arbeitsmappe
            workbook.Save("ChartWithDataTable.xlsx");
        }
    }
}
```

### Siehe auch

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


