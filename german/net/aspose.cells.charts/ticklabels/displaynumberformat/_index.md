---
title: "TickLabels.DisplayNumberFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TickLabels-Eigenschaft. Ruft das Anzeigezahlenformat der Tick-Labels ab und legt es fest"
type: docs
url: /de/net/aspose.cells.charts/ticklabels/displaynumberformat/
---
## TickLabels.DisplayNumberFormat property

Liest und setzt das Anzeige‑Zahlenformat der Tick‑Beschriftungen.

```csharp
public string DisplayNumberFormat { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyDisplayNumberFormatDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(DateTime.Now);
            worksheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            
            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("A2:A3", true);
            chart.NSeries.CategoryData = "B2:B3";
            
            // Stattdessen das Zahlenformat über die NumberFormat-Eigenschaft festlegen
            chart.CategoryAxis.TickLabels.NumberFormat = "m/d/yyyy";
            chart.ValueAxis.TickLabels.NumberFormat = "#,##0";
            
            // Speichere die Arbeitsmappe
            workbook.Save("TickLabelsDisplayNumberFormatDemo.xlsx");
            
            Console.WriteLine("DisplayNumberFormat for CategoryAxis: " + 
                chart.CategoryAxis.TickLabels.DisplayNumberFormat);
            Console.WriteLine("DisplayNumberFormat for ValueAxis: " + 
                chart.ValueAxis.TickLabels.DisplayNumberFormat);
        }
    }
}
```

### Siehe auch

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


