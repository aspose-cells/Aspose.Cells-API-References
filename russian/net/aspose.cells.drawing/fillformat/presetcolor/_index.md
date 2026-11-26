---
title: "FillFormat.PresetColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FillFormat. Возвращает предустановленный градиентный цвет для указанного заполнения"
type: docs
url: /ru/net/aspose.cells.drawing/fillformat/presetcolor/
---
## FillFormat.PresetColor property

Возвращает предустановленный цвет градиента для указанного заполнения.

```csharp
public GradientPresetType PresetColor { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyPresetColorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Получить доступ к формату заполнения области диаграммы
            FillFormat fillFormat = chart.ChartArea.Area.FillFormat;

            // Установить предустановленный градиентный цвет
            fillFormat.SetPresetColorGradient(GradientPresetType.Ocean, GradientStyleType.DiagonalUp, 2);

            // Отобразить и проверить предустановленный цвет
            Console.WriteLine("Preset Color: " + fillFormat.PresetColor);

            // Сохраните книгу
            workbook.Save("FillFormatPresetColorDemo.xlsx");
        }
    }
}
```

### См. также

* enum [GradientPresetType](../../gradientpresettype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


