---
title: "Chart.HeightPercent"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Chart. Restituisce o imposta l'altezza di un grafico 3D come percentuale della larghezza del grafico, compresa tra 5 e 500 percento"
type: docs
url: /it/net/aspose.cells.charts/chart/heightpercent/
---
## Chart.HeightPercent property

Restituisce o imposta l'altezza di un grafico 3-D come percentuale della larghezza del grafico (tra il 5 e il 500 percento).

```csharp
public int HeightPercent { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyHeightPercentDemo
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

            // Aggiungi un grafico a colonne 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Imposta la proprietà HeightPercent (controlla l'altezza del grafico 3D come percentuale della larghezza del grafico)
            chart.HeightPercent = 150; // 150% of chart width

            // Salva la cartella di lavoro
            workbook.Save("ChartHeightPercentDemo.xlsx");

            Console.WriteLine("Chart with HeightPercent 150% created successfully.");
        }
    }
}
```

### Vedi anche

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


