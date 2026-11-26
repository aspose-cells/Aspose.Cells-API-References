---
title: "ShapeCollection.AddLabelInChart"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapeCollection. Добавляет метку на диаграмму"
type: docs
url: /ru/net/aspose.cells.drawing/shapecollection/addlabelinchart/
---
## ShapeCollection.AddLabelInChart method

Добавляет метку на диаграмму.

```csharp
public Label AddLabelInChart(int top, int left, int height, int width)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| верх | Int32 | Представляет вертикальное смещение метки от верхнего левого угла в единицах 1/4000 области диаграммы. |
| влево | Int32 | Представляет вертикальное смещение метки от верхнего левого угла в единицах 1/4000 области диаграммы. |
| высота | Int32 | Представляет высоту метки, в единицах 1/4000 области диаграммы. |
| ширина | Int32 | Представляет ширину метки, в единицах 1/4000 области диаграммы. |

### Возвращаемое значение

Новый объект Label.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeCollectionMethodAddLabelInChartWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для создания диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];            
            chart.SetChartDataRange("A1:B4", true);

            try
            {
                // Вызовите метод AddLabelInChart с параметрами (top, left, height, width)
                Label label = chart.Shapes.AddLabelInChart(100, 100, 200, 200);
                
                // Установите свойства метки
                label.Text = "Sample Chart Label";
                label.Font.Color = System.Drawing.Color.Red;
                label.Font.Size = 12;

                Console.WriteLine("Label added successfully to chart with parameters (100, 100, 200, 50)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddLabelInChart method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("ShapeCollectionMethodAddLabelInChartWithInt32Int32Int32Int32Demo.xlsx");
        }
    }
}
```

### См. также

* class [Label](../../label/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


