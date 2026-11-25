---
title: "StyleFlag.QuotePrefix"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà StyleFlag. L'impostazione Hide formula verrà applicata"
type: docs
url: /it/net/aspose.cells/styleflag/quoteprefix/
---
## StyleFlag.QuotePrefix property

L'impostazione di nascondi formula sarà applicata.

```csharp
public bool QuotePrefix { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyQuotePrefixDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi alla cella A1 e imposta un valore che sembra un numero ma dovrebbe essere trattato come testo
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("123456");

            // Crea uno stile e imposta QuotePrefix su true
            Style style = workbook.CreateStyle();
            style.QuotePrefix = true;

            // Crea un flag di stile e abilita il flag QuotePrefix
            StyleFlag flag = new StyleFlag();
            flag.QuotePrefix = true;

            // Applica lo stile alla cella usando SetStyle invece di ApplyStyle
            cell.SetStyle(style, flag);

            // Visualizza il valore corrente di QuotePrefix
            Console.WriteLine("Current QuotePrefix value: " + cell.GetStyle().QuotePrefix);

            // Salva la cartella di lavoro per vedere l'effetto (il valore sarà trattato come testo in Excel)
            workbook.Save("PropertyQuotePrefixDemo.xlsx");

            // Ora cambiamo QuotePrefix a false e vediamo la differenza
            style.QuotePrefix = false;
            cell.SetStyle(style, flag);

            Console.WriteLine("Current QuotePrefix value: " + cell.GetStyle().QuotePrefix);
            // Salva di nuovo con un nome diverso per confrontare
            workbook.Save("PropertyQuotePrefixDemo_WithoutPrefix.xlsx");
        }
    }
}
```

### Vedi anche

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


