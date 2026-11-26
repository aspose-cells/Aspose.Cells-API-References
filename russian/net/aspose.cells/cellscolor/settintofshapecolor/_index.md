---
title: "CellsColor.SetTintOfShapeColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CellsColor. Установить оттенок цвета фигуры"
type: docs
url: /ru/net/aspose.cells/cellscolor/settintofshapecolor/
---
## CellsColor.SetTintOfShapeColor method

Установить оттенок цвета фигуры

```csharp
public void SetTintOfShapeColor(double tint)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| оттенок | Double |  |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class CellsColorMethodSetTintOfShapeColorWithDoubleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму на лист
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            try
            {
                // Получить цвет заливки фигуры
                CellsColor shapeColor = shape.Fill.SolidFill.CellsColor;
                
                // Установить цвет, который будет рассматриваться как цвет фигуры
                shapeColor.IsShapeColor = true;
                
                // Установить оттенок цвета фигуры (допустимый диапазон от -1.0 до 1.0)
                shapeColor.SetTintOfShapeColor(0.5); // Lighten the color by 50%
                
                Console.WriteLine("SetTintOfShapeColor method executed successfully with parameter 0.5");
                
                // Отобразить эффект, изменив цвет заливки фигуры
                shape.Fill.SolidFill.Color = System.Drawing.Color.Blue;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTintOfShapeColor method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("SetTintOfShapeColorWithDoubleDemo.xlsx");
        }
    }
}
```

### См. также

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


