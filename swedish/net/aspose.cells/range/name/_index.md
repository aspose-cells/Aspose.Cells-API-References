---
title: "Range.Name"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range-egenskapen. Hämtar eller anger namnet på intervallet"
type: docs
url: /sv/net/aspose.cells/range/name/
---
## Range.Name property

Hämtar eller anger namnet på området.

```csharp
public string Name { get; set; }
```

### Anmärkningar

Namngivet intervall stöds. Till exempel,

range.Name = "Sheet1!MyRange";

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa ett intervall (kolumnerna A till B)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 2, true);
            
            // Ställ in namn‑egenskapen för intervallet
            range.Name = "testRange";
            
            // Verifiera att namnet har satts
            Console.WriteLine("Range name: " + range.Name);
            
            // Spara arbetsboken
            workbook.Save("RangeWithName.xlsx");
            
            // Öppna den sparade filen för att demonstrera att namnet kvarstår
            Workbook loadedWorkbook = new Workbook("RangeWithName.xlsx");
            Aspose.Cells.Range loadedRange = loadedWorkbook.Worksheets[0].Cells.CreateRange(0, 2, true);
            Console.WriteLine("Loaded range name: " + loadedRange.Name);
        }
    }
}
```

### Se även

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


