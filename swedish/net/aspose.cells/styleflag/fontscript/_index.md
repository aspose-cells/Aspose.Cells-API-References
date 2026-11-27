---
title: "StyleFlag.FontScript"
second_title: "Aspose.Cells för .NET API‑referens"
description: "StyleFlag-egenskap. Inställning för teckensnittsskript kommer att tillämpas"
type: docs
url: /sv/net/aspose.cells/styleflag/fontscript/
---
## StyleFlag.FontScript property

Inställning för teckensnittsskript kommer att tillämpas.

```csharp
public bool FontScript { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyFontScriptDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Kom åt cell A1 och ange lite text
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // Skapa ett stilobjekt och sätt teckensnittsskript till nedsänkt
            Style style = workbook.CreateStyle();
            style.Font.IsSubscript = true;

            // Skapa en stilflagga och aktivera FontScript-flaggan
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.FontScript = true;

            // Applicera stilen på cellen med stilflaggan
            cell.SetStyle(style, styleFlag);

            // Visa aktuell teckensnittsskriptstatus
            Console.WriteLine("Font is subscript: " + cell.GetStyle().Font.IsSubscript);

            // Ändra teckensnittsskript till upphöjt
            style.Font.IsSubscript = false;
            style.Font.IsSuperscript = false;
            cell.SetStyle(style, styleFlag);

            // Visa den uppdaterade statusen för teckensnittsskriptet
            Console.WriteLine("Font is superscript: " + cell.GetStyle().Font.IsSuperscript);
            Console.WriteLine("Font is subscript: " + cell.GetStyle().Font.IsSubscript);

            // Spara arbetsboken
            workbook.Save("StyleFlagPropertyFontScriptDemo.xlsx");
        }
    }
}
```

### Se även

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


