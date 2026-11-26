---
title: "Cells.UnMerge"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Разъединяет указанный диапазон объединённых ячеек"
type: docs
url: /ru/net/aspose.cells/cells/unmerge/
---
## Cells.UnMerge method

Разъединяет указанный диапазон объединённых ячеек.

```csharp
public void UnMerge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| firstRow | Int32 | Первая строка этого диапазона (нумерация с нуля) |
| firstColumn | Int32 | Первая колонка этого диапазона (нумерация с нуля) |
| totalRows | Int32 | Количество строк (нумерация с единицы) |
| totalColumns | Int32 | Количество колонок (нумерация с единицы) |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUnMergeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Сначала объедините ячейки
            cells.Merge(0, 0, 2, 2);
            
            // Разъедините ранее объединённые ячейки
            cells.UnMerge(0, 0, 2, 2);
            
            // Сохраните книгу
            workbook.Save("UnMergeDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


