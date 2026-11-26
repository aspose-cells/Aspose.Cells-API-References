---
title: "Shape.RemoveHyperlink"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Shape. Удаляет гиперссылку фигуры"
type: docs
url: /ru/net/aspose.cells.drawing/shape/removehyperlink/
---
## Shape.RemoveHyperlink method

Удаляет гиперссылку фигуры.

```csharp
public void RemoveHyperlink()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodRemoveHyperlinkDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить фигуру и установить гиперссылку
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 50);
            shape.AddHyperlink("https://www.aspose.com");

            // Удалить гиперссылку
            shape.RemoveHyperlink();

            // Проверить, что гиперссылка удалена
            Console.WriteLine("Hyperlink removed: " + (shape.Hyperlink == null));

            // Сохраните книгу
            workbook.Save("ShapeRemoveHyperlinkDemo.xlsx");
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


