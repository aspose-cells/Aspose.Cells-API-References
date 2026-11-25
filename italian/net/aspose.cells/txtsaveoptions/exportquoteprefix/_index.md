---
title: "TxtSaveOptions.ExportQuotePrefix"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TxtSaveOptions. Indica se il segno di apice singolo deve essere esportato come parte del valore di una cella quando QuotePrefix è true per essa. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/txtsaveoptions/exportquoteprefix/
---
## TxtSaveOptions.ExportQuotePrefix property

Indica se il segno di apice singolo deve essere esportato come parte del valore di una cella quando [`QuotePrefix`](../../style/quoteprefix/) è true per essa. Il valore predefinito è false.

```csharp
public bool ExportQuotePrefix { get; set; }
```

### Esempi

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyExportQuotePrefixDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Aggiungi dati di esempio con caratteri speciali
            cells[0, 0].PutValue("a\\bcdef\"g");
            cells[0, 1].PutValue("f\"g");
            cells[0, 2].PutValue("a\\bcdg");
            cells[0, 3].PutValue("abcdefg");
            cells[0, 4].PutValue("efg");
            cells[0, 5].PutValue("'abc");

            // Crea le opzioni di salvataggio TXT
            TxtSaveOptions saveOptions = new TxtSaveOptions
            {
                Encoding = Encoding.ASCII,
                Separator = ',',
                ExportQuotePrefix = true // Demonstrate ExportQuotePrefix property
            };

            // Salva con ExportQuotePrefix = true
            workbook.Save("output_with_exportquoteprefix.csv", saveOptions);

            // Modifica il separatore e salva di nuovo
            saveOptions.Separator = '\\';
            workbook.Save("output_with_backslash_separator.csv", saveOptions);

            Console.WriteLine("Files saved successfully with ExportQuotePrefix property.");
        }
    }
}
```

### Vedi anche

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


