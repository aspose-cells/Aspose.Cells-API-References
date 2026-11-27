---
title: "StyleFlag.TextDirection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "StyleFlag-egenskap. Inställning för textriktning kommer att tillämpas"
type: docs
url: /sv/net/aspose.cells/styleflag/textdirection/
---
## StyleFlag.TextDirection property

Inställning för textriktning kommer att tillämpas.

```csharp
public bool TextDirection { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyTextDirectionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Kom åt cell A1 och ange lite text
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text with TextDirection");

            // Skapa en stil och ange textriktning
            Style style = workbook.CreateStyle();
            style.TextDirection = TextDirectionType.Context;

            // Skapa en stilflagga och aktivera TextDirection-flaggan
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.TextDirection = true;

            // Applicera stilen på cellen med stilflaggan
            cell.SetStyle(style, styleFlag);

            // Visa aktuell textriktning
            Console.WriteLine("Current TextDirection value: " + cell.GetStyle().TextDirection);

            // Ändra textriktning och tillämpa igen
            style.TextDirection = TextDirectionType.LeftToRight;
            cell.SetStyle(style, styleFlag);

            Console.WriteLine("Current TextDirection value: " + cell.GetStyle().TextDirection);

            // Spara arbetsboken
            workbook.Save("TextDirectionDemo.xlsx");
        }
    }
}
```

### Se även

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


