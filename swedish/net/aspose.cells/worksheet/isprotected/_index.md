---
title: "Worksheet.IsProtected"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Anger om arbetsbladet är skyddat"
type: docs
url: /sv/net/aspose.cells/worksheet/isprotected/
---
## Worksheet.IsProtected property

Anger om kalkylbladet är skyddat.

```csharp
public bool IsProtected { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsProtectedDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Skydda arbetsboken och första arbetsbladet
            workbook.Protect(ProtectionType.All, "password");
            workbook.Worksheets[0].Protect(ProtectionType.All, "password", null);

            // Kontrollera om arbetsbladet är skyddat
            bool isProtected = workbook.Worksheets[0].IsProtected;
            Console.WriteLine($"Worksheet is protected: {isProtected}");

            // Spara arbetsboken
            workbook.Save("protected_worksheet.xlsx");

            // Läs in den sparade arbetsboken och verifiera skyddet
            Workbook loadedWorkbook = new Workbook("protected_worksheet.xlsx");
            Console.WriteLine($"Loaded worksheet is protected: {loadedWorkbook.Worksheets[0].IsProtected}");
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


