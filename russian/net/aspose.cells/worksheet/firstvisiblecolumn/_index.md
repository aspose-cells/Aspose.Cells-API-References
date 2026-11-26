---
title: "Worksheet.FirstVisibleColumn"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Представляет индекс первой видимой колонки"
type: docs
url: /ru/net/aspose.cells/worksheet/firstvisiblecolumn/
---
## Worksheet.FirstVisibleColumn property

Представляет индекс первой видимой колонки.

```csharp
public int FirstVisibleColumn { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyFirstVisibleColumnDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Скрыть первую колонку (индекс 0)
            worksheet.Cells.HideColumn(0);
            
            // Получить и отобразить индекс первого видимого столбца
            Console.WriteLine("First visible column index: " + worksheet.FirstVisibleColumn);
            
            // Сохраните книгу
            workbook.Save("FirstVisibleColumnDemo.xlsx");
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


