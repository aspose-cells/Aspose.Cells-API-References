---
title: "FolderFontSource.FolderPath"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FolderFontSource. Путь к папке шрифтов"
type: docs
url: /ru/net/aspose.cells/folderfontsource/folderpath/
---
## FolderFontSource.FolderPath property

Путь к папке шрифтов.

```csharp
public string FolderPath { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FolderFontSourcePropertyFolderPathDemo
    {
        public static void Run()
        {
            // Создать источник шрифтов из папки
            string folderPath = @"C:\Windows\Fonts"; // Typical system fonts folder
            bool scanSubfolders = true;
            FolderFontSource folderFontSource = new FolderFontSource(folderPath, scanSubfolders);

            // Продемонстрируйте использование свойства FolderPath
            Console.WriteLine("Font folder path: " + folderFontSource.FolderPath);
            Console.WriteLine("Scan subfolders: " + folderFontSource.ScanSubFolders);

            // Создайте рабочую книгу с источником шрифтов
            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource });

            // Простая демонстрация — добавьте текст, который может использовать пользовательские шрифты
            workbook.Worksheets[0].Cells["A1"].PutValue("Font Source Demo");
            
            // Сохраните результаты
            workbook.Save("FolderFontSourceDemo.xlsx");
        }
    }
}
```

### См. также

* class [FolderFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


