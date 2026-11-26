---
title: "DataSorter.AddKey"
second_title: "Справочник API Aspose.Cells для .NET"
description: "DataSorter method. Добавляет индекс отсортированного столбца и порядок сортировки"
type: docs
url: /ru/net/aspose.cells/datasorter/addkey/
---
## AddKey(int, SortOrder) {#addkey_1}

Добавляет индекс отсортированного столбца и порядок сортировки.

```csharp
public void AddKey(int key, SortOrder order)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| ключ | Int32 | Индекс отсортированного столбца (абсолютная позиция, столбец A — 0, B — 1, ...) |
| порядок | SortOrder | Порядок сортировки |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodAddKeyWithInt32SortOrderDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Пример данных
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(35);

            // Добавить ключ сортировки для столбца B (индекс 1) с возрастанием
            workbook.DataSorter.AddKey(1, SortOrder.Ascending);
            
            // Отсортировать диапазон данных (A1:B4)
            workbook.DataSorter.Sort(worksheet.Cells, 0, 0, 3, 1);

            // Вывести отсортированные значения
            Console.WriteLine("Sorted by Age (Ascending):");
            for (int i = 1; i <= 3; i++)
            {
                Console.WriteLine($"{worksheet.Cells[$"A{i+1}"].StringValue}: {worksheet.Cells[$"B{i+1}"].IntValue}");
            }
        }
    }
}
```

### См. также

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddKey(int, SortOrder, string) {#addkey_2}

Добавляет индекс отсортированного столбца и порядок сортировки с пользовательским списком сортировки.

```csharp
public void AddKey(int key, SortOrder order, string customList)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| ключ | Int32 | Индекс отсортированного столбца (абсолютная позиция, столбец A — 0, B — 1, ...) |
| порядок | SortOrder | Порядок сортировки. |
| customList | String | Пользовательский список сортировки. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodAddKeyWithInt32SortOrderStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Пример данных для сортировки
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("ddd");
            worksheet.Cells["A3"].PutValue("aaa");
            worksheet.Cells["A4"].PutValue("ccc");
            worksheet.Cells["A5"].PutValue("bbb");

            // Создать сортировщик данных и добавить пользовательский ключ сортировки
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending, "aaa,ddd,ccc,bbb");
            sorter.HasHeaders = true;

            // Отсортировать данные
            sorter.Sort(worksheet.Cells, CellArea.CreateCellArea("A1", "A5"));

            // Сохранить результат
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddKey(int, SortOnType, SortOrder, object) {#addkey}

Добавляет индекс отсортированного столбца и порядок сортировки с пользовательским списком сортировки.

```csharp
public void AddKey(int key, SortOnType type, SortOrder order, object customList)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| ключ | Int32 | Индекс отсортированного столбца (абсолютная позиция, столбец A — 0, B — 1, ...) |
| type | SortOnType | Тип отсортированного значения. |
| порядок | SortOrder | Порядок сортировки. |
| customList | Object | Пользовательский список сортировки. |

### Примечания

Если тип равен SortOnType.CellColor или SortOnType.FontColor, customList имеет тип Color.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataSorterMethodAddKeyWithInt32SortOnTypeSortOrderObjectDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(35);

            // Создать сортировщик данных
            DataSorter sorter = workbook.DataSorter;
            sorter.HasHeaders = true;

            try
            {
                // Вызвать AddKey с параметрами: (Int32, SortOnType, SortOrder, Object)
                sorter.AddKey(
                    1,                          // Column index (B column)
                    SortOnType.Value,           // Sort on values (fixed from Values to Value)
                    SortOrder.Ascending,        // Sort order
                    null                        // Custom list (null for default)
                );

                // Определить диапазон для сортировки
                CellArea area = new CellArea();
                area.StartRow = 0;
                area.StartColumn = 0;
                area.EndRow = 3;
                area.EndColumn = 1;

                // Отсортировать данные
                sorter.Sort(worksheet.Cells, area);

                Console.WriteLine("Data sorted successfully using AddKey with parameters (Int32, SortOnType, SortOrder, Object)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddKey method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("DataSorterMethodAddKeyWithInt32SortOnTypeSortOrderObjectDemo.xlsx");
        }
    }
}
```

### См. также

* enum [SortOnType](../../sortontype/)
* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddKey(int, SortOrder, string[]) {#addkey_3}

Добавляет индекс отсортированного столбца и порядок сортировки с пользовательским списком сортировки.

```csharp
public void AddKey(int key, SortOrder order, string[] customList)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| ключ | Int32 | Индекс отсортированного столбца (абсолютная позиция, столбец A — 0, B — 1, ...) |
| порядок | SortOrder | Порядок сортировки. |
| customList | String[] | Пользовательский список сортировки. |

### См. также

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


