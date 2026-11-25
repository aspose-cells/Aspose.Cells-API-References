---
title: "Enum VbaModuleType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Vba.VbaModuleType. Rappresenta il tipo di modulo VBA"
type: docs
url: /it/net/aspose.cells.vba/vbamoduletype/
---
## VbaModuleType enumeration

Rappresenta il tipo di modulo VBA.

```csharp
public enum VbaModuleType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Procedural | `0` | Rappresenta un modulo procedurale. |
| Document | `1` | Rappresenta un modulo documento. |
| Class | `2` | Rappresenta un modulo classe. |
| Designer | `3` | Rappresenta un modulo designer. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaModuleTypeDemo
    {
        public static void VbaModuleTypeExample()
        {
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();
            
            // Inizializza progetto VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            // Aggiungi un nuovo modulo di classe
            int index = vbaProject.Modules.Add(VbaModuleType.Class, "test");
            
            // Ottieni il modulo VBA
            VbaModule vbaModule = vbaProject.Modules[index];
            
            // Imposta i codici per il modulo
            vbaModule.Codes = "Sub ShowMessage()\r\nMsgBox \"Welcome to Aspose!\"\r\nEnd Sub";
            
            // Salva il file Excel
            workbook.Save("VbaModuleTypeExample.xlsm");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


