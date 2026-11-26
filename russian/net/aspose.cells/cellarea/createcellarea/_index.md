---
title: "CellArea.CreateCellArea"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CellArea. Создает область ячеек"
type: docs
url: /ru/net/aspose.cells/cellarea/createcellarea/
---
## CreateCellArea(int, int, int, int) {#createcellarea}

Создаёт область ячеек.

```csharp
public static CellArea CreateCellArea(int startRow, int startColumn, int endRow, int endColumn)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | Int32 | Начальная строка. |
| startColumn | Int32 | Начальный столбец. |
| endRow | Int32 | Конечная строка. |
| endColumn | Int32 | Конечный столбец. |

### Возвращаемое значение

Верните [`CellArea`](../).

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellAreaMethodCreateCellAreaWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Заполните ячейки примерными данными
            int[] values = { 1, 3, 2, 6, 4, 5, 8, 9, 7 };
            for (int i = 0; i < values.Length; i++)
            {
                cells[i, i / 3].PutValue(values[i]);
            }

            // Создайте и настройте сортировщик данных
            DataSorter sorter = wb.DataSorter;
            sorter.Clear();
            sorter.Order1 = SortOrder.Ascending;
            sorter.Key1 = 2;
            sorter.Order2 = SortOrder.Ascending;
            sorter.Key2 = 1;
            sorter.Order3 = SortOrder.Ascending;
            sorter.Key3 = 0;

            // Сортируйте, используя CreateCellArea с параметрами Int32
            sorter.Sort(cells, CellArea.CreateCellArea(0, 0, 8, 2));

            // Вывести отсортированные значения
            Console.WriteLine("Sorted values:");
            for (int i = 0; i < 9; i++)
            {
                Console.WriteLine(cells[i, 2 - i / 3].IntValue);
            }
        }
    }
}
```

### См. также

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateCellArea(string, string) {#createcellarea_1}

Создаёт область ячеек.

```csharp
public static CellArea CreateCellArea(string startCellName, string endCellName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startCellName | String | Ячейка в левом верхнем углу диапазона. |
| endCellName | String | Ячейка в правом нижнем углу диапазона. |

### Возвращаемое значение

Верните [`CellArea`](../).

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellAreaMethodCreateCellAreaWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Заполните некоторые данные в столбце A
            for (int i = 0; i < 10; i++)
            {
                cells[i, 0].PutValue($"Data {i}");
            }

            // Создайте область ячеек от B1 до B10
            CellArea area = CellArea.CreateCellArea("B1", "B10");
            
            // Вставьте диапазон, сдвигая ячейки вниз
            cells.InsertRange(area, ShiftType.Down);
            
            // Проверьте операцию, проверяя значения ячеек
            Console.WriteLine("Inserted range from B1 to B10. Total rows: " + cells.Rows.Count);
        }
    }
}
```

### См. также

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


