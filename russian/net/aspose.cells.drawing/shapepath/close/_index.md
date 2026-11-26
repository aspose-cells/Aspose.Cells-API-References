---
title: "ShapePath.Close"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapePath. Закрывает текущую фигуру и начинает новую фигуру. Если текущая фигура содержит последовательность соединённых линий и кривых, метод замыкает контур, соединяя линией конечную точку с начальной точкой."
type: docs
url: /ru/net/aspose.cells.drawing/shapepath/close/
---
## ShapePath.Close method

Закрывает текущую фигуру и начинает новую фигуру. Если текущая фигура содержит последовательность соединённых линий и кривых, метод замыкает контур, соединяя линией конечную точку с начальной.

```csharp
public void Close()
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodCloseDemo
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
                shapePath.MoveTo(60, 45);
                shapePath.ArcTo(25, 25, 0, 270);

                // Закройте путь 
                shapePath.Close();

                shapePath.MoveTo(60, 20);
                shapePath.LineTo(110, 70);
                shapePath.LineTo(125, 155.5f);
                shapePath.ArcTo(35.5f, 35.5f, 0, 270);

                // Закройте путь 
                shapePath.Close();

                //добавить свободную форму
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath });

                Console.WriteLine("Close method called successfully to complete the shape path");
                
                // Сохраните книгу
                workbook.Save("ShapePathMethodCloseDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling Close method: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


