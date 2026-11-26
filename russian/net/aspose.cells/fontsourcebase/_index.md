---
title: "Класс FontSourceBase"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.FontSourceBase. Это абстрактный базовый класс для классов, позволяющих пользователю указывать различные источники шрифтов"
type: docs
url: /ru/net/aspose.cells/fontsourcebase/
---
## FontSourceBase class

Это абстрактный базовый класс для классов, позволяющих пользователю указывать различные источники шрифтов.

```csharp
public abstract class FontSourceBase
```

## Свойства

| Имя | Описание |
| --- | --- |
| abstract [Type](../../aspose.cells/fontsourcebase/type/) { get; } | Возвращает тип источника шрифтов. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFontSourceBaseDemo
    {
        public static void Run()
        {
            // Создать источник шрифтов из папки
            string fontFolder = @"C:\Windows\Fonts";
            FolderFontSource folderSource = new FolderFontSource(fontFolder, true);

            // Отобразить свойства источника шрифтов
            Console.WriteLine($"Font folder: {folderSource.FolderPath}");
            Console.WriteLine($"Scan subfolders: {folderSource.ScanSubFolders}");
            Console.WriteLine($"Source type: {folderSource.Type}");

            // Создать книгу и установить источник шрифта
            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderSource });

            // Сохранить с пользовательскими шрифтами
            workbook.Save("OutputWithCustomFonts.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


