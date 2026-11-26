---
title: "DataSorter.Sort"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод DataSorter. Сортирует данные области"
type: docs
url: /ru/net/aspose.cells/datasorter/sort/
---
## Sort(Cells, int, int, int, int) {#sort_2}

Сортирует данные области.

```csharp
public int[] Sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| ячейки | Ячейки | Ячейки содержат область данных. |
| startRow | Int32 | Начальная строка области. |
| startColumn | Int32 | Начальный столбец области. |
| endRow | Int32 | Конечная строка области. |
| endColumn | Int32 | Конечный столбец области. |

### Возвращаемое значение

Исходные индексы (абсолютные позиции, например, столбец A — 0, B — 1, ...) отсортированных строк/столбцов. Если ни одной строки/столбца не требуется перемещать этой операцией сортировки, будет возвращено null.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodSortWithCellsInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Заполнить примерными данными
            for (int i = 0; i < 6; i++)
            {
                cells[i, 0].PutValue(6 - i);
            }
            
            // Скройте строку, чтобы продемонстрировать сортировку с скрытыми строками
            cells.Rows[1].IsHidden = true;
            
            // Создайте и настройте сортировщик
            DataSorter sorter = wb.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);
            
            // Продемонстрировать метод Sort с параметрами Cells и Int32
            sorter.Sort(cells, 0, 0, 5, 0);
            
            // Вывести результаты в консоль
            for (int i = 0; i < 6; i++)
            {
                Console.WriteLine($"Cell A{i+1}: {cells[i, 0].IntValue}");
            }
            Console.WriteLine($"Is row 2 hidden? {cells.Rows[1].IsHidden}");
        }
    }
}
```

### См. также

* class [Cells](../../cells/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Sort(Cells, CellArea) {#sort_1}

Отсортировать данные области.

```csharp
public int[] Sort(Cells cells, CellArea area)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| ячейки | Ячейки | Ячейки содержат область данных. |
| область | CellArea | Область, необходимая для сортировки |

### Возвращаемое значение

Исходные индексы (абсолютные позиции, например, столбец A — 0, B — 1, ...) отсортированных строк/столбцов. Если ни одной строки/столбца не требуется перемещать этой операцией сортировки, будет возвращено null.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodSortWithCellsCellAreaDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Year");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue(1995);
            worksheet.Cells["B2"].PutValue(10000);
            worksheet.Cells["A3"].PutValue(1996);
            worksheet.Cells["B3"].PutValue(15000);
            worksheet.Cells["A4"].PutValue(1997);
            worksheet.Cells["B4"].PutValue(12000);
            worksheet.Cells["A5"].PutValue(1998);
            worksheet.Cells["B5"].PutValue(18000);

            // Создать сортировщик данных
            DataSorter dataSorter = workbook.DataSorter;
            dataSorter.HasHeaders = true;
            dataSorter.Key1 = 0; // Sort by first column (Year)
            dataSorter.Order1 = SortOrder.Descending;

            // Определить область сортировки
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 4;
            area.EndColumn = 1;

            // Выполнить сортировку
            dataSorter.Sort(worksheet.Cells, area);

            // Сохраните книгу
            workbook.Save("SortedData.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../../cells/)
* struct [CellArea](../../cellarea/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Sort() {#sort}

Отсортировать данные в диапазоне.

```csharp
public int[] Sort()
```

### Возвращаемое значение

Исходные индексы (абсолютные позиции, например, столбец A — 0, B — 1, ...) отсортированных строк/столбцов. Если ни одной строки/столбца не требуется перемещать этой операцией сортировки, будет возвращено null.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodSortDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для сортировки
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("C");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("A");
            worksheet.Cells["B3"].PutValue(10);
            worksheet.Cells["A4"].PutValue("B");
            worksheet.Cells["B4"].PutValue(20);

            // Создать объект таблицы/списка
            int index = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[index];
            table.ShowTotals = true;

            // Отсортировать данные по первому столбцу
            table.AutoFilter.Sorter.Sort();

            // Сохраните книгу
            workbook.Save("SortedData.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


