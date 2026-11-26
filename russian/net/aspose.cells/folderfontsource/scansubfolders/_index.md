---
title: "FolderFontSource.ScanSubFolders"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FolderFontSource. Определяет, следует ли сканировать подпапки"
type: docs
url: /ru/net/aspose.cells/folderfontsource/scansubfolders/
---
## FolderFontSource.ScanSubFolders property

Определяет, сканировать ли подпапки.

```csharp
public bool ScanSubFolders { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FolderFontSourcePropertyScanSubFoldersDemo
    {
        public static void Run()
        {
            // Создайте источник шрифтов из папки с включённым сканированием подпапок
            string folderPath = @"C:\Windows\Fonts"; // Typical system fonts folder
            bool scanSubfolders = true;
            FolderFontSource folderFontSource = new FolderFontSource(folderPath, scanSubfolders);

            // Отобразить свойства источника шрифтов
            Console.WriteLine("Folder Path: " + folderFontSource.FolderPath);
            Console.WriteLine("Scan Subfolders: " + folderFontSource.ScanSubFolders);

            // Создайте рабочую книгу и задайте источник шрифтов
            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource });

            // Продемонстрируйте использование, задав некоторый текст
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Text with fonts from folder source");

            // Сохраните книгу
            workbook.Save("FolderFontSourceDemo.xlsx");
        }
    }
}
```

### См. также

* class [FolderFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


