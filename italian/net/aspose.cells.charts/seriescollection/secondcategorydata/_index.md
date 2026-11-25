---
title: "SeriesCollection.SecondCategoryData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SeriesCollection. Ottiene o imposta l'intervallo dei valori dell'asse di seconda categoria. Può essere un intervallo di celle come d1e10 o una sequenza di valori come 26810. Ha effetto solo quando alcune serie sono tracciate sul secondo asse"
type: docs
url: /it/net/aspose.cells.charts/seriescollection/secondcategorydata/
---
## SeriesCollection.SecondCategoryData property

Ottiene o imposta l'intervallo dei valori del secondo asse di categoria. Può essere un intervallo di celle (ad esempio "d1:e10"), o una sequenza di valori (ad esempio "{2,6,8,10}"). Ha effetto solo quando alcune serie sono tracciate sul secondo asse.

```csharp
public string SecondCategoryData { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionPropertySecondCategoryDataDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Primary Categories");
            worksheet.Cells["A2"].PutValue("Cat1");
            worksheet.Cells["A3"].PutValue("Cat2");
            worksheet.Cells["A4"].PutValue("Cat3");
            
            worksheet.Cells["B1"].PutValue("Secondary Categories");
            worksheet.Cells["B2"].PutValue("SubCat1");
            worksheet.Cells["B3"].PutValue("SubCat2");
            worksheet.Cells["B4"].PutValue("SubCat3");
            
            worksheet.Cells["C1"].PutValue("Values");
            worksheet.Cells["C2"].PutValue(10);
            worksheet.Cells["C3"].PutValue(20);
            worksheet.Cells["C4"].PutValue(30);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta i dati della serie
            chart.NSeries.Add("C2:C4", true);
            
            // Imposta i dati della categoria primaria
            chart.NSeries.CategoryData = "A2:A4";
            
            // Imposta i dati della categoria secondaria
            chart.NSeries.SecondCategoryData = "B2:B4";

            // Salva la cartella di lavoro
            workbook.Save("SecondCategoryDataDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


