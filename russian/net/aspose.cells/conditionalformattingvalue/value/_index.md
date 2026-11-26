---
title: "ConditionalFormattingValue.Value"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ConditionalFormattingValue. Получить или установить значение этого объекта условного форматирования. Его следует использовать вместе с Type."
type: docs
url: /ru/net/aspose.cells/conditionalformattingvalue/value/
---
## ConditionalFormattingValue.Value property

Получить или установить значение этого объекта значения условного форматирования. Его следует использовать вместе с Type.

```csharp
public object Value { get; set; }
```

### Примечания

Если значение является строкой и начинается с \"=\", оно будет обработано как формула, иначе мы обработаем его как простое значение.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingValuePropertyValueDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Добавить условное форматирование
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            
            // Создать условное форматирование набора значков
            int conditionIndex = fcc.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = fcc[conditionIndex];
            condition.IconSet.Type = IconSetType.Arrows3;

            // Получить объекты значений условного форматирования
            ConditionalFormattingValueCollection cfvos = condition.IconSet.Cfvos;

            // Установить значения для значков
            cfvos[0].Type = FormatConditionValueType.Min;
            cfvos[0].Value = 0;
            
            cfvos[1].Type = FormatConditionValueType.Percent;
            cfvos[1].Value = 33;
            
            cfvos[2].Type = FormatConditionValueType.Percent;
            cfvos[2].Value = 67;

            // Продемонстрировать использование свойства Value
            Console.WriteLine("First icon value: " + cfvos[0].Value);
            Console.WriteLine("Second icon value: " + cfvos[1].Value);
            Console.WriteLine("Third icon value: " + cfvos[2].Value);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [ConditionalFormattingValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


