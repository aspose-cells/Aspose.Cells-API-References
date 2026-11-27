---
title: "LoadOptions.LanguageCode"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LoadOptions egenskap. Hämtar eller anger gränssnittsspråket för arbetsboksversionen baserat på CountryCode som har sparat filen"
type: docs
url: /sv/net/aspose.cells/loadoptions/languagecode/
---
## LoadOptions.LanguageCode property

Hämtar eller anger användargränssnittsspråket för arbetsbokens version baserat på landskoden som har sparat filen.

```csharp
public CountryCode LanguageCode { get; set; }
```

### Exempel

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyLanguageCodeDemo
    {
        public static void Run()
        {
            // Skapa en instans av LoadOptions
            LoadOptions loadOptions = new LoadOptions();

            // Ställ in LanguageCode-egenskapen
            loadOptions.LanguageCode = CountryCode.USA;

            // Läs in en arbetsbok med de angivna LoadOptions
            Workbook workbook = new Workbook("sample.xlsx", loadOptions);

            // Kom åt kalkylbladet och ändra innehållet
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Language Code Demo");

            // Spara den modifierade arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* enum [CountryCode](../../countrycode/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


