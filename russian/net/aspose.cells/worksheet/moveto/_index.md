---
title: "Worksheet.MoveTo"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Worksheet. Перемещает лист в другое место в таблице"
type: docs
url: /ru/net/aspose.cells/worksheet/moveto/
---
## Worksheet.MoveTo method

Перемещает лист в другое место в таблице.

```csharp
public void MoveTo(int index)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 | Индекс листа назначения. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodMoveToWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить несколько листов
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Добавить новый лист и переместить его в позицию 1
            Worksheet newWorksheet = workbook.Worksheets.Add("MovedSheet");
            newWorksheet.MoveTo(1);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


