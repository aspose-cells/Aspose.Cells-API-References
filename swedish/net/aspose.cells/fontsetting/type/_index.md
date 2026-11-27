---
title: "FontSetting.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FontSetting-egenskap. Hämtar typen av textnod"
type: docs
url: /sv/net/aspose.cells/fontsetting/type/
---
## FontSetting.Type property

Hämtar typen av textnod.

```csharp
public virtual TextNodeType Type { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;  // Added this using directive
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingPropertyTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till text i en cell
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // Hämta teckensnittinställningar för cellens tecken
            FontSetting fontSetting = new FontSetting(0, 6, workbook.Worksheets);

            // Visa det aktuella Type‑värdet
            Console.WriteLine("Current Type value: " + fontSetting.Type);

            // Demonstrera hur Typ påverkar textbehandling
            if (fontSetting.Type == TextNodeType.TextRun)
            {
                Console.WriteLine("The text is a standard text run.");
            }
            else if (fontSetting.Type == TextNodeType.TextParagraph)
            {
                Console.WriteLine("The text is part of a paragraph.");
            }
            else if (fontSetting.Type == TextNodeType.Equation)
            {
                Console.WriteLine("The text represents an equation.");
            }

            // Applicera olika formatering baserat på Typ
            if (fontSetting.Type == TextNodeType.TextRun)
            {
                fontSetting.Font.Color = System.Drawing.Color.Red;
                fontSetting.SetWordArtStyle(PresetWordArtStyle.WordArtStyle1);
            }

            // Spara resultatet
            workbook.Save("FontSettingTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [TextNodeType](../../../aspose.cells.drawing.texts/textnodetype/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


