---
title: "GradientFill.SetTwoColorGradient"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GradientFill. Устанавливает указанную заливку в двухцветный градиент. Применяется только для Excel 2007"
type: docs
url: /ru/net/aspose.cells.drawing/gradientfill/settwocolorgradient/
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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientFillMethodSetTwoColorGradientWithColorColorGradientStyleTyInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить фигуру для применения градиентной заливки
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            try
            {
                // Установить тип заливки как градиент
                shape.Fill.FillType = FillType.Gradient;

                // Получить градиентную заливку
                GradientFill gradientFill = shape.Fill.GradientFill;
                if (gradientFill == null)
                {
                    Console.WriteLine("Cannot set gradient: The shape's fill is not a GradientFill.");
                    return;
                }

                // Вызовите SetTwoColorGradient с реалистичными параметрами
                gradientFill.SetTwoColorGradient(
                    Color.Red,          // color1
                    Color.Blue,         // color2
                    GradientStyleType.DiagonalDown,  // style
                    1);                 // variant

                Console.WriteLine("SetTwoColorGradient method called successfully with parameters (Red, Blue, DiagonalDown, 1)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTwoColorGradient: {ex.Message}");
            }

            // Сохраните рабочую книгу, чтобы продемонстрировать эффект
            workbook.Save("SetTwoColorGradientDemo.xlsx");
        }
    }
}
```

### См. также

* enum [GradientStyleType](../../gradientstyletype/)
* class [GradientFill](../)
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

    public class GradientFillMethodSetTwoColorGradientWithColorDoubleColorDoubleGradient297116Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить фигуру для применения градиентной заливки
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            try
            {
                // Установить тип заливки как градиент
                shape.Fill.FillType = FillType.Gradient;

                // Получить градиентную заливку
                GradientFill gradientFill = shape.Fill.GradientFill;
                if (gradientFill == null)
                {
                    Console.WriteLine("Cannot set gradient: The shape's fill is not a GradientFill.");
                    return;
                }

                // Вызовите SetTwoColorGradient с реалистичными параметрами
                gradientFill.SetTwoColorGradient(
                    Color.Red,          // color1
                    0.5,                // transparency1 (50% transparent)
                    Color.Blue,         // color2
                    0.3,                // transparency2 (30% transparent)
                    GradientStyleType.Horizontal,  // style
                    2);                 // variant

                Console.WriteLine("SetTwoColorGradient method called successfully with parameters (Red, 0.5, Blue, 0.3, Horizontal, 2)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTwoColorGradient: {ex.Message}");
            }

            // Сохраните рабочую книгу, чтобы продемонстрировать эффект
            workbook.Save("SetTwoColorGradientWithTransparencyDemo.xlsx");
        }
    }
}
```

### См. также

* enum [GradientStyleType](../../gradientstyletype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


