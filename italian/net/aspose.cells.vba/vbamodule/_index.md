---
title: "Classe VbaModule"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Vba.VbaModule. Rappresenta il modulo nel progetto VBA"
type: docs
url: /it/net/aspose.cells.vba/vbamodule/
---
## VbaModule class

Rappresenta il modulo nel progetto VBA.

```csharp
public class VbaModule
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BinaryCodes](../../aspose.cells.vba/vbamodule/binarycodes/) { get; } | Ottiene e imposta i codici binari del modulo. |
| [Codes](../../aspose.cells.vba/vbamodule/codes/) { get; set; } | Ottiene e imposta i codici del modulo. |
| [Name](../../aspose.cells.vba/vbamodule/name/) { get; set; } | Ottiene e imposta il nome del modulo. |
| [Type](../../aspose.cells.vba/vbamodule/type/) { get; } | Ottiene il tipo del modulo. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaModuleDemo
    {
        public static void VbaModuleExample()
        {
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();

            // Inizializza il progetto VBA
            VbaProject vbaProject = workbook.VbaProject;

            // Aggiungi un nuovo modulo
            int index = vbaProject.Modules.Add(VbaModuleType.Class, "test");

            // Ottieni il modulo VBA
            VbaModule vbaModule = vbaProject.Modules[index];

            // Imposta i codici per il modulo
            vbaModule.Codes = "Sub ShowMessage()\r\nMsgBox \"Welcome to Aspose!\"\r\nEnd Sub";

            // Salvataggio del file Excel
            workbook.Save("VbaModuleExample.xlsm");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


