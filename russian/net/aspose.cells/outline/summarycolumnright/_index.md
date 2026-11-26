---
title: "Outline.SummaryColumnRight"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Outline. Указывает, будет ли столбец итога расположен справа от столбцов деталей в структуре"
type: docs
url: /ru/net/aspose.cells/outline/summarycolumnright/
---
## Outline.SummaryColumnRight property

Указывает, будет ли столбец итогов размещён справа от столбцов деталей в outline.

```csharp
public bool SummaryColumnRight { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OutlinePropertySummaryColumnRightDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные и сгруппировать строки
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Item " + (i + 1));
                worksheet.Cells["B" + (i + 1)].PutValue(i * 10);
            }

            // Группировать строки (создаёт структуру)
            worksheet.Cells.GroupRows(0, 9, false);

            // Получить настройки структуры
            Outline outline = worksheet.Outline;

            // Установить SummaryColumnRight в true (столбцы итога будут отображаться справа от столбцов деталей)
            outline.SummaryColumnRight = true;
            Console.WriteLine("SummaryColumnRight is set to: " + outline.SummaryColumnRight);

            // Сохраните книгу
            workbook.Save("OutlinePropertySummaryColumnRightDemo.xlsx");
        }
    }
}
```

### См. также

* class [Outline](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


