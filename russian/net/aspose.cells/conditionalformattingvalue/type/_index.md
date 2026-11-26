---
title: "ConditionalFormattingValue.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ConditionalFormattingValue. Получить или установить тип этого объекта условного форматирования. Установка типа в FormatConditionValueType.Min или FormatConditionValueType.Max автоматически задаст Value как null."
type: docs
url: /ru/net/aspose.cells/conditionalformattingvalue/type/
---
## ConditionalFormattingValue.Type property

Получить или установить тип этого объекта значения условного форматирования. Установка типа в FormatConditionValueType.Min или FormatConditionValueType.Max автоматически установит "Value" в null.

```csharp
public FormatConditionValueType Type { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingValuePropertyTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Создать новую книгу
                Workbook workbook = new Workbook();
                Worksheet ws = workbook.Worksheets[0];

                // Добавьте некоторые примерные данные (необходимо для существования условного форматирования)
                ws.Cells["A1"].PutValue(10);
                ws.Cells["A2"].PutValue(20);
                ws.Cells["A3"].PutValue(30);

                // Создайте коллекцию условного форматирования и добавьте условие IconSet
                int cfIndex = ws.ConditionalFormattings.Add();
                FormatConditionCollection fcc = ws.ConditionalFormattings[cfIndex];

                int condIdx = fcc.AddCondition(FormatConditionType.IconSet);
                FormatCondition condition = fcc[condIdx];
                condition.IconSet.Type = IconSetType.Arrows3; // any valid icon set type

                // Получите экземпляр ConditionalFormattingValue из коллекции IconSet
                ConditionalFormattingValue cfv = condition.IconSet.Cfvos[0];

                // Установите Type в Percent и задайте соответствующее значение
                cfv.Type = FormatConditionValueType.Percent;
                cfv.Value = 25; // 25%

                // Прочитайте и отобразите Type и Value
                Console.WriteLine("After setting Type to Percent:");
                Console.WriteLine("  Type : " + cfv.Type);
                Console.WriteLine("  Value: " + cfv.Value);

                // Измените Type на Min — согласно документации это обнулит Value
                cfv.Type = FormatConditionValueType.Min;

                // Снова прочитайте и отобразите Type и Value
                Console.WriteLine("\nAfter setting Type to Min:");
                Console.WriteLine("  Type : " + cfv.Type);
                Console.WriteLine("  Value: " + (cfv.Value == null ? "null" : cfv.Value.ToString()));

                // Сохраните книгу (условное форматирование является частью листа)
                workbook.Save("ConditionalFormattingValueTypeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* enum [FormatConditionValueType](../../formatconditionvaluetype/)
* class [ConditionalFormattingValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


