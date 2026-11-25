---
title: "Chart.SizeWithWindow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Chart. True se Microsoft Excel ridimensiona il grafico per corrispondere alle dimensioni della finestra del foglio del grafico"
type: docs
url: /it/net/aspose.cells.charts/chart/sizewithwindow/
---
## Chart.SizeWithWindow property

Vero se Microsoft Excel ridimensiona il grafico per corrispondere alle dimensioni della finestra del foglio del grafico.

```csharp
public bool SizeWithWindow { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertySizeWithWindowDemo
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
            
            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Dimostra la proprietà SizeWithWindow
            Console.WriteLine("Default SizeWithWindow: " + chart.SizeWithWindow);
            
            // Abilita SizeWithWindow
            chart.SizeWithWindow = true;
            Console.WriteLine("After setting SizeWithWindow to true: " + chart.SizeWithWindow);
            
            // Salva la cartella di lavoro
            workbook.Save("ChartSizeWithWindowDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


