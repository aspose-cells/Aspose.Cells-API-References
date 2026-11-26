---
title: "ColorScale.MidCfvo"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ColorScale. Получает или задает объект среднего значения этой шкалы цветов. Нельзя установить CFValueObject с типом FormatConditionValueType.Max или FormatConditionValueType.Min"
type: docs
url: /ru/net/aspose.cells/colorscale/midcfvo/
---
## ColorScale.MidCfvo property

Получить или установить объект среднего значения этого ColorScale. Нельзя установить CFValueObject с типом FormatConditionValueType.Max или FormatConditionValueType.Min.

```csharp
public ConditionalFormattingValue MidCfvo { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColorScalePropertyMidCfvoDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            for (int i = 0; i < 10; i++)
            {
                sheet.Cells[i, 0].PutValue(i * 10);
            }

            // Добавить условное форматирование цветовой шкалы
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[index];
            int conditionIndex = fcc.AddCondition(FormatConditionType.ColorScale);
            
            // Установить значение средней точки для цветовой шкалы
            ColorScale colorScale = fcc[conditionIndex].ColorScale;
            colorScale.MidCfvo.Type = FormatConditionValueType.Number;
            colorScale.MidCfvo.Value = 50;

            // Сохраните книгу
            workbook.Save("ColorScalePropertyMidCfvoDemo.xlsx");
        }
    }
}
```

### См. также

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


