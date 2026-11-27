---
title: "LoadOptions.ParsingFormulaOnOpen"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LoadOptions egenskap. Anger om formeln ska parsas när filen läses"
type: docs
url: /sv/net/aspose.cells/loadoptions/parsingformulaonopen/
---
## LoadOptions.ParsingFormulaOnOpen property

Anger om formeln ska parsas när filen läses.

```csharp
public bool ParsingFormulaOnOpen { get; set; }
```

### Anmärkningar

Gäller endast för Excel-filerna Xlsx, Xltx, Xltm och Xlsm eftersom formlerna i filerna lagras som en strängformel.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyParsingFormulaOnOpenDemo
    {
        public static void Run()
        {
            // Skapa laddningsalternativ
            LoadOptions loadOptions = new LoadOptions();
            
            // Ställ in ParsingFormulaOnOpen till false för att hoppa över formelparsning under inläsning
            loadOptions.ParsingFormulaOnOpen = false;
            
            // Läs in arbetsboken med de angivna alternativen
            Workbook workbook = new Workbook("example.xlsm", loadOptions);
            
            // Kom åt kalkylbladet och visa att formelparsning hoppades över
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            Console.WriteLine("Cell A1 formula: " + cell.Formula);
            Console.WriteLine("Cell A1 value: " + cell.Value);
        }
    }
}
```

### Se även

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


