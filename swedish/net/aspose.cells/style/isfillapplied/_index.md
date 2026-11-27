---
title: "Style.IsFillApplied"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style‑egenskap. Ange om fyllningsformateringen ska tillämpas"
type: docs
url: /sv/net/aspose.cells/style/isfillapplied/
---
## Style.IsFillApplied property

Anger om fyllnadsformateringen ska tillämpas.

```csharp
public bool IsFillApplied { get; set; }
```

### Anmärkningar

Endast för namngiven stil.

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyIsFillAppliedDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa en stil
            Style style = workbook.CreateStyle();
            
            // Initialt ska IsFillApplied vara falskt
            Console.WriteLine("IsFillApplied (initial): " + style.IsFillApplied);
            
            // Tillämpa fyllningsinställningar
            style.ForegroundColor = Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            
            // Efter att fyllningsegenskaperna har satts ska IsFillApplied vara sant
            Console.WriteLine("IsFillApplied (after setting fill): " + style.IsFillApplied);
            
            // Tillämpa stilen på en cell
            worksheet.Cells["A1"].SetStyle(style);
            
            // Spara arbetsboken
            workbook.Save("IsFillAppliedDemo.xlsx");
        }
    }
}
```

### Se även

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


