---
title: "Cells.HideColumn"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Скрывает столбец"
type: docs
url: /ru/net/aspose.cells/cells/hidecolumn/
---
## Cells.HideColumn method

Скрывает столбец.

```csharp
public void HideColumn(int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| column | Int32 | Индекс столбца. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodHideColumnWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установите некоторые данные в столбец, который будем скрывать
            cells["B1"].PutValue("This column will be hidden");
            cells["B2"].PutValue(123.45);

            // Скройте столбец B (индекс 1)
            cells.HideColumn(1);

            // Отобразите столбец со стандартной шириной
            cells.UnhideColumn(1, cells.StandardWidth);

            // Сохраните книгу
            workbook.Save("HideColumnDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


