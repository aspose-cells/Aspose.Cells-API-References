---
title: "FolderFontSource.FolderPath"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FolderFontSource-Eigenschaft. Pfad zum Schriftartenordner"
type: docs
url: /de/net/aspose.cells/folderfontsource/folderpath/
---
## FolderFontSource.FolderPath property

Pfad zum Schriftartenordner.

```csharp
public string FolderPath { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FolderFontSourcePropertyFolderPathDemo
    {
        public static void Run()
        {
            // Erstelle eine Ordner‑Schriftquelle
            string folderPath = @"C:\Windows\Fonts"; // Typical system fonts folder
            bool scanSubfolders = true;
            FolderFontSource folderFontSource = new FolderFontSource(folderPath, scanSubfolders);

            // Demonstriere die Verwendung der FolderPath-Eigenschaft
            Console.WriteLine("Font folder path: " + folderFontSource.FolderPath);
            Console.WriteLine("Scan subfolders: " + folderFontSource.ScanSubFolders);

            // Arbeitsmappe mit der Schriftartquelle erstellen
            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource });

            // Einfache Demonstration – Text hinzufügen, der benutzerdefinierte Schriftarten verwenden könnte
            workbook.Worksheets[0].Cells["A1"].PutValue("Font Source Demo");
            
            // Ausgaben speichern
            workbook.Save("FolderFontSourceDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [FolderFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


