---
title: "Protection.AllowDeletingColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Protection-egenskapen. Anger om borttagning av kolumner är tillåten på ett skyddat kalkylblad"
type: docs
url: /sv/net/aspose.cells/protection/allowdeletingcolumn/
---
## Protection.AllowDeletingColumn property

Representerar om radering av kolumner är tillåten på ett skyddat kalkylblad.

```csharp
public bool AllowDeletingColumn { get; set; }
```

### Anmärkningar

Kolumnerna som innehåller cellerna som ska tas bort måste vara olåsta när bladet är skyddat, och alternativet "Välj olåsta celler" måste vara aktiverat.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowDeletingColumnDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aktivera skydd av kalkylblad
            Protection protection = worksheet.Protection;
            protection.AllowDeletingColumn = true;
            worksheet.Protect(ProtectionType.All);

            // Verifiera inställningen
            Console.WriteLine("AllowDeletingColumn: " + protection.AllowDeletingColumn);

            // Försök att ta bort en kolumn (bör fungera eftersom AllowDeletingColumn är true)
            worksheet.Cells.DeleteColumn(0);
            Console.WriteLine("Column deleted successfully");

            // Inaktivera kolumnradering
            protection.AllowDeletingColumn = false;

            // Försök att ta bort en annan kolumn (ska misslyckas)
            try
            {
                worksheet.Cells.DeleteColumn(1);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Failed to delete column: " + ex.Message);
            }
        }
    }
}
```

### Se även

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


