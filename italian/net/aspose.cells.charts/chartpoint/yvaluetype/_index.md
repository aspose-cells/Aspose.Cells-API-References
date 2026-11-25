---
title: "ChartPoint.YValueType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartPoint. Ottiene il tipo di valore Y del punto del grafico"
type: docs
url: /it/net/aspose.cells.charts/chartpoint/yvaluetype/
---
## ChartPoint.YValueType property

Ottiene il tipo di valore Y del chart point.

```csharp
public CellValueType YValueType { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyYValueTypeDemo
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

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ottieni il primo punto del grafico nella prima serie
            ChartPoint chartPoint = chart.NSeries[0].Points[0];

            // Visualizza il YValueType corrente
            Console.WriteLine("Current YValueType: " + chartPoint.YValueType);

            // Mostra lo YValue prima della modifica
            Console.WriteLine("Current YValue: " + chartPoint.YValue);

            // Modifica lo YValue in un tipo diverso (stringa per dimostrare il cambio di tipo)
            chartPoint.YValue = "15"; // This will change the YValueType to IsString

            // Mostra lo YValueType dopo la modifica
            Console.WriteLine("New YValueType: " + chartPoint.YValueType);
            Console.WriteLine("New YValue: " + chartPoint.YValue);

            // Salva la cartella di lavoro
            workbook.Save("ChartPointPropertyYValueTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [CellValueType](../../../aspose.cells/cellvaluetype/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


