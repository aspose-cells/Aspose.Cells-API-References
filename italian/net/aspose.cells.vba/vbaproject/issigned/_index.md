---
title: "VbaProject.IsSigned"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà VbaProject. Indica se il codice VBA è firmato o meno"
type: docs
url: /it/net/aspose.cells.vba/vbaproject/issigned/
---
## VbaProject.IsSigned property

Indica se il codice VBA è firmato o meno.

```csharp
public bool IsSigned { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyIsSignedDemo
    {
        public static void Run()
        {
            // Carica un file Excel di esempio con progetto VBA
            Workbook workbook = new Workbook("example.xlsm");
            
            // Verifica se il progetto VBA è firmato
            if (workbook.VbaProject.IsSigned)
            {
                Console.WriteLine("VBA project is signed.");
                Console.WriteLine("Signature is valid: " + workbook.VbaProject.IsValidSigned);
            }
            else
            {
                Console.WriteLine("VBA project is not signed.");
            }
        }
    }
}
```

### Vedi anche

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


