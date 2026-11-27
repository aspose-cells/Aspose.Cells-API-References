---
title: "LoadOptions.CultureInfo"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LoadOptions egenskap. Hämtar eller anger de regionala inställningarna som används för arbetsboken som ska läsas in"
type: docs
url: /sv/net/aspose.cells/loadoptions/cultureinfo/
---
## LoadOptions.CultureInfo property

Hämtar eller anger de regionala inställningarna som används för Workbook som ska laddas.

```csharp
public CultureInfo CultureInfo { get; set; }
```

### Anmärkningar

Denna egenskap har samma effekt som [`Region`](../region/) för att ställa in regionala inställningar.

### Exempel

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyCultureInfoDemo
    {
        public static void Run()
        {
            // Skapa ett exempel på en Excel‑fil
            Workbook sampleWorkbook = new Workbook();
            sampleWorkbook.Worksheets[0].Cells["A1"].PutValue(1234.56);
            sampleWorkbook.Save("sample.xlsx", SaveFormat.Xlsx);

            // Läs in med specifik kultur
            LoadOptions options = new LoadOptions(LoadFormat.Xlsx);
            options.CultureInfo = new CultureInfo("de-DE"); // German culture uses comma as decimal separator
            
            Workbook workbook = new Workbook("sample.xlsx", options);
            Console.WriteLine("Value with German culture: " + workbook.Worksheets[0].Cells["A1"].StringValue);
        }
    }
}
```

### Se även

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


