---
title: "VerticalPageBreak.EndRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "VerticalPageBreak-egenskapen. Hämtar slutradindexet för den vertikala sidbrytningen"
type: docs
url: /sv/net/aspose.cells/verticalpagebreak/endrow/
---
## VerticalPageBreak.EndRow property

Hämtar slutradens index för den vertikala sidbrytningen.

```csharp
public int EndRow { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakPropertyEndRowDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en vertikal sidbrytning som sträcker sig över raderna 3 till 8 i kolumn C (index 2)
            worksheet.VerticalPageBreaks.Add("C3:C8");

            // Hämta den första vertikala sidbrytningen
            VerticalPageBreak vpb = worksheet.VerticalPageBreaks[0];
            
            // Visa slutraden för sidbrytningen
            Console.WriteLine("Vertical Page Break End Row: " + vpb.EndRow);
            
            // Eftersom EndRow är skrivskyddad kommer vi att demonstrera hur man hämtar den men inte sätter den
            // Följande rad tas bort eftersom den orsakar kompileringsfel:
            // vpb.EndRow = 10;
            
            // Istället kommer vi att lägga till en annan sidbrytning med en annan slutrad
            worksheet.VerticalPageBreaks.Add("C3:C10");
            VerticalPageBreak vpb2 = worksheet.VerticalPageBreaks[1];
            Console.WriteLine("Second Page Break End Row: " + vpb2.EndRow);
        }
    }
}
```

### Se även

* class [VerticalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


