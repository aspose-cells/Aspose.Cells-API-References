---
title: "LoadOptions.Region"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LoadOptions egenskap. Hämtar eller anger de regionala inställningarna som används för arbetsboken som ska läsas in"
type: docs
url: /sv/net/aspose.cells/loadoptions/region/
---
## LoadOptions.Region property

Hämtar eller anger de regionala inställningarna som används för Workbook som ska laddas.

```csharp
public CountryCode Region { get; set; }
```

### Anmärkningar

De regionala inställningarna kan användas för att initiera vissa funktioner i arbetsboken, såsom teckensnitt, teman osv. För textbaserade filformat, såsom CSV, HTML, …, kommer de regionala inställningarna också att användas för att upptäcka talformat och tolka textvärden till numeriska eller datum‑/tidvärden för celler. Denna inställning kommer att behållas för den instansierade arbetsboken senare, det vill säga, [`Region`](../../workbooksettings/region/) för arbetsboken kommer att använda samma region som denna egenskap.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyRegionDemo
    {
        public static void Run()
        {
            // Skapa inläsningsalternativ för HTML‑fil
            LoadOptions loadOpts = new LoadOptions(LoadFormat.Html);
            
            // Ställ in regionen till USA
            loadOpts.Region = CountryCode.USA;
            
            // Läs in HTML‑filen med de angivna regionsinställningarna
            Workbook wb = new Workbook("example.html", loadOpts);
            
            // Åtkomst till det första kalkylbladet
            Worksheet ws = wb.Worksheets[0];
            
            // Demonstrera regionsspecifik formatering genom att kontrollera en cells stil
            Style style = ws.Cells["A1"].GetStyle();
            Console.WriteLine("Font used in cell A1: " + style.Font.Name);
            Console.WriteLine("Region used for loading: " + loadOpts.Region);
        }
    }
}
```

### Se även

* enum [CountryCode](../../countrycode/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


