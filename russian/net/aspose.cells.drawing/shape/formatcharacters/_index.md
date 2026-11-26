---
title: "Shape.FormatCharacters"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Shape. Форматирует некоторые символы с настройкой шрифта"
type: docs
url: /ru/net/aspose.cells.drawing/shape/formatcharacters/
---
## Shape.FormatCharacters method

Форматирует некоторые символы с использованием настроек шрифта.

```csharp
public void FormatCharacters(int startIndex, int length, Font font, StyleFlag flag)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startIndex | Int32 | Начальный индекс. |
| длина | Int32 | Длина. |
| шрифт | Шрифт | Настройка шрифта. |
| флаг | StyleFlag | Флаг настройки шрифта. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodFormatCharactersWithInt32Int32FontStyleFlagDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить текстовое поле на лист
            Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);
            textBox.Text = "Sample Text Formatting";
            
            // Создать шрифт с нужными свойствами
            Aspose.Cells.Font font = textBox.Font;
            font.Name = "Arial";
            font.Size = 12;
            font.IsBold = true;
            
            // Создать флаг стиля, чтобы указать, какие свойства применять
            StyleFlag flag = new StyleFlag();
            flag.FontName = true;
            flag.FontSize = true;
            flag.FontBold = true;
            
            // Применить форматирование к определённым символам
            textBox.FormatCharacters(0, 6, font, flag);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Font](../../../aspose.cells/font/)
* class [StyleFlag](../../../aspose.cells/styleflag/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


