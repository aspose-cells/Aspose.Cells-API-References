---
title: "PatternFill.ForegroundCellsColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PatternFill. Получает и задаёт объект foreground CellsColor"
type: docs
url: /ru/net/aspose.cells.drawing/patternfill/foregroundcellscolor/
---
## PatternFill.ForegroundCellsColor property

Получает и задаёт объект foreground [`CellsColor`](../../../aspose.cells/cellscolor/).

```csharp
public CellsColor ForegroundCellsColor { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class PatternFillPropertyForegroundCellsColorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте прямоугольную форму для демонстрации заполнения шаблоном
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 100);

            try
            {
                // Установите тип заливки в шаблон
                shape.Fill.FillType = FillType.Pattern;

                // Получите экземпляр PatternFill
                PatternFill patternFill = shape.Fill.PatternFill;

                // Установите тип шаблона и цвета
                patternFill.Pattern = FillPattern.WideDownwardDiagonal;
                patternFill.ForegroundColor = Color.Red;
                patternFill.BackgroundColor = Color.Yellow;

                // Создайте объект CellsColor для переднего плана, используя свойство Color
                // Поскольку у CellsColor нет публичного конструктора, мы будем использовать существующий ForegroundCellsColor
                // и изменим его свойства напрямую
                patternFill.ForegroundCellsColor.Color = Color.Blue;
                patternFill.ForegroundCellsColor.Argb = Color.Blue.ToArgb();

                // Отобразите свойства ForegroundCellsColor
                Console.WriteLine("ForegroundCellsColor Type: " + patternFill.ForegroundCellsColor.Type);
                Console.WriteLine("ForegroundCellsColor Color: " + patternFill.ForegroundCellsColor.Color);
                Console.WriteLine("ForegroundCellsColor ARGB: " + patternFill.ForegroundCellsColor.Argb);

                // Сохраните книгу
                workbook.Save("ForegroundCellsColorDemo.xlsx");
                Console.WriteLine("ForegroundCellsColor demonstration completed successfully.");
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

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


