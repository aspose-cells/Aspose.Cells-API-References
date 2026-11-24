---
title: "Chart.SwitchRowColumn"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Chart‑Methode. Wechselt Zeile/Spalte"
type: docs
url: /de/net/aspose.cells.charts/chart/switchrowcolumn/
---
## Chart.SwitchRowColumn method

Vertauscht Zeile/Spalte.

```csharp
public bool SwitchRowColumn()
```

### Rückgabewert

False bedeutet, dass das Wechseln von Zeile/Spalte fehlschlägt.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodSwitchRowColumnDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["C1"].PutValue("Series 2");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["C2"].PutValue(150);
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["C3"].PutValue(250);
            worksheet.Cells["A4"].PutValue("Item 3");
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["C4"].PutValue(350);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.SetChartDataRange("A1:C4", true);
            
            // Originale Reihenwerte anzeigen
            Console.WriteLine("Before SwitchRowColumn:");
            Console.WriteLine("Series 1 Values: " + chart.NSeries[0].Values);
            
            // Zeile/Spalte wechseln
            chart.SwitchRowColumn();
            
            // Serienwerte nach dem Umschalten anzeigen
            Console.WriteLine("\nAfter SwitchRowColumn:");
            Console.WriteLine("Series 1 Values: " + chart.NSeries[0].Values);
            
            // Speichere die Arbeitsmappe
            workbook.Save("SwitchRowColumnDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


