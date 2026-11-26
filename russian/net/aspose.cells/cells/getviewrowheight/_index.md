---
title: "Cells.GetViewRowHeight"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Получает высоту указанной строки"
type: docs
url: /ru/net/aspose.cells/cells/getviewrowheight/
---
## Cells.GetViewRowHeight method

Получает высоту указанной строки.

```csharp
public double GetViewRowHeight(int row)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки. |

### Возвращаемое значение

Высота строки.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetViewRowHeightWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите высоту строки для строки 3 (в пунктах)
            worksheet.Cells.SetRowHeight(3, 15);
            
            // Получите высоту отображаемой строки для строки 3
            double viewRowHeight = worksheet.Cells.GetViewRowHeight(3);
            
            // Вывести результат.
            Console.WriteLine("View Row Height for row 3: " + viewRowHeight);
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


