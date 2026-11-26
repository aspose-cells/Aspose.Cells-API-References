---
title: "MsoLineFormat.IsVisible"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MsoLineFormat. Указывает, видим ли объект"
type: docs
url: /ru/net/aspose.cells.drawing/msolineformat/isvisible/
---
## MsoLineFormat.IsVisible property

Указывает, видим ли объект.

```csharp
public bool IsVisible { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте прямоугольную форму с видимой рамкой
            var shape1 = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
            shape1.LineFormat.IsVisible = true;

            // Добавьте овальную форму с невидимой рамкой
            var shape2 = worksheet.Shapes.AddOval(2, 0, 150, 100, 100, 100);
            shape2.LineFormat.IsVisible = false;

            // Проверьте и выведите значения свойства IsVisible
            Console.WriteLine("Rectangle border visible: " + shape1.LineFormat.IsVisible);
            Console.WriteLine("Oval border visible: " + shape2.LineFormat.IsVisible);

            // Сохраните книгу
            workbook.Save("MsoLineFormat_IsVisible_Demo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


