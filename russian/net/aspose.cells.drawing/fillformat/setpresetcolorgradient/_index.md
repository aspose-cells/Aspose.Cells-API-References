---
title: "FillFormat.SetPresetColorGradient"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод FillFormat. Устанавливает указанную заливку в градиент предустановленного цвета. Применяется только для Excel 2007"
type: docs
url: /ru/net/aspose.cells.drawing/fillformat/setpresetcolorgradient/
---
## FillFormat.SetPresetColorGradient method

Устанавливает указанное заполнение в градиент с предустановленным цветом. Применяется только для Excel 2007.

```csharp
public void SetPresetColorGradient(GradientPresetType presetColor, GradientStyleType style, 
    int variant)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| presetColor | GradientPresetType | Тип предустановленного цвета |
| стиль | GradientStyleType | Стиль затенения градиента. |
| variant | Int32 | Вариант градиента. Может принимать значение от 1 до 4, соответствующее одному из четырёх вариантов на вкладке Gradient в диалоговом окне Fill Effects. Если стиль равен GradientStyle.FromCenter, аргумент Variant может быть только 1 или 2. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatMethodSetPresetColorGradientWithGradientPresetTypeGradientStylDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 5; i++)
            {
                sheet.Cells[$"A{i}"].PutValue($"Item {i-1}");
                sheet.Cells[$"B{i}"].PutValue(i * 10);
            }

            // Создать диаграмму
            int chartIndex = sheet.Charts.Add(ChartType.Column, 8, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Применить градиентную заливку
            FillFormat fillFormat = chart.PlotArea.Area.FillFormat;
            fillFormat.SetPresetColorGradient(GradientPresetType.Daybreak, GradientStyleType.Vertical, 1);

            // Сохраните книгу
            workbook.Save("SetPresetColorGradientDemo.xlsx");
        }
    }
}
```

### См. также

* enum [GradientPresetType](../../gradientpresettype/)
* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


