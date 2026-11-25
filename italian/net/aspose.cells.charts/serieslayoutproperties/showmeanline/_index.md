---
title: "SeriesLayoutProperties.ShowMeanLine"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SeriesLayoutProperties. Indica se mostrare la linea che collega tutti i punti medi"
type: docs
url: /it/net/aspose.cells.charts/serieslayoutproperties/showmeanline/
---
## SeriesLayoutProperties.ShowMeanLine property

Indica se mostrare la linea che collega tutti i punti medi.

```csharp
public bool ShowMeanLine { get; set; }
```

### Osservazioni

Funziona solo per il grafico BoxWhisker.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesLayoutPropertiesPropertyShowMeanLineDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico a scatola e baffi
            worksheet.Cells["A1"].PutValue("Series 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(40);
            worksheet.Cells["A4"].PutValue(25);
            worksheet.Cells["A5"].PutValue(40);
            worksheet.Cells["A6"].PutValue(115);
            worksheet.Cells["A7"].PutValue(65.666);

            // Aggiungi un grafico a scatola e baffi
            int chartIndex = worksheet.Charts.Add(ChartType.BoxWhisker, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Aggiungi serie al grafico
            chart.NSeries.Add("A1:A7", true);

            // Ottieni la prima serie
            Series series = chart.NSeries[0];

            // Accedi alle proprietà di layout
            SeriesLayoutProperties layout = series.LayoutProperties;

            // Dimostra la proprietà ShowMeanLine
            Console.WriteLine("Default ShowMeanLine value: " + layout.ShowMeanLine);
            
            // Imposta ShowMeanLine su true
            layout.ShowMeanLine = true;
            Console.WriteLine("After setting ShowMeanLine to true: " + layout.ShowMeanLine);

            // Salva la cartella di lavoro
            workbook.Save("BoxWhiskerChart_ShowMeanLineDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


