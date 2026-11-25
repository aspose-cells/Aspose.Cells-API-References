---
title: "LowCodeSplitOptions.LoadOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LowCodeSplitOptions. Opzioni di caricamento per caricare il foglio di calcolo che verrà diviso"
type: docs
url: /it/net/aspose.cells.lowcode/lowcodesplitoptions/loadoptions/
---
## LowCodeSplitOptions.LoadOptions property

Opzioni di caricamento per il foglio di calcolo che verrà diviso.

```csharp
public LowCodeLoadOptions LoadOptions { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSplitOptionsPropertyLoadOptionsDemo
    {
        public static void Run()
        {
            // Crea un'istanza delle opzioni di divisione
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();

            // Inizializza le opzioni di caricamento
            splitOptions.LoadOptions = new LowCodeLoadOptions();

            // Crea nuove opzioni di caricamento con impostazioni diverse (utilizzando le proprietà disponibili)
            splitOptions.LoadOptions = new LowCodeLoadOptions();
            
            // Dimostra la configurazione finale
            Console.WriteLine("LoadOptions configured with InputFile: " + splitOptions.LoadOptions.InputFile);
        }
    }
}
```

### Vedi anche

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSplitOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


