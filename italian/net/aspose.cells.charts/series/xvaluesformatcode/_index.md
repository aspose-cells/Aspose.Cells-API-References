---
title: "Series.XValuesFormatCode"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà della serie. Rappresenta il codice di formato della X Values NumberList"
type: docs
url: /it/net/aspose.cells.charts/series/xvaluesformatcode/
---
## Series.XValuesFormatCode property

Rappresenta il codice di formato della NumberList dei Valori X.

```csharp
public string XValuesFormatCode { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyXValuesFormatCodeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(DateTime.Now);
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));
            worksheet.Cells["B3"].PutValue(200);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Imposta il codice di formato XValues
            chart.NSeries[0].XValuesFormatCode = "M/d/yyyy";

            // Salva la cartella di lavoro
            workbook.Save("SeriesPropertyXValuesFormatCodeDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


