---
title: "NumbersLoadOptions.LoadTableType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "NumbersLoadOptions‑egenskap. Hämtar och anger typen av inläsning av flera tabeller i ett kalkylblad"
type: docs
url: /sv/net/aspose.cells.numbers/numbersloadoptions/loadtabletype/
---
## NumbersLoadOptions.LoadTableType property

Hämtar och anger typen av inläsning av flera tabeller i ett arbetsblad.

```csharp
public LoadNumbersTableType LoadTableType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Numbers;

namespace AsposeCellsExamples
{
    public class NumbersLoadOptionsPropertyLoadTableTypeDemo
    {
        public static void Run()
        {
            // Skapa en instans av NumbersLoadOptions
            NumbersLoadOptions loadOptions = new NumbersLoadOptions
            {
                // Demonstrera användning av LoadTableType‑egenskapen
                LoadTableType = LoadNumbersTableType.OneTablePerSheet,
                
                // Andra minimala nödvändiga egenskaper
                Password = "password123",
                ParsingFormulaOnOpen = true
            };

            // Läs in en Numbers-fil med de angivna inläsningsalternativen
            Workbook workbook = new Workbook("sample.numbers", loadOptions);

            // Spara arbetsboken i XLSX-format
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* enum [LoadNumbersTableType](../../loadnumberstabletype/)
* class [NumbersLoadOptions](../)
* namespace [Aspose.Cells.Numbers](../../../aspose.cells.numbers/)
* assembly [Aspose.Cells](../../../)


