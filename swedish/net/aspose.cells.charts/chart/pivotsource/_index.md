---
title: "Chart.PivotSource"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Diagramegenskap. Källan är data från pivottabellen. Om PivotSource inte är tom är diagrammet ett PivotChart."
type: docs
url: /sv/net/aspose.cells.charts/chart/pivotsource/
---
## Chart.PivotSource property

Källan är data från pivottabellen. Om PivotSource inte är tom, är diagrammet ett PivotChart.

```csharp
public string PivotSource { get; set; }
```

### Anmärkningar

Om pivottabellen "PivotTable1" i arbetsbladet "Sheet1" i filen "Book1.xls". PivotSource kan vara "[Book1.xls]Sheet1!PivotTable1" om diagrammet och pivottabellen inte finns i samma arbetsbok. Om du anger denna egenskap förloras den tidigare datakällinställningen.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
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
            
            // Lägg till pivottabell
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Lägg till diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange pivottkälla för diagrammet
            chart.PivotSource = "Sheet1!PivotTable1";
            
            // Uppdatera pivottdata och diagram
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            chart.RefreshPivotData();
            
            // Spara arbetsboken
            workbook.Save("PivotSourceDemo.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Chart PivotSource demo executed successfully.");
        }
    }
}
```

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


