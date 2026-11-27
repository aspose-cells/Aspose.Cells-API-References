---
title: "MemoryFontSource.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MemoryFontSource-egenskap. Returnerar typen av typsnittskällan"
type: docs
url: /sv/net/aspose.cells/memoryfontsource/type/
---
## MemoryFontSource.Type property

Returnerar typen av teckensnittskälla.

```csharp
public override FontSourceType Type { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class MemoryFontSourcePropertyTypeDemo
    {
        public static void Run()
        {
            // Läs in en TrueType-typsnittfil i minnet
            byte[] fontData = File.ReadAllBytes("arial.ttf");

            // Skapa en MemoryFontSource-instans med typsnittsdata
            MemoryFontSource memoryFontSource = new MemoryFontSource(fontData);

            // Visa det aktuella Type‑värdet
            Console.WriteLine("MemoryFontSource Type: " + memoryFontSource.Type);

            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ställ in typsnittskällor med FontConfigs
            FontConfigs.SetFontSources(new FontSourceBase[] { memoryFontSource });

            // Verifiera att typsnittskällans typ är MemoryFont
            if (memoryFontSource.Type == FontSourceType.MemoryFont)
            {
                // Använd typsnittet i en cell
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 14;
                worksheet.Cells["A1"].SetStyle(style);
                worksheet.Cells["A1"].PutValue("Text using memory font source");

                // Lägg till information om typsnittskällans typ
                worksheet.Cells["A2"].PutValue("Font source type: " + memoryFontSource.Type);
            }

            // Spara arbetsboken
            workbook.Save("MemoryFontSourceTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [FontSourceType](../../fontsourcetype/)
* class [MemoryFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


