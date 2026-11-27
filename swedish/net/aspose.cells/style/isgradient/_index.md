---
title: "Style.IsGradient"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style property. Anger om cellens skuggning är ett gradientmönster"
type: docs
url: /sv/net/aspose.cells/style/isgradient/
---
## Style.IsGradient property

Anger om cellskuggning är ett gradientmönster.

```csharp
public bool IsGradient { get; set; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyIsGradientDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en stil
            Style style = workbook.CreateStyle();
            
            // Ange gradientbakgrund
            style.SetTwoColorGradient(Color.LightBlue, Color.DarkBlue, GradientStyleType.Horizontal, 1);
            
            // Tillämpa stilen på en cell
            worksheet.Cells["A1"].SetStyle(style);
            
            // Kontrollera om stilen har gradient
            bool isGradient = worksheet.Cells["A1"].GetStyle().IsGradient;
            
            // Skriv ut resultatet
            Console.WriteLine("Cell A1 style has gradient: " + isGradient);
            
            // Spara arbetsboken
            workbook.Save("GradientStyleDemo.xlsx");
        }
    }
}
```

### Se även

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


