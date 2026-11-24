---
title: "Klasse FontSourceBase"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.FontSourceBase Klasse. Dies ist eine abstrakte Basisklasse für Klassen, die dem Benutzer ermöglichen, verschiedene Schriftquellen anzugeben"
type: docs
url: /de/net/aspose.cells/fontsourcebase/
---
## FontSourceBase class

Dies ist eine abstrakte Basisklasse für die Klassen, die es dem Benutzer ermöglichen, verschiedene Schriftquellen anzugeben

```csharp
public abstract class FontSourceBase
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| abstract [Type](../../aspose.cells/fontsourcebase/type/) { get; } | Gibt den Typ der Schriftquellen zurück. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFontSourceBaseDemo
    {
        public static void Run()
        {
            // Erstelle eine Ordner‑Schriftquelle
            string fontFolder = @"C:\Windows\Fonts";
            FolderFontSource folderSource = new FolderFontSource(fontFolder, true);

            // Schriftquellen‑Eigenschaften anzeigen
            Console.WriteLine($"Font folder: {folderSource.FolderPath}");
            Console.WriteLine($"Scan subfolders: {folderSource.ScanSubFolders}");
            Console.WriteLine($"Source type: {folderSource.Type}");

            // Arbeitsmappe erstellen und Schriftquelle festlegen
            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderSource });

            // Mit benutzerdefinierten Schriften speichern
            workbook.Save("OutputWithCustomFonts.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


