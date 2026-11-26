---
title: "Cells.Merge"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Объединяет указанный диапазон ячеек в одну ячейку"
type: docs
url: /ru/net/aspose.cells/cells/merge/
---
## Merge(int, int, int, int) {#merge}

Объединяет указанный диапазон ячеек в одну ячейку.

```csharp
public void Merge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| firstRow | Int32 | Первая строка этого диапазона (нумерация с нуля) |
| firstColumn | Int32 | Первая колонка этого диапазона (нумерация с нуля) |
| totalRows | Int32 | Количество строк (нумерация с единицы) |
| totalColumns | Int32 | Количество колонок (нумерация с единицы) |

### Примечания

Ссылайтесь на объединённую ячейку через адрес верхней‑левой ячейки в диапазоне.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodMergeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Поместите значения в ячейки, чтобы продемонстрировать объединение
            cells[0, 0].PutValue("Merged Area");
            cells[5, 5].PutValue("Not Merged");

            // Объедините ячейки, начиная с строки 0, столбца 0, охватывая 3 строки и 2 столбца
            cells.Merge(0, 0, 3, 2);

            // Сохраните книгу
            workbook.Save("MergeDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Merge(int, int, int, int, bool) {#merge_1}

Объединяет указанный диапазон ячеек в одну ячейку.

```csharp
public void Merge(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    bool mergeConflict)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| firstRow | Int32 | Первая строка этого диапазона (нумерация с нуля) |
| firstColumn | Int32 | Первая колонка этого диапазона (нумерация с нуля) |
| totalRows | Int32 | Количество строк (нумерация с единицы) |
| totalColumns | Int32 | Количество колонок (нумерация с единицы) |
| mergeConflict | Boolean | Объединить конфликтные объединённые диапазоны. |

### Примечания

Ссылайтесь на объединённую ячейку через адрес верхней‑левой ячейки в диапазоне. Если mergeConflict равно true и объединённый диапазон конфликтует с другими объединёнными ячейками, другие объединённые ячейки будут автоматически удалены.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodMergeWithInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Объедините ячейки с строки 3, столбца 4 (D3) до строки 7, столбца 5 (E7) — 5 строк и 2 столбца
            worksheet.Cells.Merge(3, 4, 5, 2, true);
            
            // Сохраните книгу
            workbook.Save("MergeDemoOutput.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Merge(int, int, int, int, bool, bool) {#merge_2}

Объединяет указанный диапазон ячеек в одну ячейку.

```csharp
public void Merge(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    bool checkConflict, bool mergeConflict)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| firstRow | Int32 | Первая строка этого диапазона (нумерация с нуля) |
| firstColumn | Int32 | Первая колонка этого диапазона (нумерация с нуля) |
| totalRows | Int32 | Количество строк (нумерация с единицы) |
| totalColumns | Int32 | Количество колонок (нумерация с единицы) |
| checkConflict | Boolean | Указывает, проверяется ли пересечение объединённых ячеек с другими объединёнными ячейками |
| mergeConflict | Boolean | Объединить конфликтные объединённые диапазоны. |

### Примечания

Ссылайтесь на объединённую ячейку через адрес верхней‑левой ячейки в диапазоне. Если mergeConflict равно true и объединённый диапазон конфликтует с другими объединёнными ячейками, другие объединённые ячейки будут автоматически удалены.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodMergeWithInt32Int32Int32Int32BooleanBooDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Поместите некоторые данные в ячейки, которые будут объединены
            cells[0, 1].PutValue("Merged Cell");
            cells[1, 1].PutValue("This will be merged");

            // Объедините ячейки без параметров (простое объединение)
            cells.Merge(0, 1, 2, 2);
            Console.WriteLine("Cells merged without options");

            // Сначала разъедините, чтобы продемонстрировать следующее объединение
            cells.UnMerge(0, 1, 2, 2);

            // Объедините ячейки с ignoreStyle=false и mergeConflict=true
            cells.Merge(0, 1, 2, 2, false, true);
            Console.WriteLine("Cells merged with ignoreStyle=false and mergeConflict=true");

            // Сохраните книгу
            workbook.Save("MergeCellsDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


