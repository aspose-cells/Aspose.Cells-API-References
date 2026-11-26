---
title: "Класс FileFontSource"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.FileFontSource. Представляет отдельный файл TrueType шрифта, хранящийся в файловой системе"
type: docs
url: /ru/net/aspose.cells/filefontsource/
---
## FileFontSource class

Представляет отдельный файл шрифта TrueType, хранящийся в файловой системе.

```csharp
public class FileFontSource : FontSourceBase
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [FileFontSource](filefontsource/)(string) | Конструктор. |

## Свойства

| Имя | Описание |
| --- | --- |
| [FilePath](../../aspose.cells/filefontsource/filepath/) { get; } | Путь к файлу шрифта. |
| override [Type](../../aspose.cells/filefontsource/type/) { get; } | Возвращает тип источника шрифтов. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FileFontSourceDemo
    {
        public static void FileFontSourceExample()
        {
            // Укажите путь к файлу TrueType шрифта
            string fontFilePath = "C:\\Fonts\\CustomFont.ttf";

            // Создать экземпляр FileFontSource
            FileFontSource fontSource = new FileFontSource(fontFilePath);

            // Отобразить тип источника шрифта и путь к файлу
            Console.WriteLine("Font Source Type: " + fontSource.Type);
            Console.WriteLine("Font File Path: " + fontSource.FilePath);

            // Создать объект Workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Установить значение ячейки
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Hello, Aspose!");

            // Применить пользовательский шрифт к ячейке
            Style style = cell.GetStyle();
            style.Font.Name = "CustomFont"; // Use the name of the font
            cell.SetStyle(style);

            // Сохраните книгу
            workbook.Save("FileFontSourceExample.xlsx");
            workbook.Save("FileFontSourceExample.pdf");
        }
    }
}
```

### См. также

* class [FontSourceBase](../fontsourcebase/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


