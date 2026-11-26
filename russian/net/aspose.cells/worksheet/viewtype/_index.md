---
title: "Worksheet.ViewType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Получает и задает тип представления"
type: docs
url: /ru/net/aspose.cells/worksheet/viewtype/
---
## Worksheet.ViewType property

Получает и задает тип представления.

```csharp
public ViewType ViewType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyViewTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите тип представления в PageLayoutView и включите линейку
            worksheet.ViewType = ViewType.PageLayoutView;
            worksheet.IsRulerVisible = true;
            
            // Добавьте примерный контент для демонстрации представления
            worksheet.Cells["A1"].PutValue("Page Layout View Demo");
            worksheet.Cells["A2"].PutValue("Ruler is visible in this view");
            
            // Сохраните книгу
            workbook.Save("WorksheetViewTypeDemo.xlsx");
            
            Console.WriteLine("Worksheet ViewType demo completed successfully.");
        }
    }
}
```

### См. также

* enum [ViewType](../../viewtype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


