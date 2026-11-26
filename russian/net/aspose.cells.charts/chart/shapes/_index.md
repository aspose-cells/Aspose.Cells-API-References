---
title: "Chart.Shapes"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Chart. Возвращает все графические фигуры в этой диаграмме"
type: docs
url: /ru/net/aspose.cells.charts/chart/shapes/
---
## Chart.Shapes property

Возвращает все графические фигуры в этой диаграмме.

```csharp
public ShapeCollection Shapes { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPropertyShapesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Добавьте фигуру в диаграмму
            Aspose.Cells.Drawing.Shape shape = chart.Shapes.AddShape(MsoDrawingType.TextBox, 1000, 1000, 2000, 1000, 0, 0);
            shape.Text = "Sample Shape";
            
            // Измените свойства фигур
            shape.LeftInShape = 4000 - shape.WidthInShape;
            shape.TopInShape = 4000 - shape.HeightInShape;
            
            // Сохраните книгу
            workbook.Save("ChartPropertyShapesDemo_out.xlsx");
        }
    }
}
```

### См. также

* class [ShapeCollection](../../../aspose.cells.drawing/shapecollection/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


