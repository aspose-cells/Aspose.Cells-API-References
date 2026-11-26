---
title: "PatternFill.ForeTransparency"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PatternFill. Получает или задает прозрачность цвета переднего плана"
type: docs
url: /ru/net/aspose.cells.drawing/patternfill/foretransparency/
---
## PatternFill.ForeTransparency property

Получает или задает прозрачность переднего цвета.

```csharp
public double ForeTransparency { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class PatternFillPropertyForeTransparencyDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте прямоугольную форму для демонстрации заполнения шаблоном
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 100);

            // Установите тип заливки в шаблон
            shape.Fill.FillType = FillType.Pattern;

            // Получите экземпляр PatternFill
            PatternFill patternFill = shape.Fill.PatternFill;

            // Настройте свойства заливки шаблоном
            patternFill.Pattern = FillPattern.Solid;
            patternFill.ForegroundColor = Color.Red;
            patternFill.BackgroundColor = Color.Blue;

            try
            {
                // Отобразите начальное значение ForeTransparency
                Console.WriteLine("Initial ForeTransparency value: " + patternFill.ForeTransparency);

                // Установите новое значение ForeTransparency (прозрачность 50%)
                patternFill.ForeTransparency = 0.5;

                // Отобразите обновлённое значение ForeTransparency
                Console.WriteLine("Updated ForeTransparency value: " + patternFill.ForeTransparency);

                // Сохраните книгу
                workbook.Save("ForeTransparencyDemo.xlsx");
                Console.WriteLine("ForeTransparency demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


