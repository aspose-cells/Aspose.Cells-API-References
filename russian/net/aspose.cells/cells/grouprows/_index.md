---
title: "Cells.GroupRows"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Группирует строки"
type: docs
url: /ru/net/aspose.cells/cells/grouprows/
---
## GroupRows(int, int, bool) {#grouprows_1}

Группирует строки.

```csharp
public void GroupRows(int firstIndex, int lastIndex, bool isHidden)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| firstIndex | Int32 | Первый индекс строки для группировки. |
| lastIndex | Int32 | Последний индекс строки для группировки. |
| isHidden | Boolean | Указывает, скрыты ли сгруппированные строки. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGroupRowsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Заполните некоторыми данными
            for (int i = 0; i < 10; i++)
            {
                cells[i, 0].PutValue($"Group {i + 1}");
                for (int j = 1; j <= 5; j++)
                {
                    cells[i, j].PutValue($"Data {j}");
                }
            }

            // Сгруппировать строки с 1 по 5 (индекс с нуля) и скрыть их
            cells.GroupRows(1, 5, true);

            // Установить строку итога ниже группы
            worksheet.Outline.SummaryRowBelow = false;

            // Сохраните книгу
            workbook.Save("GroupRowsDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GroupRows(int, int) {#grouprows}

Группирует строки.

```csharp
public void GroupRows(int firstIndex, int lastIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| firstIndex | Int32 | Первый индекс строки для группировки. |
| lastIndex | Int32 | Последний индекс строки для группировки. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGroupRowsWithInt32Int32Demo
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
                cells[i, 0].PutValue("Row " + (i + 1));
            }

            // Сгруппировать строки с 2 по 5 (индекс с нуля)
            cells.GroupRows(1, 4);

            // Сохраните книгу
            workbook.Save("GroupRowsExample.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


