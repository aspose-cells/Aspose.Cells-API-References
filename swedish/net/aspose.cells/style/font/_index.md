---
title: "Style.Font"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style-egenskap. Hämtar ett Font-objekt"
type: docs
url: /sv/net/aspose.cells/style/font/
---
## Style.Font property

Hämtar ett `Font`-objekt.

```csharp
public Font Font { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyFontDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Åtkomst till cell B4 och sätt dess teckensnitt till fet
            Cell b4 = cells["B4"];
            Style b4Style = b4.GetStyle();
            b4Style.Font.IsBold = true;
            b4.SetStyle(b4Style);

            // Åtkomst till cell C4 och säkerställ att dess teckensnitt inte är fet
            Cell c4 = cells["C4"];
            Style c4Style = c4.GetStyle();
            c4Style.Font.IsBold = false;
            c4.SetStyle(c4Style);

            // Åtkomst till cell D4 och sätt dess teckensnitt till fet med en annan färg
            Cell d4 = cells["D4"];
            Style d4Style = d4.GetStyle();
            d4Style.Font.IsBold = true;
            d4Style.Font.Color = Color.Red;
            d4.SetStyle(d4Style);

            // Verifiera teckensnittets egenskaper
            Console.WriteLine("B4 Font Bold: " + b4.GetStyle().Font.IsBold);
            Console.WriteLine("C4 Font Bold: " + c4.GetStyle().Font.IsBold);
            Console.WriteLine("D4 Font Bold: " + d4.GetStyle().Font.IsBold);
            Console.WriteLine("D4 Font Color: " + d4.GetStyle().Font.Color);

            // Spara arbetsboken
            workbook.Save("FontPropertyDemo.xlsx");
        }
    }
}
```

### Se även

* class [Font](../../font/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


