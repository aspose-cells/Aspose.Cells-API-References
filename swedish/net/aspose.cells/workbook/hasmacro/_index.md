---
title: "Workbook.HasMacro"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-egenskap. Anger om detta kalkylblad innehåller makro/VBA"
type: docs
url: /sv/net/aspose.cells/workbook/hasmacro/
---
## Workbook.HasMacro property

Anger om detta kalkylblad innehåller makro/VBA.

```csharp
public bool HasMacro { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyHasMacroDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med makro genom att ladda en mallfil
            Workbook workbookWithMacro = new Workbook("sample_with_macro.xlsm");
            Console.WriteLine("Workbook with macro - HasMacro: " + workbookWithMacro.HasMacro);

            // Skapa en arbetsbok utan makro
            Workbook workbookWithoutMacro = new Workbook();
            Console.WriteLine("Workbook without macro - HasMacro: " + workbookWithoutMacro.HasMacro);
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


