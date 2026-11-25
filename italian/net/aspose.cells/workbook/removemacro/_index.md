---
title: "Workbook.RemoveMacro"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Workbook method. Rimuove VBA/macro da questo foglio di calcolo"
type: docs
url: /it/net/aspose.cells/workbook/removemacro/
---
## Workbook.RemoveMacro method

Rimuove VBA/macro da questo foglio di calcolo.

```csharp
public void RemoveMacro()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRemoveMacroDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro da un file esistente con macro
            Workbook workbook = new Workbook("example.xlsm");

            // Rimuovi le macro dalla cartella di lavoro
            workbook.RemoveMacro();
            
            // Salva come cartella di lavoro senza macro
            string noMacroPath = "NoMacro.xlsx";
            workbook.Save(noMacroPath, SaveFormat.Xlsx);

            Console.WriteLine("Macros removed successfully. File created: " + noMacroPath);
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


