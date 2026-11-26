---
title: "Worksheet.IsGridlinesVisible"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Получает или задаёт значение, указывающее, видимы ли линии сетки. По умолчанию true"
type: docs
url: /ru/net/aspose.cells/worksheet/isgridlinesvisible/
---
## Worksheet.IsGridlinesVisible property

Получает или задаёт значение, указывающее, видимы ли линии сетки. По умолчанию true.

```csharp
public bool IsGridlinesVisible { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsGridlinesVisibleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите видимость линий сетки в true
            worksheet.IsGridlinesVisible = true;
            
            // Добавьте некоторые примерные данные, чтобы увидеть линии сетки
            worksheet.Cells["A1"].PutValue("Gridlines Visible Example");
            worksheet.Cells["A2"].PutValue("This worksheet shows gridlines");
            
            // Автоматически подгонять столбцы для лучшей видимости
            worksheet.AutoFitColumns();
            
            // Сохраните книгу
            workbook.Save("GridlinesVisibleDemo.xlsx");
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


