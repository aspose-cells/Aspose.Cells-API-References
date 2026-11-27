---
title: "Border.ArgbColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Border‑egenskap. Hämtar och anger färgen med ett 32‑bitars ARGB‑värde"
type: docs
url: /sv/net/aspose.cells/border/argbcolor/
---
## Border.ArgbColor property

Hämtar och anger färgen med ett 32-bitars ARGB‑värde.

```csharp
public int ArgbColor { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BorderPropertyArgbColorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Få åtkomst till cell B2 och ange ett värde
            Cell cell = worksheet.Cells["B2"];
            cell.PutValue("Border ARGB Color Demo");

            // Hämta stilen och kanterna
            Style style = cell.GetStyle();
            Border border = style.Borders[BorderType.TopBorder];

            // Ställ in kantegenskaper inklusive ARGB‑färg
            border.LineStyle = CellBorderType.Thick;
            unchecked
            {
                border.ArgbColor = (int)0xFFFF0000; // Red color in ARGB format with unchecked cast
            }

            // Applicera den modifierade stilen på cellen
            cell.SetStyle(style);

            // Spara arbetsboken
            workbook.Save("BorderArgbColorDemo.xlsx");

            // Verifiera att ARGB‑färgen har ställts in korrekt
            Border savedBorder = workbook.Worksheets[0].Cells["B2"].GetStyle().Borders[BorderType.TopBorder];
            Console.WriteLine("ARGB Color of top border: " + savedBorder.ArgbColor.ToString("X8"));
        }
    }
}
```

### Se även

* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


