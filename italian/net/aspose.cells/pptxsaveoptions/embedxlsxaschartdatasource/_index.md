---
title: "PptxSaveOptions.EmbedXlsxAsChartDataSource"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PptxSaveOptions. Indica se incorporare un file xlsx come origine dati del grafico"
type: docs
url: /it/net/aspose.cells/pptxsaveoptions/embedxlsxaschartdatasource/
---
## PptxSaveOptions.EmbedXlsxAsChartDataSource property

Indica se incorporare un file xlsx come origine dati del grafico.

```csharp
public bool EmbedXlsxAsChartDataSource { get; set; }
```

### Osservazioni

Il valore predefinito è true.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PptxSaveOptionsPropertyEmbedXlsxAsChartDataSourceDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Crea un foglio di lavoro di esempio con dati del grafico
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // Aggiungi un grafico per dimostrare l'effetto della proprietà
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Crea un'istanza di PptxSaveOptions
                PptxSaveOptions saveOptions = new PptxSaveOptions();

                // Mostra il valore predefinito di EmbedXlsxAsChartDataSource
                Console.WriteLine("Default EmbedXlsxAsChartDataSource value: " + saveOptions.EmbedXlsxAsChartDataSource);

                // Imposta la proprietà su true per dimostrarne l'uso
                saveOptions.EmbedXlsxAsChartDataSource = true;
                Console.WriteLine("EmbedXlsxAsChartDataSource set to: " + saveOptions.EmbedXlsxAsChartDataSource);

                // Salva la cartella di lavoro come PPTX con l'opzione abilitata
                workbook.Save("EmbedXlsxAsChartDataSourceDemo.pptx", saveOptions);

                Console.WriteLine("PPTX saved with EmbedXlsxAsChartDataSource enabled");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


