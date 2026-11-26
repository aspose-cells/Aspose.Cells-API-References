---
title: "Shape.Characters"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Shape. Возвращает объект Characters, представляющий диапазон символов внутри текста"
type: docs
url: /ru/net/aspose.cells.drawing/shape/characters/
---
## Shape.Characters method

Возвращает объект Characters, представляющий диапазон символов внутри текста.

```csharp
public FontSetting Characters(int startIndex, int length)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startIndex | Int32 | Индекс начала символа. |
| длина | Int32 | Количество символов. |

### Возвращаемое значение

Объект Characters.

### Примечания

Этот метод работает только с фигурой, имеющей заголовок.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodCharactersWithInt32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте форму с текстом
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);
            shape.Text = "Sample Text";

            // Получить символы, начиная с индекса 0, длиной 4
            FontSetting fontSetting = shape.Characters(0, 4);
            
            // Изменить настройки шрифта
            fontSetting.Font.Color = System.Drawing.Color.Red;
            fontSetting.Font.Size = 14;
            fontSetting.Font.IsBold = true;

            // Сохраните книгу
            workbook.Save("ShapeCharactersDemo.xlsx");
        }
    }
}
```

### См. также

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


