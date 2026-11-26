---
title: "FillFormat.SetTwoColorGradient"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод FillFormat. Устанавливает указанное заполнение в двухцветный градиент. Применяется только для Excel 2007"
type: docs
url: /ru/net/aspose.cells.drawing/fillformat/settwocolorgradient/
---
## SetTwoColorGradient(Color, Color, GradientStyleType, int) {#settwocolorgradient_1}

Устанавливает указанное заполнение в двухцветный градиент. Применяется только для Excel 2007.

```csharp
public void SetTwoColorGradient(Color color1, Color color2, GradientStyleType style, int variant)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| color1 | Color | Один цвет градиента. |
| color2 | Color | Два цвета градиента. |
| стиль | GradientStyleType | Стиль затенения градиента. |
| variant | Int32 | Вариант градиента. Может принимать значение от 1 до 4, соответствующее одному из четырёх вариантов на вкладке Gradient в диалоговом окне Fill Effects. Если стиль равен GradientStyle.FromCenter, аргумент Variant может быть только 1 или 2. |

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatMethodSetTwoColorGradientWithColorColorGradientStyleTypeIntDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте простую форму для демонстрации градиентного заполнения
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 5, 100, 100);

            // Получите формат заполнения фигуры
            FillFormat fillFormat = shape.Fill;

            // Установите двухцветный градиент с указанными параметрами
            fillFormat.SetTwoColorGradient(Color.Blue, Color.LightBlue, GradientStyleType.DiagonalDown, 1);

            // Сохраните книгу
            workbook.Save("TwoColorGradientDemo.xlsx");
        }
    }
}
```

### См. также

* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## SetTwoColorGradient(Color, double, Color, double, GradientStyleType, int) {#settwocolorgradient}

Устанавливает указанное заполнение в двухцветный градиент. Применяется только для Excel 2007.

```csharp
public void SetTwoColorGradient(Color color1, double transparency1, Color color2, 
    double transparency2, GradientStyleType style, int variant)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| color1 | Color | Один цвет градиента. |
| transparency1 | Double | Степень прозрачности цвета1 в виде значения от 0.0 (непрозрачный) до 1.0 (прозрачный). |
| color2 | Color | Два цвета градиента. |
| transparency2 | Double | Степень прозрачности цвета2 в виде значения от 0.0 (непрозрачный) до 1.0 (прозрачный). |
| стиль | GradientStyleType | Стиль затенения градиента. |
| variant | Int32 | Вариант градиента. Может принимать значение от 1 до 4, соответствующее одному из четырёх вариантов на вкладке Gradient в диалоговом окне Fill Effects. Если стиль равен GradientStyle.FromCenter, аргумент Variant может быть только 1 или 2. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class FillFormatMethodSetTwoColorGradientWithColorDoubleColorDoubleGradientDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте прямоугольную форму для демонстрации форматирования заполнения
            var rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 5, 150, 100);
            FillFormat fillFormat = rectangle.Fill;

            try
            {
                // Подготовьте параметры для SetTwoColorGradient
                Color color1 = Color.Red;
                double transparency1 = 0.3;
                Color color2 = Color.Blue;
                double transparency2 = 0.7;
                GradientStyleType gradientStyle = GradientStyleType.Horizontal;
                int variant = 1;

                // Вызовите SetTwoColorGradient с конкретными параметрами
                fillFormat.SetTwoColorGradient(
                    color1, 
                    transparency1, 
                    color2, 
                    transparency2, 
                    gradientStyle, 
                    variant
                );

                Console.WriteLine("SetTwoColorGradient executed successfully with parameters (Color, Double, Color, Double, GradientStyleType, Int32)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTwoColorGradient: {ex.Message}");
            }

            // Сохраните книгу, чтобы показать эффект
            workbook.Save("SetTwoColorGradientDemo.xlsx");
        }
    }
}
```

### См. также

* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


