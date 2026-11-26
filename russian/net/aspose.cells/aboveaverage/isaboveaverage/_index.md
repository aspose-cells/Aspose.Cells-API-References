---
title: "AboveAverage.IsAboveAverage"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство AboveAverage. Получает или задает флаг, указывающий, является ли правило правилом выше среднего. true означает выше среднего. Значение по умолчанию — true."
type: docs
url: /ru/net/aspose.cells/aboveaverage/isaboveaverage/
---
## AboveAverage.IsAboveAverage property

Получить или задать флаг, указывающий, является ли правило правилом "above average". Значение 'true' означает "above average". Значение по умолчанию — true.

```csharp
public bool IsAboveAverage { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AboveAveragePropertyIsAboveAverageDemo
    {
        public static void Run()
        {
            // Создайте новую книгу
            Workbook workbook = new Workbook();
            
            // Получить первый лист
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для демонстрации условного форматирования
            for (int i = 0; i <= 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i * 10);
            }

            // Добавить условное форматирование
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Установить диапазон условного форматирования
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            // Добавить условие AboveAverage
            int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Yellow;

            // Настроить свойства AboveAverage
            fc.AboveAverage.IsAboveAverage = true;  // Highlight values above average
            fc.AboveAverage.IsEqualAverage = false; // Exclude values equal to average

            // Сохраните файл Excel
            workbook.Save("AboveAverageConditionDemo.xlsx");
        }
    }
}
```

### См. также

* class [AboveAverage](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


