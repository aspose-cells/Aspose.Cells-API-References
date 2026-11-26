---
title: "GradientStopCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GradientStopCollection. Добавить градиентную остановку"
type: docs
url: /ru/net/aspose.cells.drawing/gradientstopcollection/add/
---
## Add(double, CellsColor, int) {#add}

Добавить градиентную остановку.

```csharp
public void Add(double position, CellsColor color, int alpha)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| позиция | Double | Позиция остановки в процентах. |
| цвет | CellsColor | Цвет остановки. |
| альфа | Int32 | Альфа цвета. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientStopCollectionMethodAddWithDoubleCellsColorInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 2, 0, 2, 0, 300, 100);
            shape.Fill.FillType = FillType.Gradient;
            
            GradientStopCollection gradientStops = shape.Fill.GradientFill.GradientStops;
            gradientStops.Clear();

            try
            {
                // Создать CellsColor с помощью фабричного метода
                CellsColor gradientColor = workbook.CreateCellsColor();
                gradientColor.Color = Color.DarkOrange;

                gradientStops.Add(0.3, gradientColor, 192);

                Console.WriteLine("Gradient stop added successfully");
                workbook.Save("GradientStopAddDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding gradient stop: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [GradientStopCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(double, Color, int) {#add_1}

Добавить градиентную остановку.

```csharp
public void Add(double position, Color color, int alpha)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| позиция | Double | Позиция остановки в процентах. |
| цвет | Color | Цвет остановки. |
| альфа | Int32 | Альфа цвета. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientStopCollectionMethodAddWithDoubleColorInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать прямоугольную форму с градиентной заливкой
            var shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 2, 0, 2, 0, 300, 100);
            shape.Fill.FillType = FillType.Gradient;
            shape.Fill.GradientFill.GradientStops.Clear();

            GradientStopCollection gradientStops = shape.Fill.GradientFill.GradientStops;

            try
            {
                // Добавить градиентные остановки, используя параметры (Double, Color, Int32)
                gradientStops.Add(0.0, Color.Red, 255);    // Opaque red at start position
                gradientStops.Add(1.0, Color.Blue, 128);    // Semi-transparent blue at end position

                Console.WriteLine("Added gradient stops with positions: 0.0 (Red) and 1.0 (Blue)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding gradient stops: {ex.Message}");
            }

            workbook.Save("GradientStopCollectionAddDemo.xlsx");
        }
    }
}
```

### См. также

* class [GradientStopCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


