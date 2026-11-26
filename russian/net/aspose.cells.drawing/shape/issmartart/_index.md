---
title: "Shape.IsSmartArt"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Указывает, является ли объект smart art"
type: docs
url: /ru/net/aspose.cells.drawing/shape/issmartart/
---
## Shape.IsSmartArt property

Указывает, является ли фигура SmartArt.

```csharp
public bool IsSmartArt { get; }
```

### Примечания

Только для файлов ooxml.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsSmartArtDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить SmartArt-объект (Примечание: Aspose.Cells напрямую не предоставляет создание SmartArt в текущих версиях)
            // Для демонстрации мы проверим существующие фигуры
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Проверьте, является ли фигура SmartArt
            if (shape.IsSmartArt)
            {
                Console.WriteLine("The shape is a SmartArt object");
            }
            else
            {
                Console.WriteLine("The shape is not a SmartArt object");
            }
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


