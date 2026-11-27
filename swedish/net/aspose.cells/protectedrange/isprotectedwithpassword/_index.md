---
title: "ProtectedRange.IsProtectedWithPassword"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ProtectedRange-egenskap. Anger om kalkylbladet är skyddat med lösenord"
type: docs
url: /sv/net/aspose.cells/protectedrange/isprotectedwithpassword/
---
## ProtectedRange.IsProtectedWithPassword property

Anger om kalkylbladen är skyddade med lösenord.

```csharp
public bool IsProtectedWithPassword { get; }
```

### Exempel

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
            
            // Skapa skyddade områden och hämta deras index
            int protectedIndex = worksheet.AllowEditRanges.Add("PasswordProtected", 0, 0, 5, 5);
            ProtectedRange protectedWithPassword = worksheet.AllowEditRanges[protectedIndex];
            protectedWithPassword.Password = "test123";
            
            int unprotectedIndex = worksheet.AllowEditRanges.Add("Unprotected", 6, 0, 11, 5);
            ProtectedRange unprotected = worksheet.AllowEditRanges[unprotectedIndex];
            
            // Skydda kalkylbladet för att verkställa begränsningar
            worksheet.Protect(ProtectionType.All);
            
            // Verifiera status för lösenordsskydd
            Console.WriteLine($"Range '{protectedWithPassword.Name}' password protected: {protectedWithPassword.IsProtectedWithPassword}");
            Console.WriteLine($"Range '{unprotected.Name}' password protected: {unprotected.IsProtectedWithPassword}");
        }
    }
}
```

### Se även

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


