---
title: "Worksheet.Outline"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Получает структуру на этом листе"
type: docs
url: /ru/net/aspose.cells/worksheet/outline/
---
## Worksheet.Outline property

Получает контур этого листа.

```csharp
public Outline Outline { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyOutlineDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные и создайте группы структуры
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[$"A{i + 1}"].Value = $"Item {i + 1}";
                worksheet.Cells[$"B{i + 1}"].Value = (i + 1) * 100;
            }

            // Группировать строки (создаёт структуру)
            worksheet.Cells.GroupRows(0, 9, false);

            // Доступ к свойствам структуры
            Outline outline = worksheet.Outline;
            Console.WriteLine($"Outline summary row is below detail: {outline.SummaryRowBelow}");
            Console.WriteLine($"Outline summary column is to right: {outline.SummaryColumnRight}");

            // Изменить настройки структуры
            outline.SummaryRowBelow = true;
            outline.SummaryColumnRight = false;

            // Разгруппировать строки, чтобы продемонстрировать работу структуры
            worksheet.Cells.UngroupRows(0, 9);

            // Сохраните книгу
            workbook.Save("WorksheetOutlineDemo.xlsx");
        }
    }
}
```

### См. также

* class [Outline](../../outline/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


