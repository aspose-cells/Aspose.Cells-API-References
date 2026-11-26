---
title: "Shape.GetRichFormattings"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Shape. Возвращает все объекты Characters, представляющие диапазон символов в тексте"
type: docs
url: /ru/net/aspose.cells.drawing/shape/getrichformattings/
---
## Shape.GetRichFormattings method

Возвращает все объекты Characters, представляющие диапазон символов внутри текста.

```csharp
public FontSetting[] GetRichFormattings()
```

### Возвращаемое значение

Все объекты Characters

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetRichFormattingsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить фигуру с форматированным текстом (правильное количество параметров для AddRectangle)
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);
            shape.Text = "This is bold and this is italic";
            
            // Форматировать части текста
            shape.Characters(0, 4).Font.IsBold = true;
            shape.Characters(13, 6).Font.IsItalic = true;

            // Получить форматирование богатого текста
            FontSetting[] formattings = shape.GetRichFormattings();

            // Отобразить информацию о форматировании
            Console.WriteLine("Rich text formattings:");
            foreach (FontSetting setting in formattings)
            {
                Console.WriteLine($"Text segment: '{shape.Text.Substring(setting.StartIndex, setting.Length)}'");
                Console.WriteLine($"Start index: {setting.StartIndex}");
                Console.WriteLine($"Length: {setting.Length}");
                Console.WriteLine($"Bold: {setting.Font.IsBold}");
                Console.WriteLine($"Italic: {setting.Font.IsItalic}");
                Console.WriteLine();
            }
        }
    }
}
```

### См. также

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


