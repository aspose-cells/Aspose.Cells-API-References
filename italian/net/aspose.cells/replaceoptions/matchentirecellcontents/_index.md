---
title: "ReplaceOptions.MatchEntireCellContents"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ReplaceOptions proprietà. Indica se corrispondere all'intero contenuto delle celle"
type: docs
url: /it/net/aspose.cells/replaceoptions/matchentirecellcontents/
---
## ReplaceOptions.MatchEntireCellContents property

Indica se corrispondere all'intero contenuto delle celle

```csharp
public bool MatchEntireCellContents { get; set; }
```

### Osservazioni

Il valore predefinito è true.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReplaceOptionsPropertyMatchEntireCellContentsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta valori di cella di esempio
            worksheet.Cells["A1"].PutValue("apple");
            worksheet.Cells["A2"].PutValue("apple pie");
            worksheet.Cells["A3"].PutValue("an apple");
            worksheet.Cells["A4"].PutValue("apples");

            // Sostituisci con MatchEntireCellContents = true (solo corrispondenza esatta)
            ReplaceOptions options1 = new ReplaceOptions();
            options1.MatchEntireCellContents = true;
            workbook.Replace("apple", "orange", options1);

            // Sostituisci con MatchEntireCellContents = false (corrispondenza parziale)
            ReplaceOptions options2 = new ReplaceOptions();
            options2.MatchEntireCellContents = false;
            workbook.Replace("apple", "banana", options2);

            // Restituisci i risultati
            Console.WriteLine("A1: " + worksheet.Cells["A1"].StringValue); // orange (exact match)
            Console.WriteLine("A2: " + worksheet.Cells["A2"].StringValue); // banana pie (partial match)
            Console.WriteLine("A3: " + worksheet.Cells["A3"].StringValue); // an banana (partial match)
            Console.WriteLine("A4: " + worksheet.Cells["A4"].StringValue); // bananas (partial match)
        }
    }
}
```

### Vedi anche

* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


