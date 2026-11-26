---
title: "ShapePath.ShapePath"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор ShapePath. Инициализирует новый экземпляр класса ShapePath"
type: docs
url: /ru/net/aspose.cells.drawing/shapepath/shapepath/
---
## ShapePath constructor

Инициализирует новый экземпляр класса [`ShapePath`](../).

```csharp
public ShapePath()
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodCtorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Создайте новый путь фигуры, используя метод #ctor
                ShapePath shapePath = new ShapePath();

                // Добавьте сегменты пути, чтобы создать простую фигуру
                shapePath.MoveTo(100, 100);
                shapePath.LineTo(200, 100);
                shapePath.LineTo(200, 200);
                shapePath.LineTo(100, 200);
                shapePath.Close();

                //добавить свободную форму
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 200, 200, new ShapePath[] { shapePath });

                Console.WriteLine("ShapePath created and added to worksheet successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ShapePath constructor: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("ShapePathMethodCtorDemo.xlsx");
        }
    }
}
```

### См. также

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


