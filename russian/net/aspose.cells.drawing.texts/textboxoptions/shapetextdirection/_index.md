---
title: "TextBoxOptions.ShapeTextDirection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextBoxOptions. Получает или задает направление отображения текста внутри заданного текстового блока. Это соответствует Format Shape  Text Options  Text Box  Text direction в Excel"
type: docs
url: /ru/net/aspose.cells.drawing.texts/textboxoptions/shapetextdirection/
---
## TextBoxOptions.ShapeTextDirection property

Получает или задает направление отображения текста внутри заданного текстового блока. Соответствует "Форматировать форму - Параметры текста - Текстовое поле - Направление текста" в Excel

```csharp
public TextVerticalType ShapeTextDirection { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyShapeTextDirectionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму текстового поля
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);

            // Установить направление текста вертикально
            shape.TextBoxOptions.ShapeTextDirection = TextVerticalType.Vertical;

            // Установить некоторый текст для демонстрации направления
            shape.Text = "Vertical Text Example";

            // Сохраните книгу
            workbook.Save("TextBoxTextDirectionDemo.xlsx");
        }
    }
}
```

### См. также

* enum [TextVerticalType](../../textverticaltype/)
* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


