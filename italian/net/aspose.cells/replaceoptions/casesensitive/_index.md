---
title: "ReplaceOptions.CaseSensitive"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ReplaceOptions. Indica se la stringa cercata è sensibile al maiuscolo/minuscolo"
type: docs
url: /it/net/aspose.cells/replaceoptions/casesensitive/
---
## ReplaceOptions.CaseSensitive property

Indica se la stringa cercata è sensibile al maiuscolo/minuscolo.

```csharp
public bool CaseSensitive { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReplaceOptionsPropertyCaseSensitiveDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta dati di esempio
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("apple");
            worksheet.Cells["A3"].PutValue("Apple");
            worksheet.Cells["A4"].PutValue("APPLE");

            // Crea le opzioni di sostituzione con CaseSensitive = false
            ReplaceOptions options = new ReplaceOptions();
            options.CaseSensitive = false;
            
            // Sostituisci tutte le varianti di maiuscole/minuscolo di "apple" con "orange"
            workbook.Replace("apple", "orange", options);

            // Restituisci i risultati
            Console.WriteLine("After replacement (CaseSensitive = false):");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + i].StringValue);
            }

            // Reimposta i dati
            worksheet.Cells["A2"].PutValue("apple");
            worksheet.Cells["A3"].PutValue("Apple");
            worksheet.Cells["A4"].PutValue("APPLE");

            // Modifica a CaseSensitive = true
            options.CaseSensitive = true;
            workbook.Replace("apple", "orange", options);

            // Restituisci i risultati
            Console.WriteLine("\nAfter replacement (CaseSensitive = true):");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + i].StringValue);
            }
        }
    }
}
```

### Vedi anche

* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


