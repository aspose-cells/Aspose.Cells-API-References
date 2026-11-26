---
title: "Класс ShapePropertyCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Drawing.ShapePropertyCollection. Этот класс определяет визуальные свойства формы для элемента диаграммы или формы"
type: docs
url: /ru/net/aspose.cells.drawing/shapepropertycollection/
---
## ShapePropertyCollection class

Этот класс задает визуальные свойства формы для элемента диаграммы или фигуры.

```csharp
public class ShapePropertyCollection
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Format3D](../../aspose.cells.drawing/shapepropertycollection/format3d/) { get; } | Представляет объект [`Format3D`](./format3d/), который задает 3D‑свойства формы для элемента диаграммы или формы. |
| [GlowEffect](../../aspose.cells.drawing/shapepropertycollection/gloweffect/) { get; } | Представляет объект [`GlowEffect`](./gloweffect/), который задает эффект свечения для элемента диаграммы или формы. |
| [ShadowEffect](../../aspose.cells.drawing/shapepropertycollection/shadoweffect/) { get; } | Представляет объект [`ShadowEffect`](./shadoweffect/), который задает эффект тени для элемента диаграммы или формы. |
| [SoftEdgeRadius](../../aspose.cells.drawing/shapepropertycollection/softedgeradius/) { get; set; } | Получает и задает радиус размытия, применяемый к краям, в единицах точек. |

## Методы

| Имя | Описание |
| --- | --- |
| [ClearFormat3D](../../aspose.cells.drawing/shapepropertycollection/clearformat3d/)() | Очищает 3D‑свойства формы. |
| [ClearGlowEffect](../../aspose.cells.drawing/shapepropertycollection/cleargloweffect/)() | Очищает эффект свечения формы. |
| [ClearShadowEffect](../../aspose.cells.drawing/shapepropertycollection/clearshadoweffect/)() | Очищает эффект тени элемента диаграммы или формы. |
| [HasFormat3D](../../aspose.cells.drawing/shapepropertycollection/hasformat3d/)() | Указывает, содержит ли форма данные 3D‑формата. |
| [HasGlowEffect](../../aspose.cells.drawing/shapepropertycollection/hasgloweffect/)() | Указывает, содержит ли форма данные эффекта свечения. |
| [HasShadowEffect](../../aspose.cells.drawing/shapepropertycollection/hasshadoweffect/)() | Указывает, содержит ли форма данные эффекта тени. |

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassShapePropertyCollectionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте пример диаграммы
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            
            chart.NSeries.Add("B1:B2", true);
            chart.NSeries.CategoryData = "A1:A2";

            // Получите доступ к свойствам формы первой серии
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            ShapePropertyCollection shapeProperties = series.ShapeProperties;

            // Настройте 3D‑формат и фаску
            Format3D format3D = shapeProperties.Format3D;
            Bevel topBevel = format3D.TopBevel;
            
            topBevel.Type = BevelPresetType.Circle;
            topBevel.Height = 2;
            topBevel.Width = 5;
            
            format3D.SurfaceMaterialType = PresetMaterialType.WarmMatte;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;
            format3D.LightingAngle = 20;

            // Задайте цвета серии
            series.Area.BackgroundColor = Color.Blue;
            series.Area.ForegroundColor = Color.Blue;
            series.Border.Color = Color.Blue;

            // Сохраните книгу
            workbook.Save("ShapePropertyCollectionDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


