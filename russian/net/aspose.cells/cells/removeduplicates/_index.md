---
title: "Cells.RemoveDuplicates"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Удаляет дублирующие строки в листе"
type: docs
url: /ru/net/aspose.cells/cells/removeduplicates/
---
## RemoveDuplicates() {#removeduplicates}

Удаляет дублирующиеся строки в листе.

```csharp
public void RemoveDuplicates()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodRemoveDuplicatesDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;

            // Заполнить ячейки некоторыми дублирующими значениями
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    // Создать дубликаты в каждой второй строке
                    cells[i, j].PutValue(i % 2 == 0 ? "Duplicate" : $"Unique_{i}_{j}");
                }
            }

            Console.WriteLine($"Before RemoveDuplicates: {cells.Count} cells");
            
            // Удалить дублирующие значения
            cells.RemoveDuplicates();

            Console.WriteLine($"After RemoveDuplicates: {cells.Count} cells");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveDuplicates(int, int, int, int) {#removeduplicates_1}

Удаляет дублирующиеся значения в диапазоне.

```csharp
public void RemoveDuplicates(int startRow, int startColumn, int endRow, int endColumn)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | Int32 | Начальная строка. |
| startColumn | Int32 | Начальный столбец |
| endRow | Int32 | Конечный индекс строки. |
| endColumn | Int32 | Конечный индекс столбца. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodRemoveDuplicatesWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Добавить примерные данные с дубликатами
            cells["A1"].PutValue("Apple");
            cells["A2"].PutValue("Orange");
            cells["A3"].PutValue("Apple");
            cells["A4"].PutValue("Banana");
            cells["A5"].PutValue("Orange");

            // Удалить дубликаты из столбца A (индекс с нуля)
            cells.RemoveDuplicates(0, 0, 5, 0);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveDuplicates(int, int, int, int, bool, int[]) {#removeduplicates_2}

Удаляет дублирующиеся данные диапазона.

```csharp
public void RemoveDuplicates(int startRow, int startColumn, int endRow, int endColumn, 
    bool hasHeaders, int[] columnOffsets)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | Int32 | Начальная строка. |
| startColumn | Int32 | Начальный столбец |
| endRow | Int32 | Конечный индекс строки. |
| endColumn | Int32 | Конечный индекс столбца. |
| hasHeaders | Boolean | Указывает, содержит ли диапазон заголовки. |
| columnOffsets | Int32[] | Смещения столбцов. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodRemoveDuplicatesWithInt32Int32Int32Int32BooleanIntDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Заполнить примерные данные дубликатами
            cells[0, 0].PutValue("ID");
            cells[0, 1].PutValue("Name");
            cells[0, 2].PutValue("Age");
            
            cells[1, 0].PutValue(1);
            cells[1, 1].PutValue("John");
            cells[1, 2].PutValue(30);

            cells[2, 0].PutValue(2);
            cells[2, 1].PutValue("Jane");
            cells[2, 2].PutValue(25);

            cells[3, 0].PutValue(1); // Duplicate ID
            cells[3, 1].PutValue("John"); // Duplicate Name
            cells[3, 2].PutValue(35);

            cells[4, 0].PutValue(3);
            cells[4, 1].PutValue("Bob");
            cells[4, 2].PutValue(40);

            try
            {
                // Удалить дубликаты из строк 1-4 (с нуля), столбцов 0-2
                // Проверить дубликаты на основе первых двух столбцов (ID и Name)
                cells.RemoveDuplicates(1, 0, 4, 2, true, new int[] { 0, 1 });

                Console.WriteLine("Duplicates removed successfully. Remaining rows: " + (cells.MaxDataRow + 1));
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveDuplicates method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("RemoveDuplicatesDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


