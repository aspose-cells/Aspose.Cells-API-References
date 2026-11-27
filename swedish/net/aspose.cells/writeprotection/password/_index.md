---
title: "WriteProtection.Password"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WriteProtection-egenskapen. Anger det skyddade lösenordet för att ändra filen"
type: docs
url: /sv/net/aspose.cells/writeprotection/password/
---
## WriteProtection.Password property

Anger det skyddade lösenordet för att ändra filen.

```csharp
public string Password { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WriteProtectionPropertyPasswordDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ange lösenord för skrivskydd
            workbook.Settings.WriteProtection.Password = "owner";
            
            // Spara arbetsboken
            workbook.Save("WriteProtectedWorkbook.xlsx");
            
            Console.WriteLine("Workbook write-protected with password successfully.");
        }
    }
}
```

### Se även

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


