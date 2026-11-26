---
title: "ThreeDFormat.ContourColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ThreeDFormat. Получает и задает цвет контура фигуры"
type: docs
url: /ru/net/aspose.cells.drawing/threedformat/contourcolor/
---
## ThreeDFormat.ContourColor property

Получает и задает цвет контура фигуры.

```csharp
public CellsColor ContourColor { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyContourColorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте фигуру для демонстрации 3D-форматирования
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 1, 200, 100, 0, 0);
            shape.Text = "3D ContourColor Demo";
            
            // Получите ThreeDFormat фигуры
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Настройте базовые 3D‑свойства
            threeDFormat.TopBevelType = BevelType.ArtDeco;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;
            threeDFormat.ContourWidth = 2;

            try
            {
                // Получите текущее значение ContourColor
                CellsColor contourColor = threeDFormat.ContourColor;
                Console.WriteLine($"Initial ContourColor - Type: {contourColor.Type}, ARGB: {contourColor.Argb}");

                // Создайте новый цвет, изменив существующий
                contourColor.Argb = System.Drawing.Color.Red.ToArgb();
                contourColor.Transparency = 0.5;
                threeDFormat.ContourColor = contourColor;

                // Отобразите новое значение ContourColor
                Console.WriteLine($"New ContourColor - Type: {threeDFormat.ContourColor.Type}, ARGB: {threeDFormat.ContourColor.Argb}");

                // Сохраните книгу, чтобы увидеть эффекты
                workbook.Save("ThreeDFormatContourColorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


