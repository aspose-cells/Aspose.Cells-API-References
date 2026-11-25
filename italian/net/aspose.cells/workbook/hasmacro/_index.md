---
title: "Workbook.HasMacro"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Workbook. Indica se questo foglio di calcolo contiene macro/VBA"
type: docs
url: /it/net/aspose.cells/workbook/hasmacro/
---
## Workbook.HasMacro property

Indica se questo foglio di calcolo contiene macro/VBA.

```csharp
public bool HasMacro { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyHasMacroDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con macro caricando un file modello
            Workbook workbookWithMacro = new Workbook("sample_with_macro.xlsm");
            Console.WriteLine("Workbook with macro - HasMacro: " + workbookWithMacro.HasMacro);

            // Crea una cartella di lavoro senza macro
            Workbook workbookWithoutMacro = new Workbook();
            Console.WriteLine("Workbook without macro - HasMacro: " + workbookWithoutMacro.HasMacro);
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


