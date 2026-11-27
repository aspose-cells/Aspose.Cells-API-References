---
title: "Style.VerticalAlignment"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style‑egenskap. Hämtar eller anger den vertikala justeringstypen för texten i en cell"
type: docs
url: /sv/net/aspose.cells/style/verticalalignment/
---
## Style.VerticalAlignment property

Hämtar eller anger den vertikala justeringstypen för texten i en cell.

```csharp
public TextAlignmentType VerticalAlignment { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyVerticalAlignmentDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Åtkomst till cell A1
            Cell cell = worksheet.Cells["A1"];
            
            // Ange cellvärdet
            cell.PutValue("Vertical Alignment Demo");
            
            // Åtkomst till cellens stil
            Style style = cell.GetStyle();
            
            // Ställ in vertikal justering till Top
            style.VerticalAlignment = TextAlignmentType.Top;
            cell.SetStyle(style);
            
            // Spara arbetsboken
            workbook.Save("VerticalAlignmentDemo.xlsx");
            
            Console.WriteLine("Vertical alignment set to Top for cell A1.");
        }
    }
}
```

### Se även

* enum [TextAlignmentType](../../textalignmenttype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


