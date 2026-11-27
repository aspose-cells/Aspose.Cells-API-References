---
title: "LoadOptions.AutoFilter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LoadOptions egenskap. Anger om data automatiskt filtreras när filerna laddas"
type: docs
url: /sv/net/aspose.cells/loadoptions/autofilter/
---
## LoadOptions.AutoFilter property

Indikerar om data automatiskt filtreras vid inläsning av filerna.

```csharp
public bool AutoFilter { get; set; }
```

### Anmärkningar

Ibland, även om autofilter är aktiverat, döljs de motsvarande raderna inte i filen. Fungerar nu endast för SpreadSheetML-filer.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyAutoFilterDemo
    {
        public static void Run()
        {
            // Skapa laddningsalternativ och aktivera AutoFilter
            LoadOptions options = new LoadOptions();
            options.AutoFilter = true;

            // Läs in arbetsbok med AutoFilter aktiverat
            Workbook workbook = new Workbook("example.xlsx", options);

            // Kom åt det första kalkylbladet och tillämpa AutoFilter
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.AutoFilter.Range = "A1:D10";
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


