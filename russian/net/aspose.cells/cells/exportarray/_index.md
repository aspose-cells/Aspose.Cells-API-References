---
title: "Cells.ExportArray"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Экспортирует данные из коллекции Cells в двумерный массив"
type: docs
url: /ru/net/aspose.cells/cells/exportarray/
---
## Cells.ExportArray method

Экспортирует данные из коллекции [`Cells`](../) в двумерный массивный объект.

```csharp
public object[] ExportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| firstRow | Int32 | Номер строки первой ячейки для экспорта. |
| firstColumn | Int32 | Номер столбца первой ячейки для экспорта. |
| totalRows | Int32 | Количество строк для экспорта |
| totalColumns | Int32 | Количество столбцов для экспорта |

### Возвращаемое значение

Экспортированный объект массива значений ячеек.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportArrayWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Заполните некоторыми образцовыми данными
            cells[0, 0].PutValue("A");
            cells[0, 1].PutValue("B");
            cells[1, 0].PutValue(10);
            cells[1, 1].PutValue(20);

            try
            {
                // Экспортировать данные в массив
                object[,] dataArray = cells.ExportArray(0, 0, 2, 2);
                
                // Отобразить экспортированный массив
                for (int i = 0; i < 2; i++)
                {
                    for (int j = 0; j < 2; j++)
                    {
                        Console.Write(dataArray[i, j] + "\t");
                    }
                    Console.WriteLine();
                }
            }
            catch (CellsException ex)
            {
                Console.WriteLine("Error exporting array: " + ex.Message);
            }
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


