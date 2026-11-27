---
title: "HtmlLoadOptions.SupportDivTag"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlLoadOptions egenskap. Anger om layouten för div-taggen ska stödjas när HTML-filen innehåller den. Standardvärdet är falskt"
type: docs
url: /sv/net/aspose.cells/htmlloadoptions/supportdivtag/
---
## HtmlLoadOptions.SupportDivTag property

Anger om layouten för `<div>`-taggen stöds när html-filen innehåller den. Standardvärdet är false.

```csharp
public bool SupportDivTag { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertySupportDivTagDemo
    {
        public static void Run()
        {
            // Skapa HTML-inläsningsalternativ med SupportDivTag aktiverat
            HtmlLoadOptions htmlLoadOptions = new HtmlLoadOptions(LoadFormat.Html);
            htmlLoadOptions.SupportDivTag = true;

            // Läs in HTML-fil med div-taggar
            Workbook workbook = new Workbook("input.html", htmlLoadOptions);

            // Åtkomst till data från det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            // Utdata cellvärde och stilinformation
            Console.WriteLine("Cell A1 value: " + cell.StringValue);
            Console.WriteLine("Is bold: " + cell.GetStyle().Font.IsBold);

            // Spara som Excel-fil
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


