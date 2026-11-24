---
title: "PivotTableCalculateOption.RefreshCharts"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTableCalculateOption-Eigenschaft. Gibt an, ob Diagramme basierend auf dieser Pivot-Tabelle aktualisiert werden"
type: docs
url: /de/net/aspose.cells.pivot/pivottablecalculateoption/refreshcharts/
---
## PivotTableCalculateOption.RefreshCharts property

Gibt an, ob Diagramme basierend auf dieser PivotTable aktualisiert werden.

```csharp
public bool RefreshCharts { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCalculateOptionPropertyRefreshChartsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(150);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(180);

            // Pivot-Tabelle erstellen
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "SalesPivot");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Ein Diagramm erstellen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.PivotSource = "SalesPivot";
            chart.SetChartDataRange("D1:E4", true);

            // Mit der RefreshCharts-Option berechnen
            PivotTableCalculateOption options = new PivotTableCalculateOption
            {
                RefreshData = true,
                RefreshCharts = true
            };
            pivotTable.CalculateData(options);

            workbook.Save("PivotTableRefreshChartsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTableCalculateOption](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


