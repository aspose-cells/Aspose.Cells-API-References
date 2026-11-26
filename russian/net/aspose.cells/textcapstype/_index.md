---
title: "Перечисление TextCapsType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.TextCapsType enum. Этот тип определяет типы заглавных букв в тексте"
type: docs
url: /ru/net/aspose.cells/textcapstype/
---
## TextCapsType enumeration

Этот тип указывает типы заглавных букв текста.

```csharp
public enum TextCapsType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Без заглавных |
| All | `1` | Применить все заглавные к тексту. |
| Small | `2` | Применить малые заглавные к тексту. |

### Примечания

Можно применить только к диаграмме и фигуре.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TextCapsTypeDemo
    {
        public static void TextCapsTypeExample()
        {
            // Дополнительный код, демонстрирующий, как может использоваться экземпляр
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Задать значение ячейки
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Hello Aspose!");

            // Получить стиль ячейки
            Style style = cell.GetStyle();

            // Задать тип заглавных шрифта как All Caps
            style.Font.CapsType = Aspose.Cells.TextCapsType.All;

            // Применить стиль к ячейке
            cell.SetStyle(style);

            // Сохраните книгу
            workbook.Save("TextCapsTypeExample.xlsx");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


