---
title: "WriteProtection.ValidatePassword"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo WriteProtection. Restituisce true se la password specificata è la stessa della password di protezione con cui il file è stato protetto"
type: docs
url: /it/net/aspose.cells/writeprotection/validatepassword/
---
## WriteProtection.ValidatePassword method

Restituisce true se la password specificata è la stessa della password di protezione in scrittura con cui il file è stato protetto.

```csharp
public bool ValidatePassword(string password)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| password | String | La password specificata. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WriteProtectionMethodValidatePasswordWithStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Imposta la password di protezione dalla scrittura
            workbook.Settings.WriteProtection.Password = "1234";
            
            // Convalida password
            Console.WriteLine("Password '1234' is valid: " + 
                workbook.Settings.WriteProtection.ValidatePassword("1234"));
            Console.WriteLine("Password 'wrong' is valid: " + 
                workbook.Settings.WriteProtection.ValidatePassword("wrong"));
        }
    }
}
```

### Vedi anche

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


