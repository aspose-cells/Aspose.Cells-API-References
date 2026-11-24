---
title: "Chart.SetChartDataRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Chart‑Methode. Gibt den Datenbereich für ein Diagramm an."
type: docs
url: /de/net/aspose.cells.charts/chart/setchartdatarange/
---
## Chart.SetChartDataRange method

Legt den Datenbereich für ein Diagramm fest.

```csharp
public void SetChartDataRange(string area, bool isVertical)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Bereich | String | Gibt die Werte an, aus denen die Datenreihe geplottet wird |
| isVertical | Boolean | Gibt an, ob die Reihe aus einem Zellbereich zeilenweise oder spaltenweise geplottet werden soll. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodSetChartDataRangeWithStringBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["A2"].PutValue("Cat1");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Cat2");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("Cat3");
            worksheet.Cells["B4"].PutValue(30);
            
            // Diagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.SetChartDataRange("A1:B4", true);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


