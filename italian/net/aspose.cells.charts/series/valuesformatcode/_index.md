---
title: "Series.ValuesFormatCode"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Series. Rappresenta il codice di formato della Values NumberList"
type: docs
url: /it/net/aspose.cells.charts/series/valuesformatcode/
---
## Series.ValuesFormatCode property

Rappresenta il codice di formato della NumberList dei Valori.

```csharp
public string ValuesFormatCode { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyValuesFormatCodeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(0.25);
            worksheet.Cells["B3"].PutValue(0.5);
            worksheet.Cells["B4"].PutValue(0.75);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Imposta il codice di formato dei valori per la prima serie
            chart.NSeries[0].ValuesFormatCode = "0.00%";

            // Salva la cartella di lavoro
            workbook.Save("SeriesPropertyValuesFormatCodeDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


