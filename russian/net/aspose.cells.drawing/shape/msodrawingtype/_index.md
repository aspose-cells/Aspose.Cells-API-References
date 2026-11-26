---
title: "Shape.MsoDrawingType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает тип рисунка"
type: docs
url: /ru/net/aspose.cells.drawing/shape/msodrawingtype/
---
## Shape.MsoDrawingType property

Получает тип рисунка.

```csharp
public MsoDrawingType MsoDrawingType { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyMsoDrawingTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить прямоугольную фигуру (исправленные параметры)
            Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 50);
            
            // Получить и отобразить MsoDrawingType фигуры
            MsoDrawingType drawingType = rectangle.MsoDrawingType;
            Console.WriteLine("Shape MsoDrawingType: " + drawingType.ToString());

            // Добавить линейную фигуру (исправленные параметры)
            Shape line = worksheet.Shapes.AddLine(3, 0, 3, 100, 150, 1);
            
            // Получить и отобразить MsoDrawingType линии
            drawingType = line.MsoDrawingType;
            Console.WriteLine("Line MsoDrawingType: " + drawingType.ToString());
        }
    }
}
```

### См. также

* enum [MsoDrawingType](../../msodrawingtype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


