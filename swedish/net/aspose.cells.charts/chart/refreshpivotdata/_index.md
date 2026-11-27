---
title: "Chart.RefreshPivotData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Chart-metod. Uppdaterar diagrammets data från pivottabellen"
type: docs
url: /sv/net/aspose.cells.charts/chart/refreshpivotdata/
---
## Chart.RefreshPivotData method

Uppdaterar diagrammets data från pivottabell.

```csharp
public void RefreshPivotData()
```

### Anmärkningar

Vi kommer att samla data från pivotdatakällan till pivottabellsrapporten. Denna metod används endast för att samla all data till ett pivottabell-diagram.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till exempeldata i det första kalkylbladet
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Cells["A1"].PutValue("Product");
            dataSheet.Cells["B1"].PutValue("Sales");
            dataSheet.Cells["A2"].PutValue("A");
            dataSheet.Cells["B2"].PutValue(100);
            dataSheet.Cells["A3"].PutValue("B");
            dataSheet.Cells["B3"].PutValue(200);
            dataSheet.Cells["A4"].PutValue("C");
            dataSheet.Cells["B4"].PutValue(300);

            // Skapa en pivottabell
            Worksheet pivotSheet = workbook.Worksheets.Add("Pivot");
            pivotSheet.PivotTables.Add("A1", dataSheet.Cells["A1:B4"].Name, "PivotTable1");

            // Lägg till ett diagram
            int chartIndex = pivotSheet.Charts.Add(ChartType.Column, 5, 0, 15, 8);
            Aspose.Cells.Charts.Chart chart = pivotSheet.Charts[chartIndex];
            
            // Ställ in pivottabellens datakälla
            chart.PivotSource = "Pivot!PivotTable1";
            
            // Uppdatera pivottdata i diagrammet
            chart.RefreshPivotData();
            
            // Spara arbetsboken
            workbook.Save("PivotChartWithRefresh.xlsx");
        }
    }
}
```

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


