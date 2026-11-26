---
title: "ConditionalFormattingValueCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ConditionalFormattingValueCollection. Получить элемент CFValueObject по указанному индексу"
type: docs
url: /ru/net/aspose.cells/conditionalformattingvaluecollection/item/
---
## ConditionalFormattingValueCollection indexer

Получите элемент CFValueObject по указанному индексу.

```csharp
public ConditionalFormattingValue this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс элемента, начиная с нуля. |

### Возвращаемое значение

Элемент по указанному индексу.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingValueCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Добавьте примерные данные
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["A2"].PutValue(120);
                worksheet.Cells["A3"].PutValue(260);

                // Добавить условное форматирование
                int cfIndex = worksheet.ConditionalFormattings.Add();
                FormatConditionCollection fcs = worksheet.ConditionalFormattings[cfIndex];

                // Установить диапазон для условного форматирования
                CellArea ca = new CellArea
                {
                    StartRow = 0,
                    EndRow = 2,
                    StartColumn = 0,
                    EndColumn = 0
                };
                fcs.AddArea(ca);

                // Добавить условие набора значков
                int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
                FormatCondition condition = fcs[conditionIndex];
                IconSet iconSet = condition.IconSet;
                iconSet.Type = IconSetType.Arrows3;

                // Получить ConditionalFormattingValueCollection
                ConditionalFormattingValueCollection cfvos = iconSet.Cfvos;

                // Добавить значение в коллекцию
                int valueIndex = cfvos.Add(FormatConditionValueType.Number, "50");

                // Продемонстрировать доступ к свойству Item (индексатор)
                ConditionalFormattingValue cfv = cfvos[valueIndex];

                // Отобразить значение из свойства Item
                Console.WriteLine($"Conditional Formatting Value at index {valueIndex}:");
                Console.WriteLine($"  Type: {cfv.Type}");
                Console.WriteLine($"  Value: {cfv.Value}");
                Console.WriteLine($"  IsGTE: {cfv.IsGTE}");

                // Сохраните книгу
                workbook.Save("ConditionalFormattingValueCollectionItemDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [ConditionalFormattingValueCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


