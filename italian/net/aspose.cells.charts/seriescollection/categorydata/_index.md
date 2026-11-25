---
title: "SeriesCollection.CategoryData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SeriesCollection. Ottiene o imposta l'intervallo dei valori dell'asse di categoria. Può essere un intervallo di celle come d1e10 o una sequenza di valori come 26810"
type: docs
url: /it/net/aspose.cells.charts/seriescollection/categorydata/
---
## SeriesCollection.CategoryData property

Ottiene o imposta l'intervallo dei valori dell'asse di categoria. Può essere un intervallo di celle (ad esempio "d1:e10") o una sequenza di valori (ad esempio "{2,6,8,10}").

```csharp
public string CategoryData { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionPropertyCategoryDataDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue("Cat " + (i - 1));
                worksheet.Cells["B" + i].PutValue(i * 10);
            }
            
            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("=Sheet1!$B$2:$B$10", true);
            chart.NSeries.CategoryData = "=Sheet1!$A$2:$A$10";
            
            // Salva la cartella di lavoro
            workbook.Save("CategoryDataDemo.xlsx");
            
            // Verifica la proprietà CategoryData
            Console.WriteLine("Chart CategoryData: " + chart.NSeries.CategoryData);
        }
    }
}
```

### Vedi anche

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


