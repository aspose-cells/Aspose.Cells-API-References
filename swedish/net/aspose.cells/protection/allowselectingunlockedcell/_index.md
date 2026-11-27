---
title: "Protection.AllowSelectingUnlockedCell"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Skyddsegenskap. Representerar om användaren får välja olåsta celler på ett skyddat arbetsblad"
type: docs
url: /sv/net/aspose.cells/protection/allowselectingunlockedcell/
---
## Protection.AllowSelectingUnlockedCell property

Representerar om användaren får markera olåsta celler på ett skyddat kalkylblad.

```csharp
public bool AllowSelectingUnlockedCell { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowSelectingUnlockedCellDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skydda arbetsbladet med alla skyddsalternativ
            Protection protection = worksheet.Protection;
            
            // Ställ in AllowSelectingUnlockedCell till true
            protection.AllowSelectingUnlockedCell = true;
            protection.AllowSelectingLockedCell = false;
            
            // Tillämpa skydd med lösenord
            protection.Password = "password123";
            worksheet.Protect(ProtectionType.All);

            // Verifiera inställningen
            Console.WriteLine("AllowSelectingUnlockedCell: " + protection.AllowSelectingUnlockedCell);
            Console.WriteLine("Worksheet is protected: " + worksheet.IsProtected);

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


