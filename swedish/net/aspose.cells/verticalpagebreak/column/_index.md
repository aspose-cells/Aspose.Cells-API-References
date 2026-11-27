---
title: "VerticalPageBreak.Column"
second_title: "Aspose.Cells för .NET API‑referens"
description: "VerticalPageBreak-egenskapen. Hämtar kolumnindexet för den vertikala sidbrytningen"
type: docs
url: /sv/net/aspose.cells/verticalpagebreak/column/
---
## VerticalPageBreak.Column property

Hämtar kolumnindexet för den vertikala sidbrytningen.

```csharp
public int Column { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakPropertyColumnDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till vertikala sidbrytningar i kolumnerna 4 och 8
            worksheet.VerticalPageBreaks.Add(4);
            worksheet.VerticalPageBreaks.Add(8);

            // Hämta samlingen av vertikala sidbrytningar
            VerticalPageBreakCollection vpagebreaks = worksheet.VerticalPageBreaks;

            // Visa information om varje vertikal sidbrytning
            Console.WriteLine("Vertical Page Breaks Count: " + vpagebreaks.Count);
            
            foreach (VerticalPageBreak vpagebreak in vpagebreaks)
            {
                Console.WriteLine("\nPage Break at Column: " + vpagebreak.Column);
                Console.WriteLine("Start Row: " + vpagebreak.StartRow);
                Console.WriteLine("End Row: " + vpagebreak.EndRow);
            }

            // Spara arbetsboken
            workbook.Save("VerticalPageBreakDemo.xlsx");
        }
    }
}
```

### Se även

* class [VerticalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


