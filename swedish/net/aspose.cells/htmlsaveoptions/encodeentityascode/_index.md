---
title: "HtmlSaveOptions.EncodeEntityAsCode"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions-egenskap. Anger om HTML-teckenentiteter ersätts med decimalkod, t.ex. nbsp ersätts med 160. Standardvärdet är falskt."
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/encodeentityascode/
---
## HtmlSaveOptions.EncodeEntityAsCode property

Anger om html‑teckenentiteter ska ersättas med decimalkod. (t.ex. "&amp;nbsp;" ersätts med "&amp;#160;"). Standardvärdet är false.

```csharp
public bool EncodeEntityAsCode { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class HtmlSaveOptionsPropertyEncodeEntityAsCodeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata med specialtecken
            worksheet.Cells["A1"].PutValue("Sample & Text");
            worksheet.Cells["A2"].PutValue("Another <Test> String");
            worksheet.Cells["A3"].PutValue("Price: $100");

            // Skapa HTML-sparalternativ
            HtmlSaveOptions options = new HtmlSaveOptions();

            // Visa aktuellt värde för EncodeEntityAsCode
            Console.WriteLine("Current EncodeEntityAsCode value: " + options.EncodeEntityAsCode);

            // Ställ in EncodeEntityAsCode till true
            options.EncodeEntityAsCode = true;

            // Spara med entiteter kodade som kod
            workbook.Save("HtmlWithEncodedEntities.html", options);

            // Ställ in EncodeEntityAsCode till false
            options.EncodeEntityAsCode = false;

            // Spara med entiteter oförändrade
            workbook.Save("HtmlWithRawEntities.html", options);

            // Jämför utdatafilerna
            Console.WriteLine("Files created:");
            Console.WriteLine("1. HtmlWithEncodedEntities.html - with encoded entities");
            Console.WriteLine("2. HtmlWithRawEntities.html - with raw entities");
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


