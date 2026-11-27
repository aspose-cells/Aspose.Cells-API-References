---
title: "StyleFlag.QuotePrefix"
second_title: "Aspose.Cells för .NET API‑referens"
description: "StyleFlag property. Inställning för att dölja formel kommer att tillämpas"
type: docs
url: /sv/net/aspose.cells/styleflag/quoteprefix/
---
## StyleFlag.QuotePrefix property

Inställning för att dölja formel kommer att tillämpas.

```csharp
public bool QuotePrefix { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyQuotePrefixDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Få åtkomst till cell A1 och sätt ett värde som ser ut som ett tal men ska behandlas som text
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("123456");

            // Skapa en stil och sätt QuotePrefix till true
            Style style = workbook.CreateStyle();
            style.QuotePrefix = true;

            // Skapa en stilflagga och aktivera QuotePrefix-flaggan
            StyleFlag flag = new StyleFlag();
            flag.QuotePrefix = true;

            // Tillämpa stilen på cellen med SetStyle istället för ApplyStyle
            cell.SetStyle(style, flag);

            // Visa det aktuella QuotePrefix-värdet
            Console.WriteLine("Current QuotePrefix value: " + cell.GetStyle().QuotePrefix);

            // Spara arbetsboken för att se effekten (värdet kommer att behandlas som text i Excel)
            workbook.Save("PropertyQuotePrefixDemo.xlsx");

            // Nu ändrar vi QuotePrefix till false och ser skillnaden
            style.QuotePrefix = false;
            cell.SetStyle(style, flag);

            Console.WriteLine("Current QuotePrefix value: " + cell.GetStyle().QuotePrefix);
            // Spara igen med ett annat namn för att jämföra
            workbook.Save("PropertyQuotePrefixDemo_WithoutPrefix.xlsx");
        }
    }
}
```

### Se även

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


