---
title: "Cells.CopyRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Копирует данные и форматы целой строки"
type: docs
url: /ru/net/aspose.cells/cells/copyrow/
---
## Cells.CopyRow method

Копирует данные и форматы целой строки.

```csharp
public void CopyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceCells | Ячейки | Объект Source Cells содержит данные и форматы для копирования. |
| sourceRowIndex | Int32 | Индекс исходной строки. |
| destinationRowIndex | Int32 | Индекс целевой строки. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyRowWithCellsInt32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet1 = workbook.Worksheets[0];
            Cells cells1 = worksheet1.Cells;
            
            // Добавьте некоторые данные в первую строку
            cells1["A1"].PutValue("Source Data");
            cells1["B1"].PutValue(100);
            cells1["C1"].PutValue(DateTime.Now);
            
            // Создайте второй лист
            Worksheet worksheet2 = workbook.Worksheets.Add("Sheet2");
            Cells cells2 = worksheet2.Cells;
            
            // Скопировать строку из Sheet1 в Sheet2
            cells2.CopyRow(cells1, 0, 0);
            
            // Скопировать строку внутри Sheet1 в новые позиции
            cells1.CopyRow(cells1, 0, 1);
            cells1.CopyRow(cells1, 0, 2);
            
            // Сохраните книгу
            workbook.Save("CopyRowExample.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


