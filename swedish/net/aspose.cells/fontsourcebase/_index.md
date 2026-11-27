---
title: "Klass FontSourceBase"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.FontSourceBase klass. Detta är en abstrakt basklass för de klasser som låter användaren ange olika teckensnittskällor"
type: docs
url: /sv/net/aspose.cells/fontsourcebase/
---
## FontSourceBase class

Detta är en abstrakt basklass för klasserna som låter användaren specificera olika teckensnittskällor

```csharp
public abstract class FontSourceBase
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| abstract [Type](../../aspose.cells/fontsourcebase/type/) { get; } | Returnerar typen av teckensnittskälla. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFontSourceBaseDemo
    {
        public static void Run()
        {
            // Skapa en teckensnittskälla i en mapp
            string fontFolder = @"C:\Windows\Fonts";
            FolderFontSource folderSource = new FolderFontSource(fontFolder, true);

            // Visa egenskaper för teckensnittskälla
            Console.WriteLine($"Font folder: {folderSource.FolderPath}");
            Console.WriteLine($"Scan subfolders: {folderSource.ScanSubFolders}");
            Console.WriteLine($"Source type: {folderSource.Type}");

            // Skapa arbetsbok och ange teckensnittskälla
            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderSource });

            // Spara med anpassade teckensnitt
            workbook.Save("OutputWithCustomFonts.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


