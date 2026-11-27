---
title: "Class FolderFontSource"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.FolderFontSource-klass. Representerar mappen som innehåller TrueType-typsnittsfiler"
type: docs
url: /sv/net/aspose.cells/folderfontsource/
---
## FolderFontSource class

Representerar mappen som innehåller TrueType-teckensnittsfiler.

```csharp
public class FolderFontSource : FontSourceBase
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [FolderFontSource](folderfontsource/)(string, bool) | Konstruktor. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [FolderPath](../../aspose.cells/folderfontsource/folderpath/) { get; } | Sökväg till teckensnittsmappen. |
| [ScanSubFolders](../../aspose.cells/folderfontsource/scansubfolders/) { get; } | Bestämmer om underkataloger ska genomsökas eller inte. |
| override [Type](../../aspose.cells/folderfontsource/type/) { get; } | Returnerar typen av teckensnittskälla. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FolderFontSourceDemo
    {
        public static void FolderFontSourceExample()
        {
            // Skapa en instans av FolderFontSource
            string folderPath = @"C:\Fonts";
            bool scanSubfolders = true;
            FolderFontSource folderFontSource = new FolderFontSource(folderPath, scanSubfolders);

            // Åtkomst till egenskaper
            Console.WriteLine("Folder Path: " + folderFontSource.FolderPath);
            Console.WriteLine("Scan Subfolders: " + folderFontSource.ScanSubFolders);
            Console.WriteLine("Font Source Type: " + folderFontSource.Type);

            // Skapa en arbetsbok och ange teckensnittskällorna
            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource });

            // Spara arbetsboken
            workbook.Save("FolderFontSourceExample.xlsx");
            workbook.Save("FolderFontSourceExample.pdf");
            return;
        }
    }
}
```

### Se även

* class [FontSourceBase](../fontsourcebase/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


