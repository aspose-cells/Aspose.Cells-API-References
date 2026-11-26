---
title: "Cells.DeleteRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Удаляет диапазон ячеек и сдвигает ячейки согласно параметру сдвига"
type: docs
url: /ru/net/aspose.cells/cells/deleterange/
---
## Cells.DeleteRange method

Удаляет диапазон ячеек и сдвигает ячейки в соответствии с параметром сдвига.

```csharp
public void DeleteRange(int startRow, int startColumn, int endRow, int endColumn, 
    ShiftType shiftType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | Int32 | Индекс начальной строки. |
| startColumn | Int32 | Индекс начального столбца. |
| endRow | Int32 | Индекс конечной строки. |
| endColumn | Int32 | Индекс конечного столбца. |
| shiftType | ShiftType | Опция смещения ячеек. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteRangeWithInt32Int32Int32Int32ShiftTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Заполните некоторыми образцовыми данными
            sheet.Cells["A1"].PutValue("A1");
            sheet.Cells["B1"].PutValue("B1");
            sheet.Cells["C1"].PutValue("C1");
            sheet.Cells["A2"].PutValue("A2");
            sheet.Cells["B2"].PutValue("B2");
            sheet.Cells["C2"].PutValue("C2");

            // Удалить диапазон и сдвинуть влево
            sheet.Cells.DeleteRange(0, 1, 1, 2, ShiftType.Left);

            // Сохраните книгу
            workbook.Save("DeleteRangeExample.xlsx");
        }
    }
}
```

### См. также

* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


