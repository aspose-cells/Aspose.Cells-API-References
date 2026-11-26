---
title: "Класс Font"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Font класс. Инкапсулирует объект шрифта, используемый в электронных таблицах"
type: docs
url: /ru/net/aspose.cells/font/
---
## Font class

Инкапсулирует объект шрифта, используемый в электронных таблицах.

```csharp
public class Font
```

## Свойства

| Имя | Описание |
| --- | --- |
| [ArgbColor](../../aspose.cells/font/argbcolor/) { get; set; } | Получает и задаёт цвет в виде 32‑битного значения ARGB. |
| [CapsType](../../aspose.cells/font/capstype/) { get; set; } | (**Obsolete.**) Получает и задаёт тип заглавных букв текста. |
| [Charset](../../aspose.cells/font/charset/) { get; set; } | Представляет набор символов. |
| [Color](../../aspose.cells/font/color/) { get; set; } | Получает или задаёт цвет шрифта. |
| [DoubleSize](../../aspose.cells/font/doublesize/) { get; set; } | Получает и задает двойной размер шрифта. |
| [IsBold](../../aspose.cells/font/isbold/) { get; set; } | Получает или задает значение, указывающее, является ли шрифт полужирным. |
| [IsItalic](../../aspose.cells/font/isitalic/) { get; set; } | Получает или задает значение, указывающее, является ли шрифт курсивом. |
| [IsNormalizeHeights](../../aspose.cells/font/isnormalizeheights/) { get; set; } | (**Obsolete.**) Указывает, будет ли применяться нормализация высоты к последовательности текста. |
| [IsStrikeout](../../aspose.cells/font/isstrikeout/) { get; set; } | Получает или задает значение, указывающее, имеет ли шрифт одинарное зачеркивание. |
| [IsSubscript](../../aspose.cells/font/issubscript/) { get; set; } | Получает или задает значение, указывающее, является ли шрифт нижним индексом. |
| [IsSuperscript](../../aspose.cells/font/issuperscript/) { get; set; } | Получает или задает значение, указывающее, является ли шрифт верхним индексом. |
| virtual [Name](../../aspose.cells/font/name/) { get; set; } | Получает или задает имя `Font`. |
| [SchemeType](../../aspose.cells/font/schemetype/) { get; set; } | Получает и задает тип схемы шрифта. |
| [ScriptOffset](../../aspose.cells/font/scriptoffset/) { get; set; } | Получает и задает смещение скрипта в процентах |
| [Size](../../aspose.cells/font/size/) { get; set; } | Получает или задает размер шрифта. |
| [StrikeType](../../aspose.cells/font/striketype/) { get; set; } | Получает тип зачеркивания текста. |
| [ThemeColor](../../aspose.cells/font/themecolor/) { get; set; } | Получает и задает цвет темы. |
| [Underline](../../aspose.cells/font/underline/) { get; set; } | Получает или задает тип подчеркивания шрифта. |

## Методы

| Имя | Описание |
| --- | --- |
| [Equals](../../aspose.cells/font/equals/#equals)(Font) | Проверяет, равны ли два шрифта. |
| [SetName](../../aspose.cells/font/setname/)(string, FontSchemeType) | Задает имя и схему шрифта. |
| override [ToString](../../aspose.cells/font/tostring/)() | Возвращает строку, представляющую текущий объект Cell. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class FontDemo
    {
        public static void FontExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();

            // Получение ссылки на только что добавленный лист путем передачи его индекса листа
            Worksheet worksheet = workbook.Worksheets[0];

            // Доступ к ячейке "A1" листа
            Aspose.Cells.Cell cell = worksheet.Cells["A1"];

            // Добавление некоторого значения в ячейку "A1"
            cell.PutValue("Hello Aspose!");

            // Доступ к объекту шрифта стиля ячейки
            Aspose.Cells.Font font = cell.GetStyle().Font;

            // Установка имени шрифта в "Times New Roman"
            font.Name = "Times New Roman";

            // Установка размера шрифта в 14
            font.Size = 14;

            // Установка цвета шрифта как Красный
            font.Color = Color.Red;

            // Установка дополнительных свойств шрифта
            font.IsBold = true;
            font.IsItalic = true;
            font.Underline = FontUnderlineType.Single;
            font.IsStrikeout = false;
            font.IsSuperscript = false;
            font.IsSubscript = false;
            font.Charset = 1;
            font.CapsType = TextCapsType.None;
            font.StrikeType = TextStrikeType.None;
            font.ScriptOffset = 0;
            font.DoubleSize = 14.0;
            font.ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);
            font.ArgbColor = Color.Red.ToArgb();
            font.IsNormalizeHeights = false;
            font.SchemeType = FontSchemeType.None;

            // Сохранение файла Excel
            workbook.Save("FontExample.xlsx");
            workbook.Save("FontExample.pdf");
            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


