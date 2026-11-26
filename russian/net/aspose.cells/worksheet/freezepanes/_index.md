---
title: "Worksheet.FreezePanes"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Worksheet. Замораживает области в указанной ячейке листа"
type: docs
url: /ru/net/aspose.cells/worksheet/freezepanes/
---
## FreezePanes(int, int, int, int) {#freezepanes}

Замораживает области в указанной ячейке листа.

```csharp
public void FreezePanes(int row, int column, int freezedRows, int freezedColumns)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки. |
| column | Int32 | Индекс столбца. |
| freezedRows | Int32 | Количество видимых строк в верхней области, не более индекса строки. |
| freezedColumns | Int32 | Количество видимых столбцов в левой области, не более индекса столбца. |

### Примечания

Индекс строки и индекс столбца не могут быть одновременно нулевыми. Количество строк и количество столбцов также не могут быть одновременно нулевыми.

Первые два параметра задают позицию заморозки, а последние два параметра задают область, замороженную в левом верхнем окне.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodFreezePanesWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Заморозьте области в строке 3, столбце 3, с 3 замороженными строками и 3 замороженными столбцами
            worksheet.FreezePanes(3, 3, 3, 3);
            
            // Сохраните книгу
            workbook.Save("FreezePanesDemo.xlsx");
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## FreezePanes(string, int, int) {#freezepanes_1}

Замораживает области в указанной ячейке листа.

```csharp
public void FreezePanes(string cellName, int freezedRows, int freezedColumns)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| cellName | String | Имя ячейки. |
| freezedRows | Int32 | Количество видимых строк в верхней области, не более индекса строки. |
| freezedColumns | Int32 | Количество видимых столбцов в левой области, не более индекса столбца. |

### Примечания

Индекс строки и индекс столбца не могут быть одновременно нулевыми. Количество строк и количество столбцов также не могут быть одновременно нулевыми.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodFreezePanesWithStringInt32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Заморозьте области в "C3" с 3 замороженными строками и 3 замороженными столбцами
            worksheet.FreezePanes("C3", 3, 3);

            // Сохраните книгу
            workbook.Save("FreezePanesDemo.xlsx");
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


