---
title: "NegativeBarFormat.Color"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство NegativeBarFormat. Получает или задает объект FormatColor, который можно использовать для указания цвета заливки отрицательных полос данных"
type: docs
url: /ru/net/aspose.cells/negativebarformat/color/
---
## NegativeBarFormat.Color property

Получает или задает объект FormatColor, который можно использовать для указания цвета заливки отрицательных полос данных.

```csharp
public Color Color { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class NegativeBarFormatPropertyColorDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            sheet.Cells["E3"].PutValue(-10);
            sheet.Cells["E4"].PutValue(20);
            sheet.Cells["F3"].PutValue(-30);
            sheet.Cells["F4"].PutValue(40);
            sheet.Cells["G3"].PutValue(-50);
            sheet.Cells["G4"].PutValue(60);

            // Создайте условное форматирование
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection conds = sheet.ConditionalFormattings[formatIndex];
            int idx = conds.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = conds[idx];

            // Настройте свойства полос данных
            cond.DataBar.Color = Color.Orange;
            cond.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            cond.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            cond.DataBar.ShowValue = false;

            // Настройте формат отрицательной полосы
            cond.DataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            cond.DataBar.NegativeBarFormat.Color = Color.White;
            cond.DataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            cond.DataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            // Сохраните книгу
            workbook.Save("NegativeBarFormatColorDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("NegativeBarFormatPropertyColorDemo executed successfully.");
        }
    }
}
```

### См. также

* class [NegativeBarFormat](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


