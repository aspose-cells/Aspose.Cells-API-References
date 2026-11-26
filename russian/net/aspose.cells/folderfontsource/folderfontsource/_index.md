---
title: "FolderFontSource.FolderFontSource"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор FolderFontSource. Ctor"
type: docs
url: /ru/net/aspose.cells/folderfontsource/folderfontsource/
---
## FolderFontSource constructor

Конструктор.

```csharp
public FolderFontSource(string folderPath, bool scanSubfolders)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| folderPath | String | путь к папке шрифтов |
| scanSubfolders | Boolean | Определяет, следует ли сканировать подпапки. |

### Примеры

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

### См. также

* class [FolderFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


