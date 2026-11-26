---
title: "Перечисление PresetMaterialType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Drawing.PresetMaterialType enum. Описывает внешний вид поверхности фигуры"
type: docs
url: /ru/net/aspose.cells.drawing/presetmaterialtype/
---
## PresetMaterialType enumeration

Описывает внешний вид поверхности фигуры.

```csharp
public enum PresetMaterialType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Clear | `0` | Прозрачный |
| DarkEdge | `1` | Темный край |
| Flat | `2` | Плоский |
| LegacyMatte | `3` | Устаревший матовый |
| LegacyMetal | `4` | Устаревший металл |
| LegacyPlastic | `5` | Устаревший пластик |
| LegacyWireframe | `6` | Устаревший каркас |
| Matte | `7` | Матовый |
| Metal | `8` | Металлический |
| Plastic | `9` | Пластиковый |
| Powder | `10` | Порошок |
| SoftEdge | `11` | Мягкий край |
| SoftMetal | `12` | Мягкий металл |
| TranslucentPowder | `13` | Полупрозрачный порошок |
| WarmMatte | `14` | Теплый матовый |

### Примеры

```csharp
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;

namespace AsposeCellsExamples
{
    public class PresetMaterialTypeDemo
    {
        public static void PresetMaterialTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных диаграммы
            chart.SetChartDataRange("A1:B4", true);

            // Получить доступ к первой серии на диаграмме
            Series series = chart.NSeries[0];

            // Получить доступ к 3D-формату серии
            Format3D format3D = series.ShapeProperties.Format3D;

            // Установить тип материала поверхности
            format3D.SurfaceMaterialType = PresetMaterialType.Metal;

            // Установить другие 3D‑свойства
            format3D.LightingAngle = 45;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;

            // Сохраните книгу
            workbook.Save("PresetMaterialTypeExample.xlsx");

            // Выведите результаты
            Console.WriteLine("Chart with 3D format and PresetMaterialType applied has been created.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


