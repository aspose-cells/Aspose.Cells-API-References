---
title: "Cells.GroupColumns"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Группирует столбцы"
type: docs
url: /ru/net/aspose.cells/cells/groupcolumns/
---
## GroupColumns(int, int) {#groupcolumns}

Группирует столбцы.

```csharp
public void GroupColumns(int firstIndex, int lastIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| firstIndex | Int32 | Индекс первого столбца для группировки. |
| lastIndex | Int32 | Индекс последнего столбца для группировки. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGroupColumnsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Группировать столбцы с индекса 0 до 255
            cells.GroupColumns(0, 255);

            // Сохраните книгу
            string outputPath = "outputGroupColumns.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("Columns grouped successfully. File saved to: " + outputPath);
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GroupColumns(int, int, bool) {#groupcolumns_1}

Группирует столбцы.

```csharp
public void GroupColumns(int firstIndex, int lastIndex, bool isHidden)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| firstIndex | Int32 | Индекс первого столбца для группировки. |
| lastIndex | Int32 | Индекс последнего столбца для группировки. |
| isHidden | Boolean | Указывает, скрыты ли сгруппированные столбцы. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGroupColumnsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Группировать столбцы с 5 по 7 (3 столбца) и скрыть их
            cells.GroupColumns(5, 7, true);

            // Сохраните книгу
            workbook.Save("GroupColumnsOutput.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


