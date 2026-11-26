---
title: "Shape.IsWordArt"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Указывает, является ли эта фигура WordArt"
type: docs
url: /ru/net/aspose.cells.drawing/shape/iswordart/
---
## Shape.IsWordArt property

Указывает, является ли эта фигура WordArt.

```csharp
public bool IsWordArt { get; }
```

### Примечания

Только для устаревшей формы в файле xls.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsWordArtDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму WordArt со всеми необходимыми параметрами
            Shape wordArt = worksheet.Shapes.AddWordArt(PresetWordArtStyle.WordArtStyle1, "Sample WordArt", 0, 0, 100, 100, 100, 100);

            // Добавить обычную прямоугольную форму со всеми необходимыми параметрами
            Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 150, 100, 100, 100);

            // Проверить, являются ли формы WordArt
            Console.WriteLine("WordArt shape is WordArt: " + wordArt.IsWordArt);
            Console.WriteLine("Rectangle shape is WordArt: " + rectangle.IsWordArt);

            // Пример использования свойства IsWordArt
            if (wordArt.IsWordArt)
            {
                Console.WriteLine("First shape is a WordArt object");
            }

            if (!rectangle.IsWordArt)
            {
                Console.WriteLine("Second shape is not a WordArt object");
            }
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


