---
title: "Workbook.DefaultStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-egenskap. Hämtar eller anger standard‑Style‑objektet för arbetsboken"
type: docs
url: /sv/net/aspose.cells/workbook/defaultstyle/
---
## Workbook.DefaultStyle property

Hämtar eller anger standard‑[`Style`](../../style/)‑objektet för arbetsboken.

```csharp
public Style DefaultStyle { get; set; }
```

### Anmärkningar

DefaultStyle‑egenskapen är användbar för att implementera en Style för hela arbetsboken.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyDefaultStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Hämta standardstilen och ändra dess teckensnitt
            Style defaultStyle = workbook.DefaultStyle;
            defaultStyle.Font.Name = "Tahoma";
            defaultStyle.Font.Size = 12;
            
            // Tillämpa den modifierade stilen som standard
            workbook.DefaultStyle = defaultStyle;
            
            // Skapa ett arbetsblad och lägg till lite text med standardstilen
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("This text uses the default Tahoma font");
            
            // Spara arbetsboken
            workbook.Save("DefaultStyleDemo.xlsx");
        }
    }
}
```

### Se även

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


