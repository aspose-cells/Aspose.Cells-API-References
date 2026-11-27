---
title: "Style.Pattern"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style-egenskap. Hämtar eller anger cellens bakgrundsmönstertyp"
type: docs
url: /sv/net/aspose.cells/style/pattern/
---
## Style.Pattern property

Hämtar eller anger cellens bakgrundsmönstertyp.

```csharp
public BackgroundType Pattern { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyPatternDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Få åtkomst till cellen och hämta dess stil
            Cell cell = cells[0, 0];
            Style style = cell.GetStyle();
            
            // Ställ in mönster och förgrundsfärg
            style.Pattern = BackgroundType.Gray50;
            style.ForegroundColor = System.Drawing.Color.LightGray;
            
            // Tillämpa stilen på cellen
            cell.SetStyle(style);
            
            // Spara arbetsboken
            workbook.Save("PatternPropertyDemo.xlsx");
        }
    }
}
```

### Se även

* enum [BackgroundType](../../backgroundtype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


