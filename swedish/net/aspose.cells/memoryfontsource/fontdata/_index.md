---
title: "MemoryFontSource.FontData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MemoryFontSource-egenskap. Binär typsnittsdata"
type: docs
url: /sv/net/aspose.cells/memoryfontsource/fontdata/
---
## MemoryFontSource.FontData property

Binär typsnittsdata.

```csharp
public byte[] FontData { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class MemoryFontSourcePropertyFontDataDemo
    {
        public static void Run()
        {
            // Läs in en TrueType-typsnittfil i minnet
            byte[] fontBytes = File.ReadAllBytes("arial.ttf");

            // Skapa en MemoryFontSource-instans med typsnittsdata
            MemoryFontSource memoryFontSource = new MemoryFontSource(fontBytes);

            // Visa det aktuella FontData-värdet (första 10 byte för demonstration)
            Console.WriteLine("FontData length: " + memoryFontSource.FontData.Length);
            Console.Write("First 10 bytes: ");
            for (int i = 0; i < 10 && i < memoryFontSource.FontData.Length; i++)
            {
                Console.Write(memoryFontSource.FontData[i].ToString("X2") + " ");
            }
            Console.WriteLine();

            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa typsnittsinställningar och lägg till vår MemoryFontSource
            FontConfigs.SetFontSources(new FontSourceBase[] { memoryFontSource });

            // Applicera typsnittskonfigurationerna globalt (inte arbetsboksspecifikt)
            FontConfigs.DefaultFontName = "Arial";
            FontConfigs.SetFontSources(new FontSourceBase[] { memoryFontSource });

            // Skapa en stil med det anpassade typsnittet
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;

            // Tillämpa stilen på en cell
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["A1"].PutValue("Text using memory font source");

            // Spara arbetsboken
            workbook.Save("MemoryFontSourceDemo.xlsx");
        }
    }
}
```

### Se även

* class [MemoryFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


