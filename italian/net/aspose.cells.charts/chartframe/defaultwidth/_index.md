---
title: "ChartFrame.DefaultWidth"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartFrame. Rappresenta la larghezza della posizione predefinita in unità di 1/4000 dell'area del grafico"
type: docs
url: /it/net/aspose.cells.charts/chartframe/defaultwidth/
---
## ChartFrame.DefaultWidth property

Rappresenta la larghezza della posizione predefinita in unità di 1/4000 dell'area del grafico.

```csharp
[Obsolete("Use ChartFrame.DefaultWidthRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int DefaultWidth { get; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Si prega di utilizzare la proprietà ChartFrame.DefaultWidthRatioToChart, invece. DefaultWidth = (int)(DefaultWidthRatioToChart * 4000); Questa proprietà sarà rimossa tra 12 mesi a partire da febbraio 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultWidthDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            
            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 15, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            // Accedi al titolo del grafico (che eredita da ChartFrame)
            Title title = chart.Title;
            
            // Visualizza la larghezza predefinita del frame del grafico (titolo in questo caso)
            Console.WriteLine("DefaultWidth of chart title: " + title.DefaultWidth);
            
            // Nota: DefaultWidth è di sola lettura, quindi non possiamo impostarlo
            // Possiamo solo leggerlo per comprendere le dimensioni predefinite
            
            // Dimostra come questa proprietà influisce sul grafico
            Console.WriteLine("IsDefaultPosBeSet: " + title.IsDefaultPosBeSet);
            Console.WriteLine("DefaultWidthRatioToChart: " + title.DefaultWidthRatioToChart);
            
            // Salva la cartella di lavoro
            workbook.Save("ChartFrameDefaultWidthDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


