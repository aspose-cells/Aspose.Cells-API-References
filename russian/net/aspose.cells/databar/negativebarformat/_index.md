---
title: "DataBar.NegativeBarFormat"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataBar. Получает объект NegativeBarFormat, связанный с правилом условного форматирования гистограммы"
type: docs
url: /ru/net/aspose.cells/databar/negativebarformat/
---
## DataBar.NegativeBarFormat property

Получает объект NegativeBarFormat, связанный с правилом условного форматирования data bar.

```csharp
public NegativeBarFormat NegativeBarFormat { get; }
```

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarPropertyNegativeBarFormatDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить примерные данные с отрицательными значениями
            sheet.Cells["E3"].PutValue(-10);
            sheet.Cells["E4"].PutValue(20);
            sheet.Cells["F3"].PutValue(-30);
            sheet.Cells["F4"].PutValue(40);
            sheet.Cells["G3"].PutValue(-50);
            sheet.Cells["G4"].PutValue(60);

            // Добавить условное форматирование полос данных
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection conditions = sheet.ConditionalFormattings[formatIndex];
            int index = conditions.AddCondition(FormatConditionType.DataBar);
            FormatCondition condition = conditions[index];

            // Установить свойства полосы данных
            condition.DataBar.Color = Color.Orange;
            condition.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            condition.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            condition.DataBar.ShowValue = false;

            // Установить свойства границы
            condition.DataBar.BarBorder.Type = DataBarBorderType.Solid;
            condition.DataBar.BarBorder.Color = Color.Plum;

            // Установить тип заливки
            condition.DataBar.BarFillType = DataBarFillType.Gradient;

            // Установить свойства оси
            condition.DataBar.AxisColor = Color.Red;
            condition.DataBar.AxisPosition = DataBarAxisPosition.Automatic;

            // Настроить формат отрицательной полосы
            condition.DataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            condition.DataBar.NegativeBarFormat.Color = Color.White;
            condition.DataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            condition.DataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            // Сохраните книгу
            workbook.Save("DataBarNegativeFormatDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [NegativeBarFormat](../../negativebarformat/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


