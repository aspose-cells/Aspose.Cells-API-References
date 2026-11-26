---
title: "ShapeCollection.AddAutoShapeInChart"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapeCollection. Добавляет AutoShape в диаграмму"
type: docs
url: /ru/net/aspose.cells.drawing/shapecollection/addautoshapeinchart/
---
## ShapeCollection.AddAutoShapeInChart method

Добавляет AutoShape на диаграмму.

```csharp
public Shape AddAutoShapeInChart(AutoShapeType type, int top, int left, int height, int width)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| type | AutoShapeType | Тип автоформы. |
| верх | Int32 | Представляет вертикальное смещение текстового поля от верхнего левого угла в единицах 1/4000 области диаграммы. |
| влево | Int32 | Представляет вертикальное смещение текстового поля от верхнего левого угла в единицах 1/4000 области диаграммы. |
| высота | Int32 | Представляет высоту текстового поля в единицах 1/4000 области диаграммы. |
| ширина | Int32 | Представляет ширину текстового поля в единицах 1/4000 области диаграммы. |

### Возвращаемое значение

Возвращает объект формы.

### Примечания

Тип не может быть Chart/Comment/Picture/OleObject/Polygon/DialogBox

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeCollectionMethodAddAutoShapeInChartWithAutoShapeTypeInt32Int32Int32InDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            try
            {
                // Вызовите метод AddAutoShapeInChart, чтобы добавить звёздную форму в диаграмму
                Shape shape = chart.Shapes.AddAutoShapeInChart(
                    AutoShapeType.Star16,  // AutoShapeType
                    100,                  // Top position (in pixels)
                    100,                  // Left position (in pixels)
                    200,                  // Height (in pixels)
                    200);                 // Width (in pixels)

                // Установите свойства формы
                shape.Name = "SampleStar";
                shape.Fill.SolidFill.Color = System.Drawing.Color.Yellow;
                shape.Line.SolidFill.Color = System.Drawing.Color.Red;

                Console.WriteLine("Star shape added successfully to the chart.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddAutoShapeInChart method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("ShapeCollectionMethodAddAutoShapeInChartDemo.xlsx");
        }
    }
}
```

### См. также

* class [Shape](../../shape/)
* enum [AutoShapeType](../../autoshapetype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


