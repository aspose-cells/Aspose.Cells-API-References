---
title: "Shape.MacroName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает и задает имя макроса"
type: docs
url: /ru/net/aspose.cells.drawing/shape/macroname/
---
## Shape.MacroName property

Получает и задает имя макроса.

```csharp
public string MacroName { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyMacroNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму на лист
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Установить имя макроса для фигуры
            shape.MacroName = "DoWork()";

            // Вывести подтверждение
            Console.WriteLine("Shape macro name set to: " + shape.MacroName);
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


