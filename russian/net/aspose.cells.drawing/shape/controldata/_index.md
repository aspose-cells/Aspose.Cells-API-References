---
title: "Shape.ControlData"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает данные управления"
type: docs
url: /ru/net/aspose.cells.drawing/shape/controldata/
---
## Shape.ControlData property

Получает данные управления.

```csharp
public byte[] ControlData { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyControlDataDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить фигуру с правильными параметрами
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
            
            // Доступ к ControlData (только для чтения)
            byte[] controlData = shape.ControlData;

            // Проверить ControlData
            if (controlData != null)
            {
                Console.WriteLine("ControlData exists with length: " + controlData.Length);
            }
            else
            {
                Console.WriteLine("No data.");
            }
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


