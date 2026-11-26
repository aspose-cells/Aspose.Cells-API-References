---
title: "Перечисление OperatorType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.OperatorType. Представляет тип оператора условного форматирования и проверки данных"
type: docs
url: /ru/net/aspose.cells/operatortype/
---
## OperatorType enumeration

Представляет тип оператора условного форматирования и проверки данных.

```csharp
public enum OperatorType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Between | `0` | Представляет оператор Between условного форматирования и проверки данных. |
| Equal | `1` | Представляет оператор Equal условного форматирования и проверки данных. |
| GreaterThan | `2` | Представляет оператор GreaterThan условного форматирования и проверки данных. |
| GreaterOrEqual | `3` | Представляет оператор GreaterOrEqual условного форматирования и проверки данных. |
| LessThan | `4` | Представляет оператор LessThan условного форматирования и проверки данных. |
| LessOrEqual | `5` | Представляет оператор LessOrEqual условного форматирования и проверки данных. |
| None | `6` | Представляет отсутствие сравнения. |
| NotBetween | `7` | Представляет оператор NotBetween условного форматирования и проверки данных. |
| NotEqual | `8` | Представляет оператор NotEqual условного форматирования и проверки данных. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OperatorTypeDemo
    {
        public static void OperatorTypeExample()
        {
            // Создайте новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить пустое условное форматирование
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Установить диапазон условного форматирования
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Добавить условие с OperatorType.Between
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A1", "100");
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.Yellow;

            // Добавить другое условие с OperatorType.GreaterThan
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "50", null);
            FormatCondition fc2 = fcs[conditionIndex2];
            fc2.Style.BackgroundColor = System.Drawing.Color.Green;

            // Сохраните книгу
            workbook.Save("OperatorTypeExample.xlsx");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


