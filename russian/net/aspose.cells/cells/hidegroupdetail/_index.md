---
title: "Cells.HideGroupDetail"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Сворачивает сгруппированные строки/столбцы"
type: docs
url: /ru/net/aspose.cells/cells/hidegroupdetail/
---
## Cells.HideGroupDetail method

Сворачивает сгруппированные строки/столбцы.

```csharp
public void HideGroupDetail(bool isVertical, int index)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| isVertical | Boolean | True, свернуть сгруппированные строки. |
| индекс | Int32 | Индекс строки/столбца |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodHideGroupDetailWithBooleanInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Группировать строки и скрывать детали
            worksheet.Cells.GroupRows(0, 9, false);
            worksheet.Cells.HideGroupDetail(true, 4);
            worksheet.Cells.HideGroupDetail(true, 7);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


