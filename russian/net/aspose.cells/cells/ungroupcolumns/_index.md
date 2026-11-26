---
title: "Cells.UngroupColumns"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Разгруппирует столбцы"
type: docs
url: /ru/net/aspose.cells/cells/ungroupcolumns/
---
## Cells.UngroupColumns method

Разгруппирует столбцы.

```csharp
public void UngroupColumns(int firstIndex, int lastIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| firstIndex | Int32 | Первый индекс столбца для разгруппировки. |
| lastIndex | Int32 | Последний индекс столбца для разгруппировки. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUngroupColumnsWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Сначала сгруппируйте столбцы, чтобы продемонстрировать разгруппировку
            worksheet.Cells.GroupColumns(0, 2);

            // Разгруппировать столбцы (0 до 2)
            worksheet.Cells.UngroupColumns(0, 2);

            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


