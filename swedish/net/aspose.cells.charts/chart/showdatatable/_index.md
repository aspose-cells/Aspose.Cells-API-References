---
title: "Chart.ShowDataTable"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Diagramegenskap. Hämtar eller anger ett värde som indikerar om diagrammet visar en datatabell"
type: docs
url: /sv/net/aspose.cells.charts/chart/showdatatable/
---
## Chart.ShowDataTable property

Hämtar eller anger ett värde som indikerar om diagrammet visar en datatabell.

```csharp
public bool ShowDataTable { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet dataSheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
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

            // Lägg till diagramblad
            int chartIndex = workbook.Worksheets.Add(SheetType.Chart);
            Worksheet chartSheet = workbook.Worksheets[chartIndex];
            
            // Skapa diagram
            chartSheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 1, 20, 10);
            Aspose.Cells.Charts.Chart chart = chartSheet.Charts[0];
            
            // Ange datakälla
            chart.NSeries.Add("Sheet1!B2:C4", true);
            chart.NSeries.CategoryData = "Sheet1!A2:A4";
            
            // Aktivera visning av datatabell
            chart.ShowDataTable = true;
            
            // Spara arbetsboken
            workbook.Save("ChartWithDataTable.xlsx");
        }
    }
}
```

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


