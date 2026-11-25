---
title: "ReplaceOptions.RegexKey"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ReplaceOptions. Indica se la chiave cercata è una regex. Se true, la chiave cercata verrà interpretata come regex"
type: docs
url: /it/net/aspose.cells/replaceoptions/regexkey/
---
## ReplaceOptions.RegexKey property

Indica se la chiave cercata è una regex. Se vero, la chiave cercata verrà interpretata come regex.

```csharp
public bool RegexKey { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReplaceOptionsPropertyRegexKeyDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("apple");
            worksheet.Cells["A2"].PutValue("banana");
            worksheet.Cells["A3"].PutValue("orange");
            worksheet.Cells["A4"].PutValue("pear");
            worksheet.Cells["A5"].PutValue("plum");

            // Crea le opzioni di sostituzione con regex
            ReplaceOptions options = new ReplaceOptions();
            options.RegexKey = true; // Enable regex matching
            
            // Sostituisci tutte le parole che iniziano con 'p' o 'b' seguite da una vocale
            string pattern = "^[pb][aeiou]";
            string replacement = "FRUIT";
            
            // Esegui la sostituzione
            workbook.Replace(pattern, replacement, options);

            // Salva il risultato
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


