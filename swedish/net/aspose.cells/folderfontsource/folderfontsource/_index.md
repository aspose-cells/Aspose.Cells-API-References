---
title: "FolderFontSource.FolderFontSource"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FolderFontSource-konstruktor. Ctor"
type: docs
url: /sv/net/aspose.cells/folderfontsource/folderfontsource/
---
## FolderFontSource constructor

Konstruktor.

```csharp
public FolderFontSource(string folderPath, bool scanSubfolders)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| folderPath | String | sökväg till teckensnittsmappen |
| scanSubfolders | Boolean | Avgör om underkataloger ska skannas eller inte. |

### Exempel

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

### Se även

* class [FolderFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


