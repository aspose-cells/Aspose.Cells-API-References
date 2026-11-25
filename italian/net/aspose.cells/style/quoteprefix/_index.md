---
title: "Style.QuotePrefix"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Style. Indica se il valore della cella inizia con un apice singolo"
type: docs
url: /it/net/aspose.cells/style/quoteprefix/
---
## Style.QuotePrefix property

Indica se il valore della cella inizia con un apostrofo.

```csharp
public bool QuotePrefix { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyQuotePrefixDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi alla cella B10 e imposta il suo valore
            Cell cell = worksheet.Cells["B10"];
            cell.PutValue("'12345"); // Note the single quote prefix

            // Ottieni lo stile della cella e abilita QuotePrefix
            Style style = cell.GetStyle();
            style.QuotePrefix = true;
            cell.SetStyle(style);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");

            // Verifica la proprietà QuotePrefix
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Cell loadedCell = loadedWorkbook.Worksheets[0].Cells["B10"];
            Console.WriteLine("QuotePrefix is set: " + loadedCell.GetStyle().QuotePrefix);
        }
    }
}
```

### Vedi anche

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


