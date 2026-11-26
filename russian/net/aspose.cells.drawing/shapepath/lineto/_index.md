---
title: "ShapePath.LineTo"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapePath. Добавляет линейный сегмент к текущей фигуре. Начальная точка является конечной точкой текущей фигуры. Unit Pixel"
type: docs
url: /ru/net/aspose.cells.drawing/shapepath/lineto/
---
## ShapePath.LineTo method

Добавляет отрезок линии к текущей фигуре. Начальная точка является конечной точкой текущей фигуры. Единица измерения: пиксель.

```csharp
public void LineTo(float x, float y)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| x | Single | Координата x конечной точки линейного сегмента (Unit: Pixel). |
| y | Single | Координата y конечной точки линейного сегмента (Unit: Pixel). |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodLineToWithSingleSingleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                //Создать новый путь формы
                ShapePath shapePath = new ShapePath();

                // Перейти к начальной точке
                shapePath.MoveTo(10, 10);
                
                // Вызвать метод LineTo с параметрами (Single, Single)
                shapePath.LineTo(50.5f, 10.5f);
                shapePath.LineTo(50.5f, 50.5f);
                shapePath.LineTo(10.5f, 50.5f);
                shapePath.Close();

                //добавить свободную форму
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath });

                Console.WriteLine("LineTo method executed successfully with parameters (Single, Single)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing LineTo method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("ShapePathMethodLineToWithSingleSingleDemo.xlsx");
        }
    }
}
```

### См. также

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


