---
title: "Chart.Worksheet"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Chart. Ottiene il foglio di lavoro che contiene questo grafico"
type: docs
url: /it/net/aspose.cells.charts/chart/worksheet/
---
## Chart.Worksheet property

Ottiene il foglio di lavoro che contiene questo grafico.

```csharp
public Worksheet Worksheet { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyWorksheetDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            
            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Dimostrare l'uso della proprietà Worksheet
            Console.WriteLine("Chart's worksheet index: " + chart.Worksheet.Index);
            Console.WriteLine("Chart's worksheet name: " + chart.Worksheet.Name);
            
            // Salva la cartella di lavoro
            workbook.Save("ChartPropertyWorksheetDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


