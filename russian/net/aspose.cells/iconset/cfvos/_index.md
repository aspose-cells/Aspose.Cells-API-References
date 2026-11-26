---
title: "IconSet.Cfvos"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство IconSet. Получить экземпляр CFValueObjects"
type: docs
url: /ru/net/aspose.cells/iconset/cfvos/
---
## IconSet.Cfvos property

Получить экземпляр CFValueObjects.

```csharp
public ConditionalFormattingValueCollection Cfvos { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IconSetPropertyCfvosDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i * 10);
            }

            try
            {
                // Добавить условное форматирование
                int cfIndex = worksheet.ConditionalFormattings.Add();
                FormatConditionCollection fcs = worksheet.ConditionalFormattings[cfIndex];

                // Установить диапазон для условного форматирования
                CellArea area = new CellArea();
                area.StartRow = 0;
                area.StartColumn = 0;
                area.EndRow = 9;
                area.EndColumn = 0;
                fcs.AddArea(area);

                // Добавить условие набора значков
                int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
                FormatCondition condition = fcs[conditionIndex];

                // Установить тип набора значков
                condition.IconSet.Type = IconSetType.TrafficLights31;

                // Получить доступ к свойству Cfvos (только для чтения)
                ConditionalFormattingValueCollection cfvos = condition.IconSet.Cfvos;

                // Отобразить информацию о коллекции Cfvos
                Console.WriteLine("Number of CFValueObjects in the collection: " + cfvos.Count);

                // Перебрать коллекцию и отобразить каждое значение
                for (int i = 0; i < cfvos.Count; i++)
                {
                    ConditionalFormattingValue cfValue = cfvos[i];
                    Console.WriteLine($"CFValue {i + 1}: Type = {cfValue.Type}, Value = {cfValue.Value}");
                }

                // Сохраните книгу
                workbook.Save("IconSetCfvosDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with icon set conditional formatting.");
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

* class [ConditionalFormattingValueCollection](../../conditionalformattingvaluecollection/)
* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


