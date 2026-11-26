---
title: "Top10.IsPercent"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Top10. Получить или задать, является ли правило top/bottom n правилом top/bottom n percent. Значение по умолчанию — false"
type: docs
url: /ru/net/aspose.cells/top10/ispercent/
---
## Top10.IsPercent property

Получить или установить, является ли правило "top/bottom n" правилом "top/bottom n percent". Значение по умолчанию — false.

```csharp
public bool IsPercent { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class Top10PropertyIsPercentDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i + 1);
            }

            // Добавьте правило условного форматирования Top10
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.Top10, OperatorType.None, null, null);

            // Получить условие форматирования Top10
            FormatCondition fc = fcc[0];
            
            // Установить свойства Top10
            fc.Top10.IsPercent = true;  // Demonstrate IsPercent property
            fc.Top10.IsBottom = false;
            fc.Top10.Rank = 3;

            // Применить стиль форматирования
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            fc.Style = style;

            // Сохраните книгу
            workbook.Save("Top10IsPercentDemo.xlsx");
        }
    }
}
```

### См. также

* class [Top10](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


