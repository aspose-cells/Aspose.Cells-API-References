---
title: "ChartDataTable.Font"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartDataTable‑Eigenschaft. Gibt ein Font‑Objekt zurück, das die Schriftarteinstellung der angegebenen Diagrammdatentabelle darstellt."
type: docs
url: /de/net/aspose.cells.charts/chartdatatable/font/
---
## ChartDataTable.Font property

Gibt ein `Font`‑Objekt zurück, das die Schriftarteinstellung der angegebenen Diagrammdatentabelle darstellt.

```csharp
public Font Font { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyFontDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(15);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Datentabelle aktivieren
            chart.ShowDataTable = true;
            
            // Das Daten­tabellen‑Objekt abrufen
            ChartDataTable dataTable = chart.ChartDataTable;
            
            // Schriftart der Datentabelle anpassen
            dataTable.Font.Size = 14;
            dataTable.Font.Color = Color.Red;
            dataTable.Font.IsBold = true;
            dataTable.Font.Name = "Arial";

            // Speichere die Arbeitsmappe
            workbook.Save("ChartDataTableFontDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Font](../../../aspose.cells/font/)
* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


