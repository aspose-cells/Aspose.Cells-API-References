---
title: "Cells.ExportTypeArray"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Экспортирует тип значения ячейки в коллекции Cells в двумерный массивный объект"
type: docs
url: /ru/net/aspose.cells/cells/exporttypearray/
---
## Cells.ExportTypeArray method

Экспортирует тип значения ячейки в коллекции [`Cells`](../) в двумерный массивный объект.

```csharp
public CellValueType[] ExportTypeArray(int firstRow, int firstColumn, int totalRows, 
    int totalColumns)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| firstRow | Int32 | Номер строки первой ячейки для экспорта. |
| firstColumn | Int32 | Номер столбца первой ячейки для экспорта. |
| totalRows | Int32 | Количество строк для экспорта. |
| totalColumns | Int32 | Количество столбцов для экспорта. |

### Возвращаемое значение

Экспортированный массивный объект, представляющий типы значений ячеек.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportTypeArrayWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установить значения в cells
            cells["A1"].PutValue(10);
            cells["B1"].PutValue("Hello");
            cells["A2"].PutValue(true);
            cells["B2"].PutValue(DateTime.Now);

            // Экспортировать типы ячеек в 2‑мерный массив
            CellValueType[,] typeArray = cells.ExportTypeArray(0, 0, 2, 2);

            // Отобразите результаты
            for (int i = 0; i < 2; i++)
            {
                for (int j = 0; j < 2; j++)
                {
                    Console.WriteLine($"Cell[{i},{j}] Type: {typeArray[i, j]}");
                }
            }

            // Продемонстрировать случай исключения
            try
            {
                CellValueType[,] invalidArray = cells.ExportTypeArray(-1, 0, 2, 2);
            }
            catch (CellsException ex)
            {
                Console.WriteLine("Exception caught as expected: " + ex.Message);
            }
        }
    }
}
```

### См. также

* enum [CellValueType](../../cellvaluetype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


