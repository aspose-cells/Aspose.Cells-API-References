---
title: "ChartDataTable.Border"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartDataTable-Eigenschaft. Gibt ein Border-Objekt zurück, das den Rand des Objekts darstellt"
type: docs
url: /de/net/aspose.cells.charts/chartdatatable/border/
---
## ChartDataTable.Border property

Gibt ein Border-Objekt zurück, das den Rand des Objekts darstellt

```csharp
public Line Border { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyBorderDemo
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

            // Ein Säulendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Datentabelle anzeigen
            chart.ShowDataTable = true;
            ChartDataTable dataTable = chart.ChartDataTable;

            // Rand‑Eigenschaften konfigurieren
            Line border = dataTable.Border;
            border.Color = System.Drawing.Color.Blue;
            border.Style = LineType.Solid;
            border.Weight = WeightType.MediumLine;
            border.DashType = MsoLineDashStyle.Solid;
            
            // Sichtbarkeit der Tabellenränder konfigurieren
            dataTable.HasHorizontalBorder = true;
            dataTable.HasVerticalBorder = true;
            dataTable.HasOutlineBorder = true;

            // Speichere die Arbeitsmappe
            workbook.Save("ChartDataTableBorderDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Line](../../../aspose.cells.drawing/line/)
* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


