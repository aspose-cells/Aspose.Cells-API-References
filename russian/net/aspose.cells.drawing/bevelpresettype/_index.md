---
title: "Перечисление BevelPresetType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.BevelPresetType. Представляет предустановку типа фаски, которую можно применить к фигуре в 3D"
type: docs
url: /ru/net/aspose.cells.drawing/bevelpresettype/
---
## BevelPresetType enumeration

Представляет предустановку типа фаски, которую можно применить к фигуре в 3D.

```csharp
public enum BevelPresetType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Без фаски |
| Angle | `1` | Угол |
| ArtDeco | `2` | Арт-деко |
| Circle | `3` | Круг |
| Convex | `4` | Выпуклый |
| CoolSlant | `5` | Крутой наклон |
| Cross | `6` | Крест |
| Divot | `7` | Вмятина |
| HardEdge | `8` | Жёсткий край |
| RelaxedInset | `9` | Смягчённый отступ |
| Riblet | `10` | Ребристый |
| Slope | `11` | Наклон |
| SoftRound | `12` | Мягко округленный |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Charts;
    using System;

    public class BevelPresetTypeDemo
    {
        public static void BevelPresetTypeExample()
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

            // Получить доступ к заголовку диаграммы и установить его текст
            chart.Title.Text = "Sample Chart with Bevel";

            // Получить доступ к области построения диаграммы
            PlotArea plotArea = chart.PlotArea;

            // Получить доступ к свойствам фигур области построения
            ShapePropertyCollection shapeProperties = plotArea.ShapeProperties;

            
            // Получить доступ к свойствам 3D-формата
            Format3D format3D = shapeProperties.Format3D;

            // Получить доступ к свойствам верхней фаски
            Bevel topBevel = format3D.TopBevel;

            // Установить тип фаски в "Angle"
            topBevel.Type = BevelPresetType.Angle;

            // Установить ширину и высоту фаски
            topBevel.Width = 10;
            topBevel.Height = 10;

            // Сохраните книгу
            workbook.Save("BevelPresetTypeExample.xlsx");
            workbook.Save("BevelPresetTypeExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


