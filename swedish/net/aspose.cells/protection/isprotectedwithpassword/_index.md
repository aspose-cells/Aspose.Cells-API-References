---
title: "Protection.IsProtectedWithPassword"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Protection-egenskapen. Anger om kalkylbladet är skyddat med lösenord"
type: docs
url: /sv/net/aspose.cells/protection/isprotectedwithpassword/
---
## Protection.IsProtectedWithPassword property

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
    public class ProtectionPropertyIsProtectedWithPasswordDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Åtkomst till arbetsbladsskyddinställningar
            Protection protection = worksheet.Protection;

            // Ange skyddslösenord
            protection.Password = "test123";

            // Kontrollera om kalkylbladet är lösenordsskyddat
            bool isProtectedWithPassword = protection.IsProtectedWithPassword;
            Console.WriteLine("Is worksheet protected with password: " + isProtectedWithPassword);

            // Spara arbetsboken
            workbook.Save("PasswordProtectionDemo.xlsx");
        }
    }
}
```

### Se även

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


