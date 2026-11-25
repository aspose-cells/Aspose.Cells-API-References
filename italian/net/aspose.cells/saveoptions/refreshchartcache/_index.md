---
title: "SaveOptions.RefreshChartCache"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SaveOptions. Indica se memorizzare nella cache gli ultimi dati del grafico"
type: docs
url: /it/net/aspose.cells/saveoptions/refreshchartcache/
---
## SaveOptions.RefreshChartCache property

Indica se memorizzare nella cache gli ultimi dati del grafico.

```csharp
public bool RefreshChartCache { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyRefreshChartCacheDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di esempio con un grafico
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Crea le opzioni di salvataggio PDF con RefreshChartCache abilitato
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.RefreshChartCache = true;

            // Salva la cartella di lavoro con l'opzione di aggiornamento della cache del grafico
            workbook.Save("output.pdf", pdfSaveOptions);

            Console.WriteLine("Workbook saved with chart cache refreshed.");
        }
    }
}
```

### Vedi anche

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


