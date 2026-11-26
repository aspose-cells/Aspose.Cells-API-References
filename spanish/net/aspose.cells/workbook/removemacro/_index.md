---
title: "Workbook.RemoveMacro"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Workbook. Elimina VBA/macros de esta hoja de cálculo"
type: docs
url: /es/net/aspose.cells/workbook/removemacro/
---
## Workbook.RemoveMacro method

Elimina VBA/macros de esta hoja de cálculo.

```csharp
public void RemoveMacro()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRemoveMacroDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo a partir de un archivo con macros habilitadas
            Workbook workbook = new Workbook("example.xlsm");

            // Eliminar macros del libro de trabajo
            workbook.RemoveMacro();
            
            // Guardar como libro de trabajo sin macros
            string noMacroPath = "NoMacro.xlsx";
            workbook.Save(noMacroPath, SaveFormat.Xlsx);

            Console.WriteLine("Macros removed successfully. File created: " + noMacroPath);
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


