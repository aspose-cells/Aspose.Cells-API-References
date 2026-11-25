---
title: "NumbersLoadOptions.NumbersLoadOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "NumbersLoadOptions costruttore. Costruttore"
type: docs
url: /it/net/aspose.cells.numbers/numbersloadoptions/numbersloadoptions/
---
## NumbersLoadOptions constructor

Costruttore.

```csharp
public NumbersLoadOptions()
```

### Esempi

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
            // Crea NumbersLoadOptions usando il costruttore
            NumbersLoadOptions loadOptions = new NumbersLoadOptions
            {
                // Imposta alcune proprietà comuni
                Password = "secure123",
                ParsingFormulaOnOpen = true,
                CultureInfo = new CultureInfo("en-US"),
                StandardFont = "Arial",
                MemorySetting = MemorySetting.MemoryPreference
            };

            // Carica la cartella di lavoro con le opzioni
            Workbook workbook = new Workbook("sample.numbers", loadOptions);

            // Salva come XLSX
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [NumbersLoadOptions](../)
* namespace [Aspose.Cells.Numbers](../../../aspose.cells.numbers/)
* assembly [Aspose.Cells](../../../)


