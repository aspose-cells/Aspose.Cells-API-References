---
title: "GradientFill.SetPresetThemeGradient"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GradientFill. Устанавливает предустановленную градиентную заливку темы"
type: docs
url: /ru/net/aspose.cells.drawing/gradientfill/setpresetthemegradient/
---
## GradientFill.SetPresetThemeGradient method

Устанавливает предустановленную тематическую градиентную заливку.

```csharp
public void SetPresetThemeGradient(PresetThemeGradientType gradientType, 
    ThemeColorType themeColorType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| gradientType | PresetThemeGradientType | Тип предустановленного градиента. |
| themeColorType | ThemeColorType | Тип цвета темы. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class GradientFillMethodSetPresetThemeGradientWithPresetThemeGradientTypeThemeCoDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Sample");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.SetChartDataRange("A1:A4", false);

            // Настройте заливку серии с градиентом
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            series.Area.FillFormat.FillType = Aspose.Cells.Drawing.FillType.Gradient;
            
            // Продемонстрируйте SetPresetThemeGradient с указанными параметрами
            series.Area.FillFormat.GradientFill.SetPresetThemeGradient(
                Aspose.Cells.Drawing.PresetThemeGradientType.RadialGradient, 
                Aspose.Cells.ThemeColorType.Accent1);

            // Сохраните книгу
            workbook.Save("GradientFillDemo.xlsx");
        }
    }
}
```

### См. также

* enum [PresetThemeGradientType](../../presetthemegradienttype/)
* enum [ThemeColorType](../../../aspose.cells/themecolortype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


