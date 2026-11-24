---
title: "NumbersLoadOptions.NumbersLoadOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "NumbersLoadOptions-Konstruktor. Konstruktor"
type: docs
url: /de/net/aspose.cells.numbers/numbersloadoptions/numbersloadoptions/
---
## NumbersLoadOptions constructor

Konstruktor.

```csharp
public NumbersLoadOptions()
```

### Beispiele

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
            // Erstellen Sie NumbersLoadOptions mithilfe des Konstruktors
            NumbersLoadOptions loadOptions = new NumbersLoadOptions
            {
                // Setzen Sie einige gängige Eigenschaften
                Password = "secure123",
                ParsingFormulaOnOpen = true,
                CultureInfo = new CultureInfo("en-US"),
                StandardFont = "Arial",
                MemorySetting = MemorySetting.MemoryPreference
            };

            // Lade die Arbeitsmappe mit den Optionen
            Workbook workbook = new Workbook("sample.numbers", loadOptions);

            // Als XLSX speichern
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [NumbersLoadOptions](../)
* namespace [Aspose.Cells.Numbers](../../../aspose.cells.numbers/)
* assembly [Aspose.Cells](../../../)


