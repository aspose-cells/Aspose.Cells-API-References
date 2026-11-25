---
title: "ProtectedRange.IsProtectedWithPassword"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ProtectedRange. Indica se il foglio di lavoro è protetto con password"
type: docs
url: /it/net/aspose.cells/protectedrange/isprotectedwithpassword/
---
## ProtectedRange.IsProtectedWithPassword property

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
    public class ProtectedRangePropertyIsProtectedWithPasswordDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea intervalli protetti e ottieni i loro indici
            int protectedIndex = worksheet.AllowEditRanges.Add("PasswordProtected", 0, 0, 5, 5);
            ProtectedRange protectedWithPassword = worksheet.AllowEditRanges[protectedIndex];
            protectedWithPassword.Password = "test123";
            
            int unprotectedIndex = worksheet.AllowEditRanges.Add("Unprotected", 6, 0, 11, 5);
            ProtectedRange unprotected = worksheet.AllowEditRanges[unprotectedIndex];
            
            // Proteggi il foglio di lavoro per applicare le restrizioni
            worksheet.Protect(ProtectionType.All);
            
            // Verifica lo stato della protezione con password
            Console.WriteLine($"Range '{protectedWithPassword.Name}' password protected: {protectedWithPassword.IsProtectedWithPassword}");
            Console.WriteLine($"Range '{unprotected.Name}' password protected: {unprotected.IsProtectedWithPassword}");
        }
    }
}
```

### Vedi anche

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


