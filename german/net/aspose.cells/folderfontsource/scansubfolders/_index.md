---
title: "FolderFontSource.ScanSubFolders"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FolderFontSource-Eigenschaft. Bestimmt, ob die Unterordner gescannt werden sollen oder nicht"
type: docs
url: /de/net/aspose.cells/folderfontsource/scansubfolders/
---
## FolderFontSource.ScanSubFolders property

Bestimmt, ob Unterordner durchsucht werden sollen oder nicht.

```csharp
public bool ScanSubFolders { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FolderFontSourcePropertyScanSubFoldersDemo
    {
        public static void Run()
        {
            // Erstelle eine FolderFontSource mit aktivierter Unterordnererkennung
            string folderPath = @"C:\Windows\Fonts"; // Typical system fonts folder
            bool scanSubfolders = true;
            FolderFontSource folderFontSource = new FolderFontSource(folderPath, scanSubfolders);

            // Schriftquellen‑Eigenschaften anzeigen
            Console.WriteLine("Folder Path: " + folderFontSource.FolderPath);
            Console.WriteLine("Scan Subfolders: " + folderFontSource.ScanSubFolders);

            // Erstelle eine Arbeitsmappe und setze die Font-Quelle
            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource });

            // Demonstriere die Verwendung, indem du Text festlegst
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Text with fonts from folder source");

            // Speichere die Arbeitsmappe
            workbook.Save("FolderFontSourceDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [FolderFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


