---
title: "TxtSaveOptions.FormatStrategy"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TxtSaveOptions. Ottiene e imposta la strategia di formattazione durante l'esportazione del valore della cella come stringa"
type: docs
url: /it/net/aspose.cells/txtsaveoptions/formatstrategy/
---
## TxtSaveOptions.FormatStrategy property

Ottiene e imposta la strategia di formattazione quando si esporta il valore della cella come stringa.

```csharp
public CellValueFormatStrategy FormatStrategy { get; set; }
```

### Esempi

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyFormatStrategyDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta valori con formati diversi
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(599.99);

            // Applica il formato numerico ai prezzi
            Style style = workbook.CreateStyle();
            style.Number = 2; // Format as currency
            worksheet.Cells["B2:B3"].SetStyle(style);

            // Configura le opzioni di salvataggio del testo con diverse strategie di formattazione
            TxtSaveOptions options = new TxtSaveOptions
            {
                Separator = '\t',
                FormatStrategy = CellValueFormatStrategy.DisplayStyle // Show formatted values
            };

            // Salva con formattazione di visualizzazione
            workbook.Save("FormattedOutput.txt", options);

            // Passa a nessuna strategia di formattazione
            options.FormatStrategy = CellValueFormatStrategy.None;
            workbook.Save("RawOutput.txt", options);

            Console.WriteLine("Files saved with different format strategies.");
        }
    }
}
```

### Vedi anche

* enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


