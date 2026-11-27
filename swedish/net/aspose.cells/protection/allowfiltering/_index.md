---
title: "Protection.AllowFiltering"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Protection-egenskapen. Anger om användaren får använda ett AutoFilter som skapades innan bladet skyddades"
type: docs
url: /sv/net/aspose.cells/protection/allowfiltering/
---
## Protection.AllowFiltering property

Representerar om användaren får använda ett AutoFilter som skapades innan bladet skyddades.

```csharp
public bool AllowFiltering { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowFilteringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aktivera skydd av kalkylblad
            worksheet.Protect(ProtectionType.All);
            
            // Ställ in AllowFiltering‑egenskapen till true
            worksheet.Protection.AllowFiltering = true;
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
            
            // Verifiera att egenskapen sparades korrekt
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("AllowFiltering: " + 
                loadedWorkbook.Worksheets[0].Protection.AllowFiltering);
        }
    }
}
```

### Se även

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


