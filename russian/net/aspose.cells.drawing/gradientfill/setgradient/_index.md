---
title: "GradientFill.SetGradient"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GradientFill. Устанавливает тип градиентной заливки и направление"
type: docs
url: /ru/net/aspose.cells.drawing/gradientfill/setgradient/
---
## GradientFill.SetGradient method

Установите тип градиентной заливки и направление.

```csharp
public void SetGradient(GradientFillType type, double angle, GradientDirectionType direction)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| type | GradientFillType | Тип градиентной заливки. |
| angle | Double | Угол. Применяется только для GradientFillType.Linear. |
| direction | GradientDirectionType | Тип направления. Применяется только для GradientFillType.Radial и GradientFillType.Rectangle. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class GradientFillMethodSetGradientWithGradientFillTypeDoubleGradientDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить фигуру для применения градиентной заливки
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 200, 100);

            try
            {
                // Получить градиент заливки фигуры
                GradientFill gradientFill = shape.Fill.GradientFill; // Fixed property name from Gradient to GradientFill
                if (gradientFill == null)
                {
                    Console.WriteLine("Cannot set gradient: The shape's fill is not a GradientFill.");
                    return;
                }

                // Вызовите SetGradient с конкретными параметрами: линейная заливка, 90 градусов, направление FromCenter
                gradientFill.SetGradient(GradientFillType.Linear, 90.0, GradientDirectionType.FromCenter);
                
                Console.WriteLine("SetGradient method executed successfully with parameters (GradientFillType.Linear, 90.0, GradientDirectionType.FromCenter)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetGradient method: {ex.Message}");
            }
            
            // Сохраните рабочую книгу, чтобы продемонстрировать эффект
            workbook.Save("GradientFillSetGradientDemo.xlsx");
        }
    }
}
```

### См. также

* enum [GradientFillType](../../gradientfilltype/)
* enum [GradientDirectionType](../../gradientdirectiontype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


