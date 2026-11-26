---
title: "Перечисление LightRigType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.LightRigType. Представляет предустановленный свет, который можно применить к форме"
type: docs
url: /ru/net/aspose.cells.drawing/lightrigtype/
---
## LightRigType enumeration

Представляет предустановленный правый свет, который можно применить к фигуре.

```csharp
public enum LightRigType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Balanced | `0` | Сбалансированный |
| BrightRoom | `1` | Светлая комната |
| Chilly | `2` | Прохладно |
| Contrasting | `3` | Контрастный |
| Flat | `4` | Плоский |
| Flood | `5` | Наводнение |
| Freezing | `6` | Морозно |
| Glow | `7` | Сияние |
| Harsh | `8` | Суровый |
| LegacyFlat1 | `9` | LegacyFlat1 |
| LegacyFlat2 | `10` | LegacyFlat2 |
| LegacyFlat3 | `11` | LegacyFlat3 |
| LegacyFlat4 | `12` | LegacyFlat4 |
| LegacyHarsh1 | `13` | LegacyHarsh1 |
| LegacyHarsh2 | `14` | LegacyHarsh2 |
| LegacyHarsh3 | `15` | LegacyHarsh3 |
| LegacyHarsh4 | `16` | LegacyHarsh4 |
| LegacyNormal1 | `17` | LegacyNormal1 |
| LegacyNormal2 | `18` | LegacyNormal2 |
| LegacyNormal3 | `19` | LegacyNormal3 |
| LegacyNormal4 | `20` | LegacyNormal4 |
| Morning | `21` | Утро |
| Soft | `22` | Мягкий |
| Sunrise | `23` | Рассвет |
| Sunset | `24` | Закат |
| ThreePoint | `25` | Три точки |
| TwoPoint | `26` | Две точки |
| None | `27` | Нет световой установки. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class LightRigTypeDemo
    {
        public static void LightRigTypeExample()
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных диаграммы
            chart.SetChartDataRange("A1:B4", true);

            // Получить доступ к первой серии на диаграмме
            Series series = chart.NSeries[0];

            // Получите доступ к свойствам формы серии
            ShapePropertyCollection shapeProperties = series.ShapeProperties;

            // Проверьте, есть ли у серии данные 3D-формата
            if (shapeProperties.HasFormat3D())
            {
                // Получить доступ к свойствам 3D-формата
                Format3D format3D = shapeProperties.Format3D;

                // Установите тип освещения поверхности в Balanced
                format3D.SurfaceLightingType = LightRigType.Balanced;

                // Установите угол освещения
                format3D.LightingAngle = 45.0;
            }

            // Сохраните книгу
            workbook.Save("LightRigTypeExample.xlsx");
            workbook.Save("LightRigTypeExample.pdf");
            // Выведите результаты
            Console.WriteLine("LightRigType example applied and workbook saved as 'LightRigTypeExample.xlsx'.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


