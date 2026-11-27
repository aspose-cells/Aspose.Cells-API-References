---
title: "Workbook.IsWorkbookProtectedWithPassword"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-egenskap. Anger om struktur eller fönster är skyddade med lösenord"
type: docs
url: /sv/net/aspose.cells/workbook/isworkbookprotectedwithpassword/
---
## Workbook.IsWorkbookProtectedWithPassword property

Anger om struktur eller fönster är skyddade med lösenord.

```csharp
public bool IsWorkbookProtectedWithPassword { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyIsWorkbookProtectedWithPasswordDemo
    {
        public static void Run()
        {
            // Skapa en ny Workbook-instans
            Workbook workbook = new Workbook();

            // Kontrollera om workbook är skyddad med lösenord (bör vara falskt för ny workbook)
            Console.WriteLine("Is Workbook Protected With Password: " + workbook.IsWorkbookProtectedWithPassword);

            // Skydda arbetsboken med ett lösenord
            workbook.Protect(ProtectionType.All, "password123");

            // Kontrollera nu igen (bör vara sant)
            Console.WriteLine("Is Workbook Protected With Password: " + workbook.IsWorkbookProtectedWithPassword);

            // Ta bort skyddet från workbook
            workbook.Unprotect("password123");

            // Slutlig kontroll (bör vara falskt igen)
            Console.WriteLine("Is Workbook Protected With Password: " + workbook.IsWorkbookProtectedWithPassword);

            // Frigör arbetsboken
            workbook.Dispose();
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


