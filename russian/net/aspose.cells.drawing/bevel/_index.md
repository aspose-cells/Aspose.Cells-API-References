---
title: "Класс Bevel"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Drawing.Bevel класс. Представляет фаску фигуры"
type: docs
url: /ru/net/aspose.cells.drawing/bevel/
---
## Bevel class

Представляет фаску формы

```csharp
public class Bevel
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Height](../../aspose.cells.drawing/bevel/height/) { get; set; } | Получает и задает высоту фаски, или насколько она расположена над фигурой. В единицах точек. |
| [Type](../../aspose.cells.drawing/bevel/type/) { get; set; } | Получает и задает тип предустановленной фаски. |
| [Width](../../aspose.cells.drawing/bevel/width/) { get; set; } | Получает и задает ширину фаски, или насколько она проникает в фигуру. В единицах точек. |

### Примеры

```csharp
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;

namespace AsposeCellsExamples
{
    public class BevelDemo
    {
        public static void RunDemo()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            workbook.CalculateFormula();

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Добавьте серию данных в диаграмму
            chart.NSeries.Add("A1:B4", true);

            // Получить доступ к области построения диаграммы
            ChartFrame plotArea = chart.PlotArea;

            // Получить доступ к свойствам фигур области построения
            ShapePropertyCollection shapeProperties = plotArea.ShapeProperties;

            // Получить доступ к свойствам 3D-формата
            Format3D format3D = shapeProperties.Format3D;

            // Получить доступ к свойствам верхней фаски
            Bevel topBevel = format3D.TopBevel;

            // Установите ширину, высоту и тип фаски
            topBevel.Width = 10.0;
            topBevel.Height = 5.0;
            topBevel.Type = BevelPresetType.Circle;

            // Установите другие свойства 3D-формата
            format3D.SurfaceMaterialType = PresetMaterialType.WarmMatte;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;
            format3D.LightingAngle = 45.0;

            // Сохраните книгу
            workbook.Save("BevelDemo.xlsx");
            workbook.Save("BevelDemo.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


