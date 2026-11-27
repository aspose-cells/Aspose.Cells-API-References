---
title: "Row.IsHeightMatched"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Row-egenskap. Anger om radens höjd matchar den aktuella standardteckensnittinställningen i arbetsboken. Sant för denna egenskap betyder också att radens höjd är automatisk utan att ett anpassat höjdvärde har satts av användaren."
type: docs
url: /sv/net/aspose.cells/row/isheightmatched/
---
## Row.IsHeightMatched property

Anger om radens höjd matchar den aktuella standardteckensnittinställningen i arbetsboken. Sant för den här egenskapen betyder också att radens höjd är "automatisk" utan att ett anpassat höjdvärde har satts av användaren.

```csharp
public bool IsHeightMatched { get; set; }
```

### Anmärkningar

När denna egenskap är sann, om innehållet i raden ändras, måste radens höjd vanligtvis omberäknas (t.ex. med [`AutoFitRows`](../../worksheet/autofitrows/)) för att få samma resultat som visas i MS Excel när du öppnar arbetsboken i den.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyIsHeightMatchedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in exempeldata och formatera för att demonstrera radhöjdsanpassning
            worksheet.Cells["A1"].PutValue("This is a test string to demonstrate row height matching");
            worksheet.Cells["B1"].PutValue("Another cell in the same row");
            
            // Tillämpa radbrytning för att tvinga höjdjustering
            Style style = worksheet.Cells["A1"].GetStyle();
            style.IsTextWrapped = true;
            worksheet.Cells["A1"].SetStyle(style);
            
            // Autoanpassa raden för att matcha innehållshöjden
            worksheet.AutoFitRow(0);
            
            // Kontrollera om radens höjd matchar dess innehåll
            Console.WriteLine("Is row height matched: " + worksheet.Cells.Rows[0].IsHeightMatched);
        }
    }
}
```

### Se även

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


