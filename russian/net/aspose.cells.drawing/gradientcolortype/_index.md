---
title: "Перечисление GradientColorType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Drawing.GradientColorType перечисление. Представляет тип градиентного цвета для указанного заполнения"
type: docs
url: /ru/net/aspose.cells.drawing/gradientcolortype/
---
## GradientColorType enumeration

Представляет тип градиентного цвета для указанной заливки.

```csharp
public enum GradientColorType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Без градиентного цвета |
| OneColor | `1` | Один градиентный цвет |
| PresetColors | `2` | Предустановленные градиентные цвета |
| TwoColors | `3` | Два градиентных цвета |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassGradientColorTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу для демонстрации
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Добавьте форму, чтобы продемонстрировать заливку градиентом
                Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 200, 200);
                FillFormat fill = shape.Fill;

                // Установите тип заливки градиентом
                fill.FillType = FillType.Gradient;

                // Продемонстрируйте различные значения перечисления GradientColorType
                Console.WriteLine("Available GradientColorType values:");
                Console.WriteLine("None: " + GradientColorType.None);
                Console.WriteLine("OneColor: " + GradientColorType.OneColor);
                Console.WriteLine("PresetColors: " + GradientColorType.PresetColors);
                Console.WriteLine("TwoColors: " + GradientColorType.TwoColors);

                // Прочитайте и отобразите текущий тип градиентного цвета (свойство только для чтения)
                Console.WriteLine("Current gradient color type: " + fill.GradientColorType);

                // Сохраните книгу
                workbook.Save("GradientColorTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with GradientColorType: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


