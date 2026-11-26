---
title: "FillFormat.FillType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FillFormat. Получает и задает тип заполнения"
type: docs
url: /ru/net/aspose.cells.drawing/fillformat/filltype/
---
## FillFormat.FillType property

Получает и задает тип заливки.

```csharp
public FillType FillType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyFillTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить прямоугольную фигуру
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);

            // Установить сплошное заполнение с цветом
            shape.Fill.FillType = FillType.Solid;
            shape.Fill.SolidFill.Color = System.Drawing.Color.Red;

            // Вывести тип заполнения
            Console.WriteLine("Shape fill type: " + shape.Fill.FillType);

            // Переключить на градиентное заполнение
            shape.Fill.FillType = FillType.Gradient;
            Console.WriteLine("Shape fill type changed to: " + shape.Fill.FillType);

            // Сохраните книгу
            workbook.Save("FillTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [FillType](../../filltype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


