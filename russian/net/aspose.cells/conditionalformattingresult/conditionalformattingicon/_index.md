---
title: "ConditionalFormattingResult.ConditionalFormattingIcon"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ConditionalFormattingResult. Возвращает изображение набора значков"
type: docs
url: /ru/net/aspose.cells/conditionalformattingresult/conditionalformattingicon/
---
## ConditionalFormattingResult.ConditionalFormattingIcon property

Получает изображение набора значков.

```csharp
public ConditionalFormattingIcon ConditionalFormattingIcon { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingResultPropertyConditionalFormattingIconDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные и условное форматирование
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Добавить условное форматирование набора значков
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 2;
            area.EndColumn = 0;
            fcc.AddArea(area);

            int conditionIndex = fcc.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = fcc[conditionIndex];
            condition.IconSet.Type = IconSetType.TrafficLights31;

            // Вычислите формулы и получите результат условного форматирования
            workbook.CalculateFormula();
            ConditionalFormattingResult result = worksheet.Cells["A1"].GetConditionalFormattingResult();

            // Продемонстрируйте свойство ConditionalFormattingIcon
            if (result != null && result.ConditionalFormattingIcon != null)
            {
                Console.WriteLine("Icon Type: " + result.ConditionalFormattingIcon.Type);
                Console.WriteLine("Icon Index: " + result.ConditionalFormattingIcon.Index);
            }
        }
    }
}
```

### См. также

* class [ConditionalFormattingIcon](../../conditionalformattingicon/)
* class [ConditionalFormattingResult](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


