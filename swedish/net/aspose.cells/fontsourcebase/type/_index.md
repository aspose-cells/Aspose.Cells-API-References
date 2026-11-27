---
title: "FontSourceBase.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FontSourceBase-egenskap. Returnerar typen av teckensnittskällan"
type: docs
url: /sv/net/aspose.cells/fontsourcebase/type/
---
## FontSourceBase.Type property

Returnerar typen av teckensnittskälla.

```csharp
public abstract FontSourceType Type { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontSourceBasePropertyTypeDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbokinstans
            Workbook workbook = new Workbook();
            
            // Skapa en teckensnittskälla i en mapp
            FolderFontSource folderFontSource = new FolderFontSource("C:\\MyFonts", true);
            
            // Visa Type-egenskapen för teckensnittskällan
            Console.WriteLine("Font source type: " + folderFontSource.Type);
            
            // Skapa en filteckensnittskälla
            FileFontSource fileFontSource = new FileFontSource("arial.ttf");
            
            // Visa Type-egenskapen för teckensnittskällan
            Console.WriteLine("Font source type: " + fileFontSource.Type);
            
            // Skapa minnes-teckensnittskälla (exempel med byte-array)
            byte[] fontData = System.IO.File.ReadAllBytes("arial.ttf");
            MemoryFontSource memoryFontSource = new MemoryFontSource(fontData);
            
            // Visa Type-egenskapen för teckensnittskällan
            Console.WriteLine("Font source type: " + memoryFontSource.Type);
            
            // Ange teckensnittskällor med den statiska metoden
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource, fileFontSource, memoryFontSource });
            
            // Spara arbetsboken
            workbook.Save("FontSourceTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [FontSourceType](../../fontsourcetype/)
* class [FontSourceBase](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


