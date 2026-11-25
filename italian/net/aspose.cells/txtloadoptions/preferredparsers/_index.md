---
title: "TxtLoadOptions.PreferredParsers"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TxtLoadOptions. Ottiene e imposta i parser di valore preferiti per il caricamento di file di testo"
type: docs
url: /it/net/aspose.cells/txtloadoptions/preferredparsers/
---
## TxtLoadOptions.PreferredParsers property

Ottiene e imposta i parser di valore preferiti per il caricamento di un file di testo.

```csharp
public ICustomParser[] PreferredParsers { get; set; }
```

### Osservazioni

parsers[0] è il parser che verrà usato per la prima colonna nel file modello di testo, parsers[1] è il parser che verrà usato per la seconda colonna, ...ecc. L'ultimo (parsers[parsers.length-1]) verrà usato per tutte le altre colonne a partire da parsers.length-1. Se un elemento è null, la colonna corrispondente verrà analizzata dal parser predefinito di Aspose.Cells.

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyPreferredParsersDemo
    {
        private class StringParser : ICustomParser
        {
            public bool Parse(string value, out object result)
            {
                result = value; // Always return as string
                return true;
            }

            public object ParseObject(string value)
            {
                return value; // Always return as string
            }

            public string GetFormat()
            {
                return "String"; // Return format description
            }
        }

        public static void Run()
        {
            // Crea opzioni di caricamento CSV
            TxtLoadOptions options = new TxtLoadOptions(LoadFormat.Csv);
            
            // Imposta i parser preferiti - prima prova il parser di stringa personalizzato, poi i parser predefiniti
            options.PreferredParsers = new ICustomParser[] { new StringParser(), null };

            // Dati CSV di esempio con date
            string csvData = "\"2018-10-08\",2018-10-08\n\"2018-10-08\",2018-10-08";
            
            // Carica la cartella di lavoro con opzioni
            Workbook workbook = new Workbook(new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData)), options);
            Cells cells = workbook.Worksheets[0].Cells;

            // Verifica i risultati dell'analisi
            Console.WriteLine("A1 Type: " + cells[0, 0].Type); // Should be string
            Console.WriteLine("A1 Value: " + cells[0, 0].StringValue); // "2018-10-08"
            Console.WriteLine("B1 Type: " + cells[0, 1].Type); // Should be DateTime
            Console.WriteLine("B1 Value: " + cells[0, 1].DateTimeValue); // 10/8/2018
        }
    }
}
```

### Vedi anche

* interface [ICustomParser](../../icustomparser/)
* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


