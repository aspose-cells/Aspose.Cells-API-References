---
title: "Chart.HidePivotFieldButtons"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Diagramegenskap. Anger om pivotdiagrammets fältknappar ska döljas endast när diagrammet är ett PivotChart"
type: docs
url: /sv/net/aspose.cells.charts/chart/hidepivotfieldbuttons/
---
## Chart.HidePivotFieldButtons property

Anger om fältknapparna för pivottabell-diagram ska döljas endast när diagrammet är ett PivotChart.

```csharp
public bool HidePivotFieldButtons { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class ChartPropertyHidePivotFieldButtonsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["B4"].Value = 200;

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Skapa diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column3DClustered, 9, 6, 24, 14);
            Chart chart = worksheet.Charts[chartIndex];
            chart.PivotSource = "Sheet1!PivotTable1";
            
            // Demonstrera egenskapen HidePivotFieldButtons
            chart.HidePivotFieldButtons = false; // Show pivot field buttons
            chart.RefreshPivotData();

            // Spara arbetsboken
            workbook.Save("HidePivotFieldButtonsDemo.xlsx");
        }
    }
}
```

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


