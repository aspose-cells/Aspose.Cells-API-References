---
title: "FolderFontSource.FolderFontSource"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FolderFontSource Konstruktor. Ctor"
type: docs
url: /de/net/aspose.cells/folderfontsource/folderfontsource/
---
## FolderFontSource constructor

Ctor.

```csharp
public FolderFontSource(string folderPath, bool scanSubfolders)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| folderPath | String | Pfad zum Schriftartenordner |
| scanSubfolders | Boolean | Bestimmt, ob Unterordner gescannt werden sollen oder nicht. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FolderFontSourceMethodCtorWithStringBooleanDemo
    {
        public static void Run()
        {
            string folderPath = @"C:\Fonts";
            bool scanSubfolders = true;
            FolderFontSource folderFontSource = new FolderFontSource(folderPath, scanSubfolders);

            Console.WriteLine("Folder Path: " + folderFontSource.FolderPath);
            Console.WriteLine("Scan Subfolders: " + folderFontSource.ScanSubFolders);

            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource });
            workbook.Save("FolderFontSourceExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [FolderFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


