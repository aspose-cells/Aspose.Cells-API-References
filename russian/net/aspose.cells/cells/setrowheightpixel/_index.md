---
title: "Cells.SetRowHeightPixel"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Устанавливает высоту строки в пикселях"
type: docs
url: /ru/net/aspose.cells/cells/setrowheightpixel/
---
## Cells.SetRowHeightPixel method

Устанавливает высоту строки в пикселях.

```csharp
public void SetRowHeightPixel(int row, int pixels)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки. |
| пиксели | Int32 | Количество пикселей. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetRowHeightPixelWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установить высоту первой строки в 50 пикселей
            worksheet.Cells.SetRowHeightPixel(0, 50);

            // Установить высоту второй строки в 100 пикселей
            worksheet.Cells.SetRowHeightPixel(1, 100);

            // Сохраните книгу
            workbook.Save("RowHeightPixelDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


