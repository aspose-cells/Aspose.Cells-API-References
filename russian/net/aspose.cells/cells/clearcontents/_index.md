---
title: "Cells.ClearContents"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Очищает содержимое диапазона"
type: docs
url: /ru/net/aspose.cells/cells/clearcontents/
---
## ClearContents(CellArea) {#clearcontents}

Очищает содержимое диапазона.

```csharp
public void ClearContents(CellArea range)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| диапазон | CellArea | Диапазон для очистки. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodClearContentsWithCellAreaDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Заполнить некоторыми данными область ячеек
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 2;
            area.EndColumn = 2;

            for (int row = area.StartRow; row <= area.EndRow; row++)
            {
                for (int col = area.StartColumn; col <= area.EndColumn; col++)
                {
                    cells[row, col].PutValue($"Data_{row}_{col}");
                }
            }

            Console.WriteLine("Before ClearContents:");
            PrintCellAreaContents(cells, area);

            // Очистить содержимое области ячеек
            cells.ClearContents(area);

            Console.WriteLine("\nAfter ClearContents:");
            PrintCellAreaContents(cells, area);
        }

        private static void PrintCellAreaContents(Cells cells, CellArea area)
        {
            for (int row = area.StartRow; row <= area.EndRow; row++)
            {
                for (int col = area.StartColumn; col <= area.EndColumn; col++)
                {
                    Console.Write(cells[row, col].StringValue + "\t");
                }
                Console.WriteLine();
            }
        }
    }
}
```

### См. также

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ClearContents(int, int, int, int) {#clearcontents_1}

Очищает содержимое диапазона.

```csharp
public void ClearContents(int startRow, int startColumn, int endRow, int endColumn)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | Int32 | Индекс начальной строки. |
| startColumn | Int32 | Индекс начального столбца. |
| endRow | Int32 | Индекс конечной строки. |
| endColumn | Int32 | Индекс конечного столбца. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodClearContentsWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Заполните некоторые ячейки значениями
            cells[0, 0].PutValue("Value A1");
            cells[0, 1].PutValue("Value B1");
            cells[1, 0].PutValue("Value A2");
            cells[1, 1].PutValue("Value B2");

            // Отобразить исходные значения
            Console.WriteLine("Before ClearContents:");
            Console.WriteLine("A1: " + cells[0, 0].StringValue);
            Console.WriteLine("B1: " + cells[0, 1].StringValue);
            Console.WriteLine("A2: " + cells[1, 0].StringValue);
            Console.WriteLine("B2: " + cells[1, 1].StringValue);

            // Очистить содержимое ячеек в диапазоне (0,1) до (1,1)
            cells.ClearContents(0, 1, 1, 1);

            // Отобразить значения после очистки
            Console.WriteLine("\nAfter ClearContents(0, 1, 1, 1):");
            Console.WriteLine("A1: " + cells[0, 0].StringValue);
            Console.WriteLine("B1: " + cells[0, 1].StringValue);
            Console.WriteLine("A2: " + cells[1, 0].StringValue);
            Console.WriteLine("B2: " + cells[1, 1].StringValue);

            // Сохраните книгу
            workbook.Save("ClearContentsDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


