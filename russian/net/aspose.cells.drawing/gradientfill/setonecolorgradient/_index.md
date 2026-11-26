---
title: "GradientFill.SetOneColorGradient"
second_title: "Справочник API Aspose.Cells для .NET"
description: "GradientFill method. Устанавливает указанную заливку в градиент из одного цвета. Применяется только для Excel 2007"
type: docs
url: /ru/net/aspose.cells.drawing/gradientfill/setonecolorgradient/
---
## GradientFill.SetOneColorGradient method

Устанавливает указанное заполнение в одноцветный градиент. Применяется только для Excel 2007.

```csharp
public void SetOneColorGradient(Color color, double degree, GradientStyleType style, int variant)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| цвет | Color | Один цвет градиента. |
| степень | Double | Степень градиента. Может принимать значение от 0.0 (тёмный) до 1.0 (светлый). |
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

    public class GradientFillMethodSetOneColorGradientWithColorDoubleGradientStyleTyInt32Demo
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

                // Вызвать SetOneColorGradient с реалистичными параметрами
                gradientFill.SetOneColorGradient(
                    Color.Green,        // color
                    0.7,                // degree (70% intensity)
                    GradientStyleType.DiagonalUp,  // style
                    1);                 // variant

                Console.WriteLine("SetOneColorGradient method called successfully with parameters (Green, 0.7, DiagonalUp, 1)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetOneColorGradient: {ex.Message}");
            }

            // Сохраните рабочую книгу, чтобы продемонстрировать эффект
            workbook.Save("SetOneColorGradientDemo.xlsx");
        }
    }
}
```

### См. также

* enum [GradientStyleType](../../gradientstyletype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


