---
title: "Chart.IsRectangularCornered"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Chart. Ottiene o imposta un valore che indica se l'area del grafico ha angoli rettangolari. Il valore predefinito è true"
type: docs
url: /it/net/aspose.cells.charts/chart/isrectangularcornered/
---
## Chart.IsRectangularCornered property

Ottiene o imposta un valore che indica se l'area del grafico ha angoli rettangolari. Il valore predefinito è true.

```csharp
public bool IsRectangularCornered { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyIsRectangularCorneredDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
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

            // Aggiungi un grafico a colonne
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Dimostra la proprietà IsRectangularCornered
            Console.WriteLine("Default IsRectangularCornered: " + chart.IsRectangularCornered);
            
            // Imposta su true per rendere gli angoli del grafico rettangolari
            chart.IsRectangularCornered = true;
            Console.WriteLine("After setting IsRectangularCornered to true: " + chart.IsRectangularCornered);

            // Salva la cartella di lavoro
            workbook.Save("ChartPropertyIsRectangularCorneredDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


