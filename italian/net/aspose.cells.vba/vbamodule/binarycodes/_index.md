---
title: "VbaModule.BinaryCodes"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà VbaModule. Ottiene e imposta i codici binari del modulo"
type: docs
url: /it/net/aspose.cells.vba/vbamodule/binarycodes/
---
## VbaModule.BinaryCodes property

Ottiene e imposta i codici binari del modulo.

```csharp
public byte[] BinaryCodes { get; }
```

### Esempi

```csharp
using System;
using System.Text;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModulePropertyBinaryCodesDemo
    {
        public static void Run()
        {
            // Carica la cartella di lavoro con il progetto VBA
            Workbook workbook = new Workbook("example.xlsm");
            
            // Accedi al progetto VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            // Ottieni i codici binari dal primo modulo
            byte[] binaryCodes = vbaProject.Modules[0].BinaryCodes;
            
            // Converti in stringa usando la codifica cinese (936)
            string codeContent = Encoding.GetEncoding(936).GetString(binaryCodes);
            
            // Stampa il contenuto contenente caratteri cinesi
            Console.WriteLine("VBA Module Content:");
            Console.WriteLine(codeContent);
        }
    }
}
```

### Vedi anche

* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


