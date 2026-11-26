---
title: "Класс FolderFontSource"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.FolderFontSource. Представляет папку, содержащую файлы шрифтов TrueType"
type: docs
url: /ru/net/aspose.cells/folderfontsource/
---
## FolderFontSource class

Представляет папку, содержащую файлы шрифтов TrueType.

```csharp
public class FolderFontSource : FontSourceBase
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [FolderFontSource](folderfontsource/)(string, bool) | Конструктор. |

## Свойства

| Имя | Описание |
| --- | --- |
| [FolderPath](../../aspose.cells/folderfontsource/folderpath/) { get; } | Путь к папке шрифтов. |
| [ScanSubFolders](../../aspose.cells/folderfontsource/scansubfolders/) { get; } | Определяет, сканировать ли подпапки. |
| override [Type](../../aspose.cells/folderfontsource/type/) { get; } | Возвращает тип источника шрифтов. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FolderFontSourceDemo
    {
        public static void FolderFontSourceExample()
        {
            // Создайте экземпляр FolderFontSource
            string folderPath = @"C:\Fonts";
            bool scanSubfolders = true;
            FolderFontSource folderFontSource = new FolderFontSource(folderPath, scanSubfolders);

            // Доступ к свойствам
            Console.WriteLine("Folder Path: " + folderFontSource.FolderPath);
            Console.WriteLine("Scan Subfolders: " + folderFontSource.ScanSubFolders);
            Console.WriteLine("Font Source Type: " + folderFontSource.Type);

            // Создайте книгу и задайте источники шрифтов
            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource });

            // Сохраните книгу
            workbook.Save("FolderFontSourceExample.xlsx");
            workbook.Save("FolderFontSourceExample.pdf");
            return;
        }
    }
}
```

### См. также

* class [FontSourceBase](../fontsourcebase/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


