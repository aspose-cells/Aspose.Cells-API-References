---
title: "VbaModule.Codes"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà VbaModule. Ottiene e imposta i codici del modulo"
type: docs
url: /it/net/aspose.cells.vba/vbamodule/codes/
---
## VbaModule.Codes property

Ottiene e imposta i codici del modulo.

```csharp
public string Codes { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModulePropertyCodesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un modulo VBA
            int index = workbook.VbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
            Aspose.Cells.Vba.VbaModule module = workbook.VbaProject.Modules[index];
            
            // Imposta il codice iniziale
            module.Codes = "Sub TestMacro()\n    MsgBox \"Hello World\"\nEnd Sub";
            
            // Modifica il codice aggiungendo nuove righe
            module.Codes = module.Codes + "\nSub AnotherMacro()\n    MsgBox \"Second Macro\"\nEnd Sub";
            
            // Salva la cartella di lavoro
            workbook.Save("VbaModuleDemo.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### Vedi anche

* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


