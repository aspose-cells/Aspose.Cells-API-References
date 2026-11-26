---
title: "Cells.SetColumnWidthInch"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Устанавливает ширину столбца в единицах дюймов в обычном представлении"
type: docs
url: /ru/net/aspose.cells/cells/setcolumnwidthinch/
---
## Cells.SetColumnWidthInch method

Устанавливает ширину столбца в дюймах в обычном виде.

```csharp
public void SetColumnWidthInch(int column, double inches)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| column | Int32 | Индекс столбца. |
| дюймы | Double | Количество дюймов. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetColumnWidthInchWithInt32DoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установите ширину столбцов в дюймах
            cells.SetColumnWidthInch(0, 2.0);
            cells.SetColumnWidthInch(1, 1.5);
            cells.SetColumnWidthInch(2, 0.8);

            // Установите некоторые данные в ячейки, чтобы файл стал видимым
            cells["A1"].PutValue("Column A (2 inches)");
            cells["B1"].PutValue("Column B (1.5 inches)");
            cells["C1"].PutValue("Column C (0.8 inches)");

            // Сохраните книгу
            workbook.Save("ColumnWidthsInInches.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


