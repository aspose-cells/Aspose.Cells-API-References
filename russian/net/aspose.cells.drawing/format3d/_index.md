---
title: "Класс Format3D"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Drawing.Format3D класс. Этот класс задает свойства 3D‑формы для элемента диаграммы или фигуры"
type: docs
url: /ru/net/aspose.cells.drawing/format3d/
---
## Format3D class

Этот класс задает свойства 3D-формы для элемента диаграммы или формы.

```csharp
public class Format3D
```

## Свойства

| Имя | Описание |
| --- | --- |
| [LightingAngle](../../aspose.cells.drawing/format3d/lightingangle/) { get; set; } | Получает и задает угол освещения. Диапазон от 0 до 359,9 градусов. |
| [SurfaceLightingType](../../aspose.cells.drawing/format3d/surfacelightingtype/) { get; set; } | Получает и задает тип освещения, который применяется к сцене фигуры. Значение по умолчанию — LightRigType.ThreePoint. |
| [SurfaceMaterialType](../../aspose.cells.drawing/format3d/surfacematerialtype/) { get; set; } | Получает и задает тип материала, который комбинируется со свойствами освещения, чтобы придать фигуре окончательный вид и ощущение. Значение по умолчанию — PresetMaterialType.WarmMatte. |
| [TopBevel](../../aspose.cells.drawing/format3d/topbevel/) { get; } | Получает объект [`Bevel`](../bevel/), который содержит свойства, связанные с определением фаски на верхней или передней грани фигуры. |

## Методы

| Имя | Описание |
| --- | --- |
| [HasTopBevelData](../../aspose.cells.drawing/format3d/hastopbeveldata/)() | Указывает, содержит ли фигура данные о верхней фаске. |

### Примеры

```csharp
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;

namespace AsposeCellsExamples
{
    public class Format3DDemo
    {
        public static void RunDemo()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);
            sheet.Cells["A4"].PutValue(40);

            // Добавить диаграмму в лист
            int chartIndex = sheet.Charts.Add(ChartType.Column3DClustered, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Добавить серию к диаграмме
            chart.NSeries.Add("A1:A4", true);

            // Получить доступ к первой серии
            Series series = chart.NSeries[0];

            // Получить доступ к 3D-формату серии
            Format3D format3D = series.ShapeProperties.Format3D;

            // Установите свойства 3D‑формата
            format3D.SurfaceMaterialType = PresetMaterialType.WarmMatte;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;
            format3D.LightingAngle = 45.0;

            // Проверьте, содержит ли фигура данные о верхней фаске
            if (format3D.HasTopBevelData())
            {
                Bevel topBevel = format3D.TopBevel;
                Console.WriteLine("Top Bevel Width: " + topBevel.Width);
                Console.WriteLine("Top Bevel Height: " + topBevel.Height);
            }

            // Сохраните книгу
            workbook.Save("Format3DDemo.xlsx");
            workbook.Save("Format3DDemo.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


