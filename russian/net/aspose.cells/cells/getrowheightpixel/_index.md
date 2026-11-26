---
title: "Cells.GetRowHeightPixel"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Получает высоту указанной строки в пикселях"
type: docs
url: /ru/net/aspose.cells/cells/getrowheightpixel/
---
## Cells.GetRowHeightPixel method

Получает высоту указанной строки в пикселях.

```csharp
public int GetRowHeightPixel(int row)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки |

### Возвращаемое значение

Высота строки

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetRowHeightPixelWithInt32Demo
    {
        public static void Run()
        {
            // Создайте новый Workbook
            Workbook wb = new Workbook();

            // Получить первый лист
            Worksheet worksheet = wb.Worksheets[0];

            // Установить высоту строки для строки 5 (в пикселях)
            worksheet.Cells.SetRowHeightPixel(5, 30);

            // Получить высоту строки для строки 5 (в пикселях)
            int rowHeight = worksheet.Cells.GetRowHeightPixel(5);

            Console.WriteLine("Row height of row 5 in pixels: " + rowHeight);
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


