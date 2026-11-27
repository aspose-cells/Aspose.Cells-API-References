---
title: "NumbersLoadOptions.NumbersLoadOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "NumbersLoadOptions‑konstruktor. Konstruktor"
type: docs
url: /sv/net/aspose.cells.numbers/numbersloadoptions/numbersloadoptions/
---
## NumbersLoadOptions constructor

Konstruktor.

```csharp
public NumbersLoadOptions()
```

### Exempel

```csharp
using System;
using System.Globalization;
using Aspose.Cells;
using Aspose.Cells.Numbers;

namespace AsposeCellsExamples
{
    public class NumbersLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Skapa NumbersLoadOptions med hjälp av konstruktorn
            NumbersLoadOptions loadOptions = new NumbersLoadOptions
            {
                // Ställ in några vanliga egenskaper
                Password = "secure123",
                ParsingFormulaOnOpen = true,
                CultureInfo = new CultureInfo("en-US"),
                StandardFont = "Arial",
                MemorySetting = MemorySetting.MemoryPreference
            };

            // Läs in arbetsboken med alternativen
            Workbook workbook = new Workbook("sample.numbers", loadOptions);

            // Spara som XLSX
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [NumbersLoadOptions](../)
* namespace [Aspose.Cells.Numbers](../../../aspose.cells.numbers/)
* assembly [Aspose.Cells](../../../)


