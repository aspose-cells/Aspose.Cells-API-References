---
title: "Cells.CopyColumn"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Копирует данные и форматы целого столбца"
type: docs
url: /ru/net/aspose.cells/cells/copycolumn/
---
## Cells.CopyColumn method

Копирует данные и форматы целого столбца.

```csharp
public void CopyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceCells | Ячейки | Объект Source Cells содержит данные и форматы для копирования. |
| sourceColumnIndex | Int32 | Индекс исходного столбца. |
| destinationColumnIndex | Int32 | Индекс целевого столбца. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyColumnWithCellsInt32Int32Demo
    {
        public static void Run()
        {
            // Создайте исходную книгу и заполните данные
            Workbook wbSrc = new Workbook();
            Cells cellsSrc = wbSrc.Worksheets[0].Cells;
            cellsSrc[0, 255].PutValue(1);
            cellsSrc[1, 255].PutValue(true);
            cellsSrc[2, 255].PutValue("abc");
            cellsSrc[3, 255].PutValue(false);
            cellsSrc[65535, 255].PutValue(2.56);

            // Создайте целевую книгу
            Workbook wbDest = new Workbook();
            Cells cellsDest = wbDest.Worksheets[0].Cells;

            // Скопировать столбец из источника в назначение
            cellsDest.CopyColumn(cellsSrc, 255, 0);

            // Сохранить результат
            wbDest.Save("outputCopyColumn.xlsx");
            
            Console.WriteLine("Column copied successfully.");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


