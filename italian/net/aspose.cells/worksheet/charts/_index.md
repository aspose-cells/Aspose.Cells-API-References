---
title: "Worksheet.Charts"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Ottiene una raccolta di Chart"
type: docs
url: /it/net/aspose.cells/worksheet/charts/
---
## Worksheet.Charts property

Ottiene una raccolta di [`Chart`](../../../aspose.cells.charts/chart/)

```csharp
public ChartCollection Charts { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyChartsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per il grafico
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);
            
            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Accedi alla prima serie e imposta il modello di riempimento
            Series series = chart.NSeries[0];
            series.Area.FillFormat.Pattern = FillPattern.Solid;
            
            // Salva la cartella di lavoro
            workbook.Save("WorksheetPropertyChartsDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartCollection](../../../aspose.cells.charts/chartcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


