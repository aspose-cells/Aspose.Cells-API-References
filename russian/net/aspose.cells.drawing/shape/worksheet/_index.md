---
title: "Shape.Worksheet"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает объект Worksheet, содержащий эту фигуру"
type: docs
url: /ru/net/aspose.cells.drawing/shape/worksheet/
---
## Shape.Worksheet property

Получает объект [`Worksheet`](../../../aspose.cells/worksheet/) который содержит эту фигуру.

```csharp
public Worksheet Worksheet { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWorksheetDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить форму на лист
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
            
            // Продемонстрировать использование свойства Worksheet
            Worksheet shapeWorksheet = shape.Worksheet;
            
            // Вывести имя листа, чтобы показать, что свойство работает
            Console.WriteLine("Shape belongs to worksheet: " + shapeWorksheet.Name);
        }
    }
}
```

### См. также

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


