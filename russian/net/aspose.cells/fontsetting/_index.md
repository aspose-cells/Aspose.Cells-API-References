---
title: "Класс FontSetting"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.FontSetting. Представляет диапазон символов внутри текста ячейки"
type: docs
url: /ru/net/aspose.cells/fontsetting/
---
## FontSetting class

Представляет диапазон символов в тексте ячейки.

```csharp
public class FontSetting
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [FontSetting](fontsetting/)(int, int, WorksheetCollection) |  |

## Свойства

| Имя | Описание |
| --- | --- |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Возвращает шрифт этого объекта. |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Получает длину символов. |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Получает начальный индекс символов. |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Возвращает параметры текста. |
| virtual [Type](../../aspose.cells/fontsetting/type/) { get; } | Получает тип текстового узла. |

## Методы

| Имя | Описание |
| --- | --- |
| [SetWordArtStyle](../../aspose.cells/fontsetting/setwordartstyle/)(PresetWordArtStyle) | Устанавливает предустановленный стиль WordArt. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class FontSettingDemo
    {
        public static void FontSettingExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();

            // Добавление нового листа к объекту Excel
            workbook.Worksheets.Add();

            // Получение ссылки на только что добавленный лист путем передачи его индекса листа
            Worksheet worksheet = workbook.Worksheets[0];

            // Доступ к ячейке "A1" листа
            Aspose.Cells.Cell cell = worksheet.Cells["A1"];

            // Добавление некоторого значения в ячейку "A1"
            cell.PutValue("Visit Aspose!");

            // Получение диапазона символов
            FontSetting character = cell.Characters(6, 7);

            // Установка шрифта выбранных символов полужирным
            character.Font.IsBold = true;

            // Установка цвета шрифта выбранных символов в синий
            character.Font.Color = Color.Blue;

            // Сохранение файла Excel
            workbook.Save("FontSettingExample.xlsx");
            workbook.Save("FontSettingExample.pdf");

        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


