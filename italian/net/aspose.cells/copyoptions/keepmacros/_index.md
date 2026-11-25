---
title: "CopyOptions.KeepMacros"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CopyOptions. Indica se mantenere le macro"
type: docs
url: /it/net/aspose.cells/copyoptions/keepmacros/
---
## CopyOptions.KeepMacros property

Indica se mantenere le macro;

```csharp
public bool KeepMacros { get; set; }
```

### Osservazioni

Solo per la copia della cartella di lavoro.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyKeepMacrosDemo
    {
        public static void Run()
        {
            // Crea la cartella di lavoro di origine con macro (usando un file modello che contiene macro)
            Workbook srcWorkbook = new Workbook("macros_template.xlsm");
            Worksheet srcSheet = srcWorkbook.Worksheets[0];
            srcSheet.Cells["A1"].PutValue("Macro-enabled source");

            // Crea la cartella di lavoro di destinazione
            Workbook destWorkbook = new Workbook();
            
            // Imposta le opzioni di copia con KeepMacros true
            CopyOptions options = new CopyOptions();
            options.KeepMacros = true;

            // Copia il foglio di lavoro con macro
            destWorkbook.Worksheets[0].Copy(srcSheet, options);

            // Salva il risultato
            destWorkbook.Save("KeepMacrosExample.xlsm");
        }
    }
}
```

### Vedi anche

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


