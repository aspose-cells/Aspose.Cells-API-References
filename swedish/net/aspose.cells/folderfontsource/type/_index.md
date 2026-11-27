---
title: "FolderFontSource.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FolderFontSource-egenskap. Returnerar typen av teckensnittskällan"
type: docs
url: /sv/net/aspose.cells/folderfontsource/type/
---
## FolderFontSource.Type property

Returnerar typen av teckensnittskälla.

```csharp
public override FontSourceType Type { get; }
```

### Exempel

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

### Se även

* enum [FontSourceType](../../fontsourcetype/)
* class [FolderFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


