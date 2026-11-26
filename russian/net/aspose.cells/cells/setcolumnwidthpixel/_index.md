---
title: "Cells.SetColumnWidthPixel"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Устанавливает ширину столбца в пикселях в обычном виде"
type: docs
url: /ru/net/aspose.cells/cells/setcolumnwidthpixel/
---
## Cells.SetColumnWidthPixel method

Устанавливает ширину столбца в пикселях в обычном виде.

```csharp
public void SetColumnWidthPixel(int column, int pixels)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| column | Int32 | Индекс столбца. |
| пиксели | Int32 | Количество пикселей. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetColumnWidthPixelWithInt32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установите ширину столбцов в пикселях для столбцов с 1 по 5
            for (int i = 0; i < 5; i++)
            {
                cells.SetColumnWidthPixel(i, 120); // 120 pixels width
            }

            // Сохраните книгу
            workbook.Save("SetColumnWidthPixelDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


