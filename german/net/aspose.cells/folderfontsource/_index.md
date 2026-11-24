---
title: "Class FolderFontSource"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.FolderFontSource-Klasse. Stellt den Ordner dar, der TrueType-Schriftdateien enthält"
type: docs
url: /de/net/aspose.cells/folderfontsource/
---
## FolderFontSource class

Stellt den Ordner dar, der TrueType-Schriftdateien enthält.

```csharp
public class FolderFontSource : FontSourceBase
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [FolderFontSource](folderfontsource/)(string, bool) | Ctor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [FolderPath](../../aspose.cells/folderfontsource/folderpath/) { get; } | Pfad zum Schriftartenordner. |
| [ScanSubFolders](../../aspose.cells/folderfontsource/scansubfolders/) { get; } | Bestimmt, ob Unterordner durchsucht werden sollen oder nicht. |
| override [Type](../../aspose.cells/folderfontsource/type/) { get; } | Gibt den Typ der Schriftquellen zurück. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FolderFontSourceDemo
    {
        public static void FolderFontSourceExample()
        {
            // Erstelle eine Instanz von FolderFontSource
            string folderPath = @"C:\Fonts";
            bool scanSubfolders = true;
            FolderFontSource folderFontSource = new FolderFontSource(folderPath, scanSubfolders);

            // Zugriff auf Eigenschaften
            Console.WriteLine("Folder Path: " + folderFontSource.FolderPath);
            Console.WriteLine("Scan Subfolders: " + folderFontSource.ScanSubFolders);
            Console.WriteLine("Font Source Type: " + folderFontSource.Type);

            // Erstelle eine Arbeitsmappe und setze die Schriftquellen
            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource });

            // Speichere die Arbeitsmappe
            workbook.Save("FolderFontSourceExample.xlsx");
            workbook.Save("FolderFontSourceExample.pdf");
            return;
        }
    }
}
```

### Siehe auch

* class [FontSourceBase](../fontsourcebase/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


