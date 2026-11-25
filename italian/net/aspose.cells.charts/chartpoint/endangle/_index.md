---
title: "ChartPoint.EndAngle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ChartPoint property. Restituisce l'angolo finale per la sezione a torta misurato in gradi in senso orario dall'asse x dopo le chiamate al metodo Chart.Calculate. Si applica al grafico a torta"
type: docs
url: /it/net/aspose.cells.charts/chartpoint/endangle/
---
## ChartPoint.EndAngle property

Ottiene l'angolo finale per la sezione a torta, misurato in gradi in senso orario dall'asse x dopo aver chiamato il metodo Chart.Calculate(). Si applica al grafico a torta.

```csharp
public float EndAngle { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyEndAngleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico a torta
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Aggiungi un grafico a torta
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcola il grafico per garantire che le proprietà siano popolate
            chart.Calculate();

            // Ottieni il primo punto del grafico (fetta di mela)
            ChartPoint point = chart.NSeries[0].Points[0];

            // Visualizza il valore corrente di EndAngle
            Console.WriteLine("Current EndAngle value: " + point.EndAngle);

            // Nota: EndAngle è di sola lettura, quindi non possiamo impostarlo direttamente
            // Invece, dimostreremo come si relaziona alla fetta di torta

            // Esplodi il punto per vedere come influisce sugli angoli
            point.Explosion = 20;
            chart.Calculate(); // Recalculate to update angles

            // Visualizza il nuovo EndAngle dopo l'esplosione
            Console.WriteLine("EndAngle after explosion: " + point.EndAngle);

            // Salva la cartella di lavoro
            workbook.Save("ChartPointEndAngleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


