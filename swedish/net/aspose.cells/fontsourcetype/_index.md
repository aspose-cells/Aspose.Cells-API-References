---
title: "Enum FontSourceType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.FontSourceType enum. Anger typen av en teckensnittskälla"
type: docs
url: /sv/net/aspose.cells/fontsourcetype/
---
## FontSourceType enumeration

Anger typen av en typsnittskälla.

```csharp
public enum FontSourceType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| FontFile | `0` | representerar en enskild teckensnittfil. |
| FontsFolder | `1` | Representerar en mapp med teckensnittsfiler. |
| MemoryFont | `2` | Representerar ett enskilt teckensnitt i minnet. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassFontSourceTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Demonstrera FontSourceType enum-värden
            Console.WriteLine("FontSourceType values:");
            Console.WriteLine($"FontFile: {FontSourceType.FontFile}");
            Console.WriteLine($"FontsFolder: {FontSourceType.FontsFolder}");
            Console.WriteLine($"MemoryFont: {FontSourceType.MemoryFont}");

            // Skapa teckensnittinställningar och använd FontSourceType
            FontConfigs.SetFontFolder(@"C:\MyFonts\", false);
            FontConfigs.SetFontSources(new FontSourceBase[]
            {
                new FolderFontSource(@"C:\MyFonts\", false),
                new FileFontSource(@"C:\MyFonts\arial.ttf"),
                new MemoryFontSource(new byte[0])
            });

            // Applicera teckensnitt på en cell
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["A1"].PutValue("Text with Arial font");

            // Spara resultatet
            workbook.Save("FontSourceTypeDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


