---
title: "Workbook.HasMacro"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Workbook. Indica si esta hoja de cálculo contiene macro/VBA"
type: docs
url: /es/net/aspose.cells/workbook/hasmacro/
---
## Workbook.HasMacro property

Indica si esta hoja de cálculo contiene macro/VBA.

```csharp
public bool HasMacro { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyHasMacroDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con macro cargando un archivo de plantilla
            Workbook workbookWithMacro = new Workbook("sample_with_macro.xlsm");
            Console.WriteLine("Workbook with macro - HasMacro: " + workbookWithMacro.HasMacro);

            // Crear un libro de trabajo sin macro
            Workbook workbookWithoutMacro = new Workbook();
            Console.WriteLine("Workbook without macro - HasMacro: " + workbookWithoutMacro.HasMacro);
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


