---
title: "FolderFontSource.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FolderFontSource. Возвращает тип источника шрифтов"
type: docs
url: /ru/net/aspose.cells/folderfontsource/type/
---
## FolderFontSource.Type property

Возвращает тип источника шрифтов.

```csharp
public override FontSourceType Type { get; }
```

### Примеры

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

### См. также

* enum [FontSourceType](../../fontsourcetype/)
* class [FolderFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


