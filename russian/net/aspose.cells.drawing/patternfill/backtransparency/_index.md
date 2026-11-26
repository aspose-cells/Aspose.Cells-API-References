---
title: "PatternFill.BackTransparency"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PatternFill. Получает или задает прозрачность цвета фона"
type: docs
url: /ru/net/aspose.cells.drawing/patternfill/backtransparency/
---
## PatternFill.BackTransparency property

Получает или задает прозрачность фонового цвета.

```csharp
public double BackTransparency { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class PatternFillPropertyBackTransparencyDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить прямоугольную фигуру на лист
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 200, 200);

            // Получите существующий экземпляр PatternFill из фигуры и настройте свойства
            shape.Fill.FillType = FillType.Pattern;
            PatternFill patternFill = shape.Fill.PatternFill;
            patternFill.Pattern = FillPattern.Solid;
            patternFill.BackgroundColor = Color.Blue;

            // Отобразите начальное значение BackTransparency
            Console.WriteLine("Current BackTransparency value: " + patternFill.BackTransparency);

            // Установите новое значение BackTransparency (прозрачность 50%)
            patternFill.BackTransparency = 0.5;

            // Сохранить изменённую книгу
            workbook.Save("PatternFillBackTransparencyDemo.xlsx");
        }
    }
}
```

### См. также

* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


