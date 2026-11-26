---
title: "Clase SpreadsheetLocker"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.LowCode.SpreadsheetLocker. API de bajo código para bloquear el archivo de hoja de cálculo"
type: docs
url: /es/net/aspose.cells.lowcode/spreadsheetlocker/
---
## SpreadsheetLocker class

API de bajo código para bloquear archivos de hoja de cálculo.

```csharp
public class SpreadsheetLocker
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/spreadsheetlocker/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions, AbstractLowCodeProtectionProvider) | Bloquea el archivo de hoja de cálculo con la configuración especificada. |
| static [Process](../../aspose.cells.lowcode/spreadsheetlocker/process/#process_1)(LowCodeLoadOptions, LowCodeSaveOptions, string, string) | Bloquea el archivo de hoja de cálculo con la configuración especificada. |
| static [Process](../../aspose.cells.lowcode/spreadsheetlocker/process/#process_3)(string, string, string, string) | Bloquea el archivo de hoja de cálculo con la configuración especificada. |
| static [Process](../../aspose.cells.lowcode/spreadsheetlocker/process/#process_2)(LowCodeLoadOptions, LowCodeSaveOptions, string, string, string, ProtectionType) | Bloquea el archivo de hoja de cálculo con la configuración especificada. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassSpreadsheetLockerDemo
    {
        public static void Run()
        {
            // Usar SpreadsheetLocker para proteger el libro de trabajo
            SpreadsheetLocker.Process("template.xlsx", "locked.xlsx", "mypassword", "mypassword");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


