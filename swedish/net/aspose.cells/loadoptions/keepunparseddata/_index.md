---
title: "LoadOptions.KeepUnparsedData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LoadOptions egenskap. Anger om de oparserade data ska hållas i minnet för arbetsboken när den laddas från mallfil. Standard är sant"
type: docs
url: /sv/net/aspose.cells/loadoptions/keepunparseddata/
---
## LoadOptions.KeepUnparsedData property

Om de oparsade data ska behållas i minnet för Workbook när den laddas från mallfilen. Standard är true.

```csharp
public bool KeepUnparsedData { get; set; }
```

### Anmärkningar

För scenarier där användaren bara behöver läsa vissa innehåll från mallfilen och inte behöver spara arbetsboken igen, kan det förbättra prestandan att sätta denna egenskap till falskt, särskilt när den används tillsammans med någon form av LoadFilter,

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyKeepUnparsedDataDemo
    {
        public static void Run()
        {
            // Skapa laddningsalternativ och sätt KeepUnparsedData till falskt
            LoadOptions options = new LoadOptions();
            options.KeepUnparsedData = false;

            // Läs in arbetsbok med alternativ
            Workbook workbook = new Workbook("example.xlsx", options);

            // Öppna kalkylbladet och demonstrera att oparsa data inte behålls
            Worksheet worksheet = workbook.Worksheets[0];
            Console.WriteLine("Cell A1 value: " + worksheet.Cells["A1"].Value);

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


