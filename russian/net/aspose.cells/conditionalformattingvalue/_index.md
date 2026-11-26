---
title: "Класс ConditionalFormattingValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.ConditionalFormattingValue. Описывает значения точек интерполяции в градиентной шкале dataBar или iconSet"
type: docs
url: /ru/net/aspose.cells/conditionalformattingvalue/
---
## ConditionalFormattingValue class

Описывает значения точек интерполяции в градиентной шкале, dataBar или iconSet.

```csharp
public class ConditionalFormattingValue
```

## Свойства

| Имя | Описание |
| --- | --- |
| [IsGTE](../../aspose.cells/conditionalformattingvalue/isgte/) { get; set; } | Получить или установить флаг Greater Than Or Equal. Используется только для наборов значков, определяет, использует ли это пороговое значение оператор «больше или равно». Значение 'false' указывает, что используется «больше», а не «больше или равно». Значение по умолчанию — true. |
| [Type](../../aspose.cells/conditionalformattingvalue/type/) { get; set; } | Получить или установить тип этого объекта значения условного форматирования. Установка типа в FormatConditionValueType.Min или FormatConditionValueType.Max автоматически установит "Value" в null. |
| [Value](../../aspose.cells/conditionalformattingvalue/value/) { get; set; } | Получить или установить значение этого объекта значения условного форматирования. Его следует использовать вместе с Type. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ConditionalFormattingValueDemo
    {
        public static void ConditionalFormattingValueExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавляет пустое условное форматирование
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Устанавливает диапазон условного форматирования
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Добавляет условие
            int conditionIndex = fcs.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcs[conditionIndex];

            // Установка свойств для ColorScale
            fc.ColorScale.Is3ColorScale = true;

            // Установка минимального значения
            fc.ColorScale.MinCfvo.Type = FormatConditionValueType.Min;
            fc.ColorScale.MinCfvo.Value = null;
            fc.ColorScale.MinColor = Color.Blue;

            // Установка среднего значения
            fc.ColorScale.MidCfvo.Type = FormatConditionValueType.Percentile;
            fc.ColorScale.MidCfvo.Value = 50;
            fc.ColorScale.MidColor = Color.Yellow;

            // Установка максимального значения
            fc.ColorScale.MaxCfvo.Type = FormatConditionValueType.Max;
            fc.ColorScale.MaxCfvo.Value = null;
            fc.ColorScale.MaxColor = Color.Red;

            // Сохраните книгу
            workbook.Save("ConditionalFormattingValueExample.xlsx");
            workbook.Save("ConditionalFormattingValueExample.pdf");
            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


