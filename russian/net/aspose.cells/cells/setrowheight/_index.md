---
title: "Cells.SetRowHeight"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Устанавливает высоту указанной строки"
type: docs
url: /ru/net/aspose.cells/cells/setrowheight/
---
## Cells.SetRowHeight method

Устанавливает высоту указанной строки.

```csharp
public void SetRowHeight(int row, double height)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки. |
| высота | Double | Высота строки. В единицах точек. Должна быть между 0 и 409,5. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetRowHeightWithInt32DoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установите высоту строки для первой строки (индекс 0) в 25,5 пункта
            cells.SetRowHeight(0, 25.5);

            // Проверьте высоту строки
            Console.WriteLine("Row height of row 0: " + cells.GetRowHeight(0));
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


