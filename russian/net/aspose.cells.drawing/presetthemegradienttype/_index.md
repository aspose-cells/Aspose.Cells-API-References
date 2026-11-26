---
title: "Перечисление PresetThemeGradientType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Drawing.PresetThemeGradientType перечисление. Представляет предустановленный тип градиента темы"
type: docs
url: /ru/net/aspose.cells.drawing/presetthemegradienttype/
---
## PresetThemeGradientType enumeration

Представляет тип предустановленного градиента темы.

```csharp
public enum PresetThemeGradientType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| LightGradient | `0` | Светлый градиент |
| TopSpotlight | `1` | Верхний прожектор |
| MediumGradient | `2` | Средний градиент |
| BottomSpotlight | `3` | Нижний прожектор |
| RadialGradient | `4` | Радиальный градиент |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DrawingClassPresetThemeGradientTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Category 1");
            worksheet.Cells["A3"].PutValue("Category 2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B3", true);

            // Применить градиентную заливку к первой серии
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            series.Area.FillFormat.FillType = FillType.Gradient;
            series.Area.FillFormat.GradientFill.SetPresetThemeGradient(
                PresetThemeGradientType.RadialGradient, 
                ThemeColorType.Accent1);

            // Сохраните книгу
            workbook.Save("PresetThemeGradientDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


