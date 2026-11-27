---
title: "Protection.AllowFormattingRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Protection-egenskapen. Anger om formatering av rader är tillåten på ett skyddat kalkylblad"
type: docs
url: /sv/net/aspose.cells/protection/allowformattingrow/
---
## Protection.AllowFormattingRow property

Representerar om formatering av rader är tillåten på ett skyddat kalkylblad

```csharp
public bool AllowFormattingRow { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowFormattingRowDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aktivera skydd av kalkylblad
            worksheet.Protect(ProtectionType.All);

            // Åtkomst till skyddsinställningar
            Protection protection = worksheet.Protection;

            // Tillåt formatering av rader samtidigt som andra skydd behålls
            protection.AllowFormattingRow = true;

            // Spara arbetsboken
            workbook.Save("Protection_AllowFormattingRow.xlsx");
        }
    }
}
```

### Se även

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


