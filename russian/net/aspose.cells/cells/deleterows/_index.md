---
title: "Cells.DeleteRows"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Удаляет несколько строк"
type: docs
url: /ru/net/aspose.cells/cells/deleterows/
---
## DeleteRows(int, int) {#deleterows}

Удаляет несколько строк.

```csharp
public bool DeleteRows(int rowIndex, int totalRows)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | Int32 | Индекс первой строки, которую нужно удалить. |
| totalRows | Int32 | Количество строк для удаления. |

### Примечания

Если удалённый диапазон содержит верхнюю часть (не полностью) таблицы (ListObject), диапазон не может быть удалён, и ничего не будет сделано. Это работает так же, как в MS Excel.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Заполните некоторыми образцовыми данными
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    cells[i, j].PutValue($"Row {i+1}, Col {j+1}");
                }
            }

            Console.WriteLine("Before deleting rows:");
            PrintCellValues(cells, 0, 9, 0, 4);

            // Удалить 2 строки, начиная с индекса строки 2 (3‑я строка)
            cells.DeleteRows(2, 2);

            Console.WriteLine("\nAfter deleting rows 3-4:");
            PrintCellValues(cells, 0, 7, 0, 4);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }

        private static void PrintCellValues(Cells cells, int startRow, int endRow, int startCol, int endCol)
        {
            for (int i = startRow; i <= endRow; i++)
            {
                for (int j = startCol; j <= endCol; j++)
                {
                    Console.Write($"{cells[i, j].StringValue}\t");
                }
                Console.WriteLine();
            }
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteRows(int, int, bool) {#deleterows_2}

Удаляет несколько строк в листе.

```csharp
public bool DeleteRows(int rowIndex, int totalRows, bool updateReference)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | Int32 | Индекс первой строки, которую нужно удалить. |
| totalRows | Int32 | Количество строк для удаления. |
| updateReference | Boolean | Указывает, следует ли обновлять ссылки в других листах. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteRowsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Импортировать данные в ячейки
            worksheet.Cells.ImportTwoDimensionArray(new object[2, 2] { { "A1", "B1" }, { "A2", "B2" } }, 0, 0);

            // Создать таблицу
            ListObject table = worksheet.ListObjects[worksheet.ListObjects.Add(0, 0, 1, 1, false)];
            table.ShowHeaderRow = false;

            Console.WriteLine("Before DeleteRows:");
            Console.WriteLine($"Table Data Range Row Count: {table.ListColumns.Count}");
            Console.WriteLine($"Table Start Row: {table.StartRow}");
            Console.WriteLine($"Table End Row: {table.EndRow}");

            // Удалить строку с индексом 1 (вторая строка) с обновлением ссылок
            worksheet.Cells.DeleteRows(1, 1, true);

            Console.WriteLine("\nAfter DeleteRows:");
            Console.WriteLine($"Table Data Range Row Count: {table.ListColumns.Count}");
            Console.WriteLine($"Table Start Row: {table.StartRow}");
            Console.WriteLine($"Table End Row: {table.EndRow}");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteRows(int, int, DeleteOptions) {#deleterows_1}

Удаляет несколько строк в листе.

```csharp
public bool DeleteRows(int rowIndex, int totalRows, DeleteOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | Int32 | Индекс первой строки, которую нужно удалить. |
| totalRows | Int32 | Количество строк для удаления. |
| опции | DeleteOptions | Параметры операции удаления |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteRowsWithInt32Int32DeleteOptionsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Установить примерные данные и формулы
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            cells["A3"].PutValue(30);
            cells["B1"].Formula = "=SUM(A1:A3)";
            
            // Удалить строку 2 без мониторинга (поскольку FormulaChangeMonitor недоступен)
            cells.DeleteRows(1, 1, new DeleteOptions());
            
            Console.WriteLine("Deleted row 2. Formula in B1 should now be: " + cells["B1"].Formula);
        }
    }
}
```

### См. также

* class [DeleteOptions](../../deleteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


