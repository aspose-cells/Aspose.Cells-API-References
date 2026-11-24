---
title: "Workbook.HasMacro"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook‑Eigenschaft. Gibt an, ob diese Tabelle Makros/VBA enthält."
type: docs
url: /de/net/aspose.cells/workbook/hasmacro/
---
## Workbook.HasMacro property

Gibt an, ob diese Tabelle Makros/VBA enthält.

```csharp
public bool HasMacro { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyHasMacroDemo
    {
        public static void Run()
        {
            // Eine Arbeitsmappe mit Makro erstellen, indem eine Vorlagendatei geladen wird.
            Workbook workbookWithMacro = new Workbook("sample_with_macro.xlsm");
            Console.WriteLine("Workbook with macro - HasMacro: " + workbookWithMacro.HasMacro);

            // Eine Arbeitsmappe ohne Makro erstellen.
            Workbook workbookWithoutMacro = new Workbook();
            Console.WriteLine("Workbook without macro - HasMacro: " + workbookWithoutMacro.HasMacro);
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


