---
title: "Перечисление FormatConditionValueType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.FormatConditionValueType. Тип значения условия"
type: docs
url: /ru/net/aspose.cells/formatconditionvaluetype/
---
## FormatConditionValueType enumeration

Тип значения условия.

```csharp
public enum FormatConditionValueType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Formula | `0` | Минимальное/среднее/максимальное значение градиента определяется формулой. |
| Max | `1` | Указывает, что максимальное значение в диапазоне будет использоваться как максимальное значение градиента. |
| Min | `2` | Указывает, что минимальное значение в диапазоне будет использоваться как минимальное значение градиента. |
| Number | `3` | Указывает, что минимальное/среднее/максимальное значение градиента задаётся постоянным числовым значением. |
| Percent | `4` | Значение указывает, что процент между минимальным и максимальным значениями в диапазоне будет использоваться как минимальное/среднее/максимальное значение градиента. |
| Percentile | `5` | Значение указывает, что процентильный ранг в диапазоне будет использоваться как минимальное/среднее/максимальное значение градиента. |
| AutomaticMax | `6` | Указывает, что автоматическое максимальное значение в диапазоне будет использоваться как автоматическое максимальное значение градиента. |
| AutomaticMin | `7` | Указывает, что автоматическое минимальное значение в диапазоне будет использоваться как автоматическое минимальное значение градиента. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFormatConditionValueTypeDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить условия форматирования
            int formatConditionsIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection formatConditions = sheet.ConditionalFormattings[formatConditionsIndex];
            int conditionIndex = formatConditions.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = formatConditions[conditionIndex];

            // Установить свойства набора значков
            condition.IconSet.Type = IconSetType.Boxes5;
            condition.IconSet.ShowValue = false;
            condition.IconSet.Reverse = true;

            // Установить значение ячейки и применить форматирование
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Boxes5 Icon Set Example");

            // Получить тип значения условия форматирования
            FormatConditionValueType valueType = condition.IconSet.Cfvos[0].Type;
            Console.WriteLine("First CFVO Type: " + valueType);

            // Отобразить значения из условий набора значков
            Console.WriteLine("\nIcon Set Threshold Values:");
            foreach (ConditionalFormattingValue cfvo in condition.IconSet.Cfvos)
            {
                Console.WriteLine($"Type: {cfvo.Type}, Value: {cfvo.Value}");
            }

            // Сохраните книгу
            workbook.Save("FormatConditionValueTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


