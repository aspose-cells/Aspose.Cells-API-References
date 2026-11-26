---
title: "Cells.InsertColumn"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Вставляет новый столбец в лист"
type: docs
url: /ru/net/aspose.cells/cells/insertcolumn/
---
## InsertColumn(int, bool) {#insertcolumn_1}

Вставляет новый столбец в лист.

```csharp
public void InsertColumn(int columnIndex, bool updateReference)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | Int32 | Индекс столбца. |
| updateReference | Boolean | Указывает, будут ли обновляться ссылки в других листах. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertColumnWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Заполните некоторыми примерными данными столбец 0
            Cells cells = sheet.Cells;
            for (int i = 0; i < 5; i++)
            {
                cells[i, 0].PutValue($"Original {i}");
            }

            // Вставьте новый столбец с индексом 1 и сдвиньте столбцы вправо
            cells.InsertColumn(1, true);

            // Скопируйте данные из столбца 0 в новый столбец 1
            cells.CopyColumn(cells, 0, 1);

            // Сохраните книгу
            workbook.Save("InsertColumnDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertColumn(int) {#insertcolumn}

Вставляет новый столбец в лист.

```csharp
public void InsertColumn(int columnIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | Int32 | Индекс столбца. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertColumnWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet sheet = workbook.Worksheets[0];
            
            // Получите коллекцию ячеек
            Cells cells = sheet.Cells;
            
            // Вставьте данные в ячейки для демонстрации
            cells["A1"].PutValue("Column A");
            cells["B1"].PutValue("Column B");
            cells["C1"].PutValue("Column C");
            
            // Вставьте новый столбец с индексом 1 (это станет новым столбцом B)
            cells.InsertColumn(1);
            
            // Проверьте, вставив данные в новый столбец
            cells["B1"].PutValue("New Column");
            
            // Сохраните книгу
            workbook.Save("InsertColumnDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


