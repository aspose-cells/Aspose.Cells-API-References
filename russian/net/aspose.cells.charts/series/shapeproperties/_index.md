---
title: "Series.ShapeProperties"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Series. Получает объект ShapePropertyCollection, который содержит визуальные свойства формы Series."
type: docs
url: /ru/net/aspose.cells.charts/series/shapeproperties/
---
## Series.ShapeProperties property

Получает объект [`ShapePropertyCollection`](../../../aspose.cells.drawing/shapepropertycollection/), который содержит визуальные свойства формы Series.

```csharp
public ShapePropertyCollection ShapeProperties { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SeriesPropertyShapePropertiesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавить диаграмму
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Установите данные диаграммы
            chart.NSeries.Add("Sheet1!B2:B4", true);
            chart.NSeries.CategoryData = "Sheet1!A2:A4";

            // Получить первую серию и её свойства формы
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            ShapePropertyCollection shapeProperties = series.ShapeProperties;

            // Настройте 3D‑формат и фаску
            Format3D format3D = shapeProperties.Format3D;
            Bevel topBevel = format3D.TopBevel;
            topBevel.Type = BevelPresetType.Circle;
            topBevel.Height = 2;
            topBevel.Width = 5;

            // Настроить материал и освещение
            format3D.SurfaceMaterialType = PresetMaterialType.WarmMatte;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;
            format3D.LightingAngle = 20;

            // Задайте цвета серии
            series.Area.BackgroundColor = Color.Blue;
            series.Area.ForegroundColor = Color.Blue;
            series.Border.Color = Color.Blue;

            // Сохраните книгу
            workbook.Save("SeriesShapePropertiesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [ShapePropertyCollection](../../../aspose.cells.drawing/shapepropertycollection/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


