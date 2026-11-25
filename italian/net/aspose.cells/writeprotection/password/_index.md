---
title: "WriteProtection.Password"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WriteProtection. Imposta la password di protezione per modificare il file"
type: docs
url: /it/net/aspose.cells/writeprotection/password/
---
## WriteProtection.Password property

Imposta la password di protezione per modificare il file.

```csharp
public string Password { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WriteProtectionPropertyPasswordDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta la password di protezione dalla scrittura
            workbook.Settings.WriteProtection.Password = "owner";
            
            // Salva la cartella di lavoro
            workbook.Save("WriteProtectedWorkbook.xlsx");
            
            Console.WriteLine("Workbook write-protected with password successfully.");
        }
    }
}
```

### Vedi anche

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


