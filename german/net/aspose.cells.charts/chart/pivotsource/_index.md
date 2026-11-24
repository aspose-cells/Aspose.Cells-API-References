---
title: "Chart.PivotSource"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Chart-Eigenschaft. Die Quelle ist die Daten der Pivot-Tabelle. Wenn PivotSource nicht leer ist, ist das Diagramm ein PivotChart."
type: docs
url: /de/net/aspose.cells.charts/chart/pivotsource/
---
## Chart.PivotSource property

Die Quelle sind die Daten der Pivot‑Tabelle. Wenn PivotSource nicht leer ist, ist das Diagramm ein PivotChart.

```csharp
public string PivotSource { get; set; }
```

### Hinweise

Wenn die Pivot-Tabelle "PivotTable1" im Arbeitsblatt "Sheet1" in der Datei "Book1.xls" ist. Die pivotSource könnte "[Book1.xls]Sheet1!PivotTable1" sein, wenn das Diagramm und die Pivot-Tabelle nicht in derselben Arbeitsmappe liegen. Wenn Sie diese Eigenschaft festlegen, geht die vorherige Datenquelleneinstellung verloren.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPivotSourceDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["B4"].Value = 200;
            
            // PivotTable hinzufügen
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Diagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Pivot-Quelle für das Diagramm festlegen
            chart.PivotSource = "Sheet1!PivotTable1";
            
            // Pivot-Daten und Diagramm aktualisieren
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            chart.RefreshPivotData();
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotSourceDemo.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Chart PivotSource demo executed successfully.");
        }
    }
}
```

### Siehe auch

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


