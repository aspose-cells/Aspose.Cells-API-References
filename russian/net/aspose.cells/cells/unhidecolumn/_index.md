---
title: "Cells.UnhideColumn"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Делает столбец видимым"
type: docs
url: /ru/net/aspose.cells/cells/unhidecolumn/
---
## Cells.UnhideColumn method

Отображает скрытый столбец

```csharp
public void UnhideColumn(int column, double width)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| column | Int32 | Индекс столбца. |
| ширина | Double | Ширина столбца. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUnhideColumnWithInt32DoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Скрыть столбец 2
            cells.HideColumn(2);
            
            // Показать столбец 2 с корректировкой ширины (-1 означает использование стандартной ширины)
            cells.UnhideColumn(2, -1);
            
            Console.WriteLine("Column 2 width after unhiding: " + cells.Columns[2].Width);
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


