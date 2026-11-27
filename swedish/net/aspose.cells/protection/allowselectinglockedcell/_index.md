---
title: "Protection.AllowSelectingLockedCell"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Protection egenskap. Anger om användaren får välja låsta celler på ett skyddat kalkylblad"
type: docs
url: /sv/net/aspose.cells/protection/allowselectinglockedcell/
---
## Protection.AllowSelectingLockedCell property

Representerar om användaren får markera låsta celler på ett skyddat kalkylblad.

```csharp
public bool AllowSelectingLockedCell { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowSelectingLockedCellDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ställ in skyddsinställningar
            Protection protection = worksheet.Protection;
            
            // Demonstrera egenskapen AllowSelectingLockedCell
            protection.AllowSelectingLockedCell = true;
            Console.WriteLine("AllowSelectingLockedCell is set to: " + protection.AllowSelectingLockedCell);

            // Modifiera egenskapen och visa förändringen
            protection.AllowSelectingLockedCell = false;
            Console.WriteLine("AllowSelectingLockedCell is now set to: " + protection.AllowSelectingLockedCell);

            // Skydda kalkylbladet med lösenord
            protection.Password = "password123";
            worksheet.Protect(ProtectionType.All);

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


