---
title: "Protection.AllowInsertingRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Protection-egenskapen. Anger om infogning av rader är tillåten på ett skyddat kalkylblad"
type: docs
url: /sv/net/aspose.cells/protection/allowinsertingrow/
---
## Protection.AllowInsertingRow property

Representerar om infogning av rader är tillåten på ett skyddat kalkylblad

```csharp
public bool AllowInsertingRow { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowInsertingRowDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Åtkomst till skyddsinställningarna
            Protection protection = worksheet.Protection;

            // Aktivera infogning av rader när skyddat
            protection.AllowInsertingRow = true;
            protection.Password = "password123";
            worksheet.Protect(ProtectionType.All);

            // Försök att infoga en rad (bör fungera eftersom AllowInsertingRow är true)
            worksheet.Cells.InsertRow(0);

            // Spara arbetsboken
            workbook.Save("AllowInsertingRowDemo.xlsx");
        }
    }
}
```

### Se även

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


