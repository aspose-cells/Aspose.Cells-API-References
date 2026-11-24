---
title: "ProtectedRange.IsProtectedWithPassword"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ProtectedRange-Eigenschaft. Gibt an, ob das Arbeitsblatt mit einem Passwort geschützt ist"
type: docs
url: /de/net/aspose.cells/protectedrange/isprotectedwithpassword/
---
## ProtectedRange.IsProtectedWithPassword property

Gibt an, ob das Arbeitsblatt mit einem Passwort geschützt ist.

```csharp
public bool IsProtectedWithPassword { get; }
```

### Beispiele

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
            
            // Erstelle geschützte Bereiche und rufe ihre Indizes ab
            int protectedIndex = worksheet.AllowEditRanges.Add("PasswordProtected", 0, 0, 5, 5);
            ProtectedRange protectedWithPassword = worksheet.AllowEditRanges[protectedIndex];
            protectedWithPassword.Password = "test123";
            
            int unprotectedIndex = worksheet.AllowEditRanges.Add("Unprotected", 6, 0, 11, 5);
            ProtectedRange unprotected = worksheet.AllowEditRanges[unprotectedIndex];
            
            // Schütze das Arbeitsblatt, um Einschränkungen durchzusetzen
            worksheet.Protect(ProtectionType.All);
            
            // Überprüfe den Passwortschutzstatus
            Console.WriteLine($"Range '{protectedWithPassword.Name}' password protected: {protectedWithPassword.IsProtectedWithPassword}");
            Console.WriteLine($"Range '{unprotected.Name}' password protected: {unprotected.IsProtectedWithPassword}");
        }
    }
}
```

### Siehe auch

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


