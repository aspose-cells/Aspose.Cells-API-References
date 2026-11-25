---
title: "Chart.RotationAngle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà del grafico. Rappresenta la rotazione della vista del grafico 3D, la rotazione dell'area del tracciato attorno all'asse z in gradi"
type: docs
url: /it/net/aspose.cells.charts/chart/rotationangle/
---
## Chart.RotationAngle property

Rappresenta la rotazione della visualizzazione del grafico 3-D (la rotazione dell'area del grafico attorno all'asse z, in gradi).

```csharp
public int RotationAngle { get; set; }
```

### Osservazioni

Il valore di questa proprietà deve essere da 0 a 360, eccetto per i grafici a barre 3D, dove il valore deve essere da 0 a 44. Il valore predefinito è 20. Si applica solo ai grafici 3D.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyRotationAngleDemo
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

            // Imposta l'angolo di rotazione a 45 gradi
            chart.RotationAngle = 45;

            // Salva la cartella di lavoro
            workbook.Save("ChartRotationAngleDemo.xlsx");

            Console.WriteLine("Chart with rotation angle created successfully.");
        }
    }
}
```

### Vedi anche

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


