---
title: "Worksheet.GetPanes"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Worksheet. Получает области окна"
type: docs
url: /ru/net/aspose.cells/worksheet/getpanes/
---
## Worksheet.GetPanes method

Получает области окна.

```csharp
public PaneCollection GetPanes()
```

### Примечания

Если окно не разделено и не зафиксировано.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodGetPanesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Зафиксировать области в строке 5 и столбце 3
            worksheet.FreezePanes(5, 3, 5, 3);
            
            // Получить информацию об области
            PaneCollection panes = worksheet.GetPanes();
            
            // Отобразить информацию об области
            Console.WriteLine("First visible row of bottom pane: " + panes.FirstVisibleRowOfBottomPane);
            Console.WriteLine("First visible column of right pane: " + panes.FirstVisibleColumnOfRightPane);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [PaneCollection](../../panecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


