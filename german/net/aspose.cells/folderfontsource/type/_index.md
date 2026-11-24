---
title: "FolderFontSource.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FolderFontSource-Eigenschaft. Gibt den Typ der Font-Quelle zurück"
type: docs
url: /de/net/aspose.cells/folderfontsource/type/
---
## FolderFontSource.Type property

Gibt den Typ der Schriftquellen zurück.

```csharp
public override FontSourceType Type { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FolderFontSourcePropertyTypeDemo
    {
        public static void Run()
        {
            string folderPath = @"C:\Fonts";
            bool scanSubfolders = true;
            FolderFontSource folderFontSource = new FolderFontSource(folderPath, scanSubfolders);

            Console.WriteLine("Folder Path: " + folderFontSource.FolderPath);
            Console.WriteLine("Scan Subfolders: " + folderFontSource.ScanSubFolders);
            Console.WriteLine("Font Source Type: " + folderFontSource.Type);

            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource });

            workbook.Save("FolderFontSourceExample.xlsx");
        }
    }
}
```

### Siehe auch

* enum [FontSourceType](../../fontsourcetype/)
* class [FolderFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


