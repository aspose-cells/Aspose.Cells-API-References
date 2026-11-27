---
title: "TxtSaveOptions.ExportQuotePrefix"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TxtSaveOptions-egenskap. Anger om enkelfnuttstecknet ska exporteras som en del av värdet i en cell när QuotePrefix är true för den. Standard är false."
type: docs
url: /sv/net/aspose.cells/txtsaveoptions/exportquoteprefix/
---
## TxtSaveOptions.ExportQuotePrefix property

Anger om enkelfnuttstecknet ska exporteras som en del av värdet i en cell när [`QuotePrefix`](../../style/quoteprefix/) är true för den. Standard är false.

```csharp
public bool ExportQuotePrefix { get; set; }
```

### Exempel

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
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Lägg till exempeldata med specialtecken
            cells[0, 0].PutValue("a\\bcdef\"g");
            cells[0, 1].PutValue("f\"g");
            cells[0, 2].PutValue("a\\bcdg");
            cells[0, 3].PutValue("abcdefg");
            cells[0, 4].PutValue("efg");
            cells[0, 5].PutValue("'abc");

            // Skapa TXT-sparalternativ
            TxtSaveOptions saveOptions = new TxtSaveOptions
            {
                Encoding = Encoding.ASCII,
                Separator = ',',
                ExportQuotePrefix = true // Demonstrate ExportQuotePrefix property
            };

            // Spara med ExportQuotePrefix = true
            workbook.Save("output_with_exportquoteprefix.csv", saveOptions);

            // Ändra separator och spara igen
            saveOptions.Separator = '\\';
            workbook.Save("output_with_backslash_separator.csv", saveOptions);

            Console.WriteLine("Files saved successfully with ExportQuotePrefix property.");
        }
    }
}
```

### Se även

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


