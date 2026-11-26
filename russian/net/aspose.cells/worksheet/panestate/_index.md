---
title: "Worksheet.PaneState"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Указывает, имеет ли панель горизонтальные или вертикальные разрывы и заморожены ли эти разрывы"
type: docs
url: /ru/net/aspose.cells/worksheet/panestate/
---
## Worksheet.PaneState property

Указывает, имеет ли панель горизонтальное или вертикальное разделение, и заморожены ли эти разделения.

```csharp
public PaneStateType PaneState { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyPaneStateDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установить примерные данные
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");

            // Заморозить панели (первая строка)
            worksheet.FreezePanes(1, 0, 1, 0);

            // Получить и отобразить состояние панели
            PaneStateType paneState = worksheet.PaneState;
            Console.WriteLine("Pane State: " + paneState);

            // Сохранить книгу
            workbook.Save("PaneStateDemo.xlsx");
        }
    }
}
```

### См. также

* enum [PaneStateType](../../panestatetype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


