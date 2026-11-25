---
title: "WorkbookSettings.QuotePrefixToStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Indica se impostare la proprietà QuotePrefix quando si inserisce il valore stringa che inizia con il carattere di apice singolo nella cella"
type: docs
url: /it/net/aspose.cells/workbooksettings/quoteprefixtostyle/
---
## WorkbookSettings.QuotePrefixToStyle property

Indica se impostare la proprietà [`QuotePrefix`](../../style/quoteprefix/) quando si inserisce il valore stringa (che inizia con il carattere di apice singolo) nella cella

```csharp
public bool QuotePrefixToStyle { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyQuotePrefixToStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Abilita QuotePrefixToStyle - le stringhe che iniziano con ' avranno applicato lo stile QuotePrefix
            workbook.Settings.QuotePrefixToStyle = true;
            Cell cell1 = workbook.Worksheets[0].Cells["A1"];
            cell1.PutValue("'abc");
            Console.WriteLine("Cell A1 - QuotePrefix: " + cell1.GetStyle().QuotePrefix);
            Console.WriteLine("Cell A1 - Value: " + cell1.StringValue);

            // Disabilita QuotePrefixToStyle - le stringhe mantengono il loro valore letterale
            workbook.Settings.QuotePrefixToStyle = false;
            Cell cell2 = workbook.Worksheets[0].Cells["A2"];
            cell2.PutValue("'abc");
            Console.WriteLine("Cell A2 - QuotePrefix: " + cell2.GetStyle().QuotePrefix);
            Console.WriteLine("Cell A2 - Value: " + cell2.StringValue);

            workbook.Save("QuotePrefixToStyleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


