---
title: "VbaProject.IsValidSigned"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà VbaProject. Indica se la firma del progetto VBA è valida o meno"
type: docs
url: /it/net/aspose.cells.vba/vbaproject/isvalidsigned/
---
## VbaProject.IsValidSigned property

Indica se la firma del progetto VBA è valida o meno.

```csharp
public bool IsValidSigned { get; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyIsValidSignedDemo
    {
        public static void Run()
        {
            // Carica una cartella di lavoro di esempio con progetto VBA firmato
            Workbook wb = new Workbook("example.xlsm");
            
            // Verifica se il progetto VBA è firmato e se la firma è valida
            Console.WriteLine("Is VBA Project Signed: " + wb.VbaProject.IsSigned);
            Console.WriteLine("Is Signature Valid: " + wb.VbaProject.IsValidSigned);

            // Salva e ricarica per verificare che la firma persista
            MemoryStream ms = new MemoryStream();
            wb.Save(ms, SaveFormat.Excel97To2003);
            
            Workbook validateWb = new Workbook(ms);
            Console.WriteLine("After Reload - Is VBA Project Signed: " + validateWb.VbaProject.IsSigned);
            Console.WriteLine("After Reload - Is Signature Valid: " + validateWb.VbaProject.IsValidSigned);
        }
    }
}
```

### Vedi anche

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


