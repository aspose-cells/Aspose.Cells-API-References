---
title: "Protection.IsProtectedWithPassword"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Protection. Indica se il foglio di lavoro è protetto con password"
type: docs
url: /it/net/aspose.cells/protection/isprotectedwithpassword/
---
## Protection.IsProtectedWithPassword property

Indica se i fogli di lavoro sono protetti da password.

```csharp
public bool IsProtectedWithPassword { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyIsProtectedWithPasswordDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi alle impostazioni di protezione del foglio di lavoro
            Protection protection = worksheet.Protection;

            // Imposta la password di protezione
            protection.Password = "test123";

            // Verifica se il foglio di lavoro è protetto da password
            bool isProtectedWithPassword = protection.IsProtectedWithPassword;
            Console.WriteLine("Is worksheet protected with password: " + isProtectedWithPassword);

            // Salva la cartella di lavoro
            workbook.Save("PasswordProtectionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


