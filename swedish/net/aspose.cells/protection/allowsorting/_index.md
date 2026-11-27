---
title: "Protection.AllowSorting"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Protection egenskap. Anger om sorteringsalternativet är tillåtet på ett skyddat kalkylblad"
type: docs
url: /sv/net/aspose.cells/protection/allowsorting/
---
## Protection.AllowSorting property

Representerar om sorteringsalternativet är tillåtet på ett skyddat kalkylblad.

```csharp
public bool AllowSorting { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowSortingDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aktivera skydd av kalkylblad
            worksheet.Protect(ProtectionType.All);
            
            // Ställ in skyddsegenskaper inklusive AllowSorting
            Protection protection = worksheet.Protection;
            protection.AllowSorting = true;
            protection.AllowFiltering = true;
            protection.AllowEditingContent = false;

            // Visa skyddsinställningar
            Console.WriteLine("Protection Settings:");
            Console.WriteLine($"AllowSorting: {protection.AllowSorting}");
            Console.WriteLine($"AllowFiltering: {protection.AllowFiltering}");
            Console.WriteLine($"AllowEditingContent: {protection.AllowEditingContent}");

            // Demonstrera sorteringsfunktion
            if (protection.AllowSorting)
            {
                Console.WriteLine("\nSorting is allowed on this protected worksheet");
            }
            else
            {
                Console.WriteLine("\nSorting is not allowed on this protected worksheet");
            }
        }
    }
}
```

### Se även

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


