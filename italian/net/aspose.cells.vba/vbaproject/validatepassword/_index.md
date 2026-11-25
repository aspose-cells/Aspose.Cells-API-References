---
title: "VbaProject.ValidatePassword"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo VbaProject. Convalida la password di protezione"
type: docs
url: /it/net/aspose.cells.vba/vbaproject/validatepassword/
---
## VbaProject.ValidatePassword method

Convalida la password di protezione.

```csharp
public bool ValidatePassword(string password)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| password | String | la password |

### Valore di ritorno

Indica se la password è la password di protezione di questo progetto VBA

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaProjectMethodValidatePasswordWithStringDemo
    {
        public static void Run()
        {
            // Crea un oggetto cartella di lavoro dal file Excel di esempio con progetto VBA
            Workbook workbook = new Workbook("example.xlsm");
            
            // Convalida la password del progetto VBA
            bool isValid = workbook.VbaProject.ValidatePassword("test");
            
            // Restituisci il risultato della convalida
            Console.WriteLine("Password validation result: " + isValid);
        }
    }
}
```

### Vedi anche

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


