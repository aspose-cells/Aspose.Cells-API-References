---
title: "ShapePath.MoveTo"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapePath. Начинает новую фигуру из указанной точки без закрытия текущей фигуры. Все последующие точки, добавляемые в путь, добавляются в эту новую фигуру. Unit Pixel"
type: docs
url: /ru/net/aspose.cells.drawing/shapepath/moveto/
---
## ShapePath.MoveTo method

Начинает новую фигуру из указанной точки без закрытия текущей фигуры. Все последующие точки, добавляемые в путь, добавляются к этой новой фигуре. Единица измерения: пиксель.

```csharp
public void MoveTo(float x, float y)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| x | Single | Координата X начальной точки фигуры (Unit: Pixel). |
| y | Single | Координата Y начальной точки фигуры (Unit: Pixel). |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodMoveToWithSingleSingleDemo
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

                Console.WriteLine("MoveTo method executed successfully with parameters (Single, Single)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing LineTo method: {ex.Message}");
            }
           
            
            // Сохранить результат
            workbook.Save("ShapePathMethodMoveToWithSingleSingleDemo.xlsx");
        }
    }
}
```

### См. также

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


