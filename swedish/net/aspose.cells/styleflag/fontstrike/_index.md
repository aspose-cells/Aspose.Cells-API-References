---
title: "StyleFlag.FontStrike"
second_title: "Aspose.Cells för .NET API‑referens"
description: "StyleFlag-egenskap. Inställning för genomstruken text kommer att tillämpas"
type: docs
url: /sv/net/aspose.cells/styleflag/fontstrike/
---
## StyleFlag.FontStrike property

Inställning för genomstrykning i teckensnittet kommer att tillämpas.

```csharp
public bool FontStrike { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyFontStrikeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Kom åt cell A1 och ange lite text
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // Skapa ett stilobjekt och sätt FontStrike till true
            Style style = workbook.CreateStyle();
            style.Font.IsStrikeout = true;

            // Skapa en stilflagga och aktivera FontStrike-flaggan
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.FontStrike = true;

            // Applicera stilen på cellen med stilflaggan
            cell.SetStyle(style, styleFlag);

            // Visa aktuell FontStrike-status
            Console.WriteLine("FontStrike applied: " + cell.GetStyle().Font.IsStrikeout);

            // Skapa en annan cell för att demonstrera text utan genomstrykning
            Cell cell2 = worksheet.Cells["A2"];
            cell2.PutValue("Normal Text");
            styleFlag.FontStrike = false;

            cell2.SetStyle(style, styleFlag);
            Console.WriteLine("FontStrike applied: " + cell2.GetStyle().Font.IsStrikeout);

            // Spara arbetsboken för att se effekterna
            workbook.Save("PropertyFontStrikeDemo.xlsx");
        }
    }
}
```

### Se även

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


