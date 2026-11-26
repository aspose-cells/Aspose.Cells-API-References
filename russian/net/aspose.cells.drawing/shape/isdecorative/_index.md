---
title: "Shape.IsDecorative"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Указывает, является ли объект декоративным"
type: docs
url: /ru/net/aspose.cells.drawing/shape/isdecorative/
---
## Shape.IsDecorative property

Указывает, является ли объект декоративным.

```csharp
public bool IsDecorative { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsDecorativeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить прямоугольную фигуру
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);
            
            // Установить форму как декоративную
            shape.IsDecorative = true;
            
            // Сохраните книгу
            string outputPath = "ShapeIsDecorativeDemo.xlsx";
            workbook.Save(outputPath);
            
            // Перезагрузите рабочую книгу, чтобы проверить свойство
            Workbook loadedWorkbook = new Workbook(outputPath);
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            
            // Вывести результат.
            Console.WriteLine("Shape IsDecorative property: " + loadedShape.IsDecorative);
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


