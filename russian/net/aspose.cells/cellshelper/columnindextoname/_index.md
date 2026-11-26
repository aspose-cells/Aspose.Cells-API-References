---
title: "CellsHelper.ColumnIndexToName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CellsHelper. Получает имя столбца по его индексу"
type: docs
url: /ru/net/aspose.cells/cellshelper/columnindextoname/
---
## CellsHelper.ColumnIndexToName method

Получает имя столбца в соответствии с индексом столбца.

```csharp
public static string ColumnIndexToName(int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| column | Int32 | Индекс столбца. |

### Возвращаемое значение

Имя столбца.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodColumnIndexToNameWithInt32Demo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установите значения в ячейках для демонстрации преобразования индекса столбца в имя
            worksheet.Cells["A1"].PutValue("Column Index");
            worksheet.Cells["B1"].PutValue("Column Name");

            // Продемонстрировать ColumnIndexToName для индексов 0-4
            for (int i = 0; i < 5; i++)
            {
                worksheet.Cells[i + 1, 0].PutValue(i);
                string columnName = CellsHelper.ColumnIndexToName(i);
                worksheet.Cells[i + 1, 1].PutValue(columnName);
            }

            // Сохраните книгу
            workbook.Save("ColumnIndexToNameDemo.xlsx");
        }
    }
}
```

### См. также

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


