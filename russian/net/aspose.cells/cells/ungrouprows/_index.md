---
title: "Cells.UngroupRows"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Разгруппирует строки"
type: docs
url: /ru/net/aspose.cells/cells/ungrouprows/
---
## UngroupRows(int, int, bool) {#ungrouprows_1}

Разгруппирует строки.

```csharp
public void UngroupRows(int firstIndex, int lastIndex, bool isAll)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| firstIndex | Int32 | Первый индекс строки, который будет разгруппирован. |
| lastIndex | Int32 | Последний индекс строки, который будет разгруппирован. |
| isAll | Boolean | True, удаляет всю информацию о группировке. Иначе, удаляет информацию о внешней группе. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodUngroupRowsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте вложенные группировки строк для демонстрации
            worksheet.Cells.GroupRows(5, 7);  // First level grouping
            worksheet.Cells.GroupRows(5, 7);  // Second level grouping

            try
            {
                // Разгруппировать все уровни строк 5-7
                worksheet.Cells.UngroupRows(5, 7, true);

                Console.WriteLine("Rows 5-7 successfully ungrouped with all levels removed");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UngroupRows: {ex.Message}");
            }

            // Сохранить изменённую книгу
            workbook.Save("UngroupRowsWithBooleanDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## UngroupRows(int, int) {#ungrouprows}

Разгруппирует строки.

```csharp
public void UngroupRows(int firstIndex, int lastIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| firstIndex | Int32 | Первый индекс строки, который будет разгруппирован. |
| lastIndex | Int32 | Последний индекс строки, который будет разгруппирован. |

### Примечания

Удаляет только информацию о внешней группе.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUngroupRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Заполните некоторыми данными
            for (int i = 0; i < 6; i++)
            {
                cells[i, 0].PutValue($"Row {i}");
            }

            // Группировать строки с 1 по 3 (индексация с нуля)
            cells.GroupRows(1, 3, true);

            Console.WriteLine("Rows grouped from index 1 to 3");

            // Разгруппировать те же строки
            cells.UngroupRows(1, 3);

            Console.WriteLine("Rows ungrouped from index 1 to 3");

            // Сохраните книгу
            workbook.Save("UngroupRowsDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


