---
title: "Protection.AllowInsertingColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Protection-egenskapen. Anger om infogning av kolumner är tillåten på ett skyddat kalkylblad"
type: docs
url: /sv/net/aspose.cells/protection/allowinsertingcolumn/
---
## Protection.AllowInsertingColumn property

Representerar om infogning av kolumner är tillåten på ett skyddat kalkylblad

```csharp
public bool AllowInsertingColumn { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowInsertingColumnDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hämta skyddsinställningarna
            Protection protection = worksheet.Protection;

            // Ställ in AllowInsertingColumn till true
            protection.AllowInsertingColumn = true;

            // Verifiera inställningen
            Console.WriteLine("AllowInsertingColumn is set to: " + protection.AllowInsertingColumn);

            // Skydda kalkylbladet med lösenord (använder Workbook.Protect‑metoden)
            workbook.Protect(ProtectionType.All, "password123");
            protection.AllowInsertingColumn = true; // Explicitly set again to demonstrate

            // Spara arbetsboken
            workbook.Save("ProtectionDemo.xlsx");
        }
    }
}
```

### Se även

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


