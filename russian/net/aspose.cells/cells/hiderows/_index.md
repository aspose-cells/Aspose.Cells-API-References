---
title: "Cells.HideRows"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Скрывает несколько строк"
type: docs
url: /ru/net/aspose.cells/cells/hiderows/
---
## Cells.HideRows method

Скрывает несколько строк.

```csharp
public void HideRows(int row, int totalRows)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки. |
| totalRows | Int32 | Номер строки. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodHideRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполните некоторыми данными
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].Value = $"Row {i+1}, Col {j+1}";
                }
            }

            // Скрыть строки 3‑5 (индекс с нуля: 2‑4)
            worksheet.Cells.HideRows(2, 3);

            // Сохраните книгу
            workbook.Save("HideRowsExample.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


