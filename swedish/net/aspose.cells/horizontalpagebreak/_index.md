---
title: "Klass HorizontalPageBreak"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.HorizontalPageBreak klass. Inkapslar objektet som representerar ett horisontellt sidbrytning"
type: docs
url: /sv/net/aspose.cells/horizontalpagebreak/
---
## HorizontalPageBreak class

Inkapslar objektet som representerar ett horisontellt sidbryt.

```csharp
public class HorizontalPageBreak
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [EndColumn](../../aspose.cells/horizontalpagebreak/endcolumn/) { get; } | Hämtar slutkolumnindex för detta horisontella sidbrytning. |
| [Row](../../aspose.cells/horizontalpagebreak/row/) { get; } | Hämtar radindex med nollbas. |
| [StartColumn](../../aspose.cells/horizontalpagebreak/startcolumn/) { get; } | Hämtar startkolumnindex för detta horisontella sidbrytning. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HorizontalPageBreakDemo
    {
        public static void HorizontalPageBreakExample()
        {
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();
            
            // Hämtar referensen till det nyligen tillagda kalkylbladet genom att ange dess bladindex
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en sidbrytning vid cell Y30
            int index = worksheet.HorizontalPageBreaks.Add("Y30");
            
            // Hämta den nyligen tillagda horisontella sidbrytningen
            HorizontalPageBreak hPageBreak = worksheet.HorizontalPageBreaks[index];
            
            // Visa egenskaperna för den horisontella sidbrytningen
            Console.WriteLine("Horizontal Page Break Details:");
            Console.WriteLine($"Row: {hPageBreak.Row}");
            Console.WriteLine($"Start Column: {hPageBreak.StartColumn}");
            Console.WriteLine($"End Column: {hPageBreak.EndColumn}");
            
            // Spara arbetsboken
            workbook.Save("HorizontalPageBreakExample.xlsx");
            workbook.Save("HorizontalPageBreakExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


