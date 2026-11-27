---
title: "Protection.AllowFormattingCell"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Skyddsegenskap. Representerar om formatering av celler är tillåten på ett skyddat arbetsblad"
type: docs
url: /sv/net/aspose.cells/protection/allowformattingcell/
---
## Protection.AllowFormattingCell property

Representerar om formatering av celler är tillåten på ett skyddat kalkylblad.

```csharp
public bool AllowFormattingCell { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowFormattingCellDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aktivera skydd av kalkylblad
            Protection protection = worksheet.Protection;
            
            // Ställ in olika skyddsegenskaper med en flagga
            int flag = 0x40; // Only AllowFormattingCell flag is set
            protection.AllowFormattingCell = (flag & 0x40) != 0;

            // Verifiera inställningen
            Console.WriteLine("AllowFormattingCell is set to: " + protection.AllowFormattingCell);

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


