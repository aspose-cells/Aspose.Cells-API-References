---
title: "Cells.ImportDataView"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Импортирует DataView в лист"
type: docs
url: /ru/net/aspose.cells/cells/importdataview/
---
## Cells.ImportDataView method

Импортирует DataView в рабочий лист.

```csharp
public int ImportDataView(DataView dataView, int firstRow, int firstColumn)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| dataView | DataView | Объект DataView для импорта. |
| firstRow | Int32 | Номер строки первой ячейки для импорта. |
| firstColumn | Int32 | Номер столбца первой ячейки для импорта. |

### Возвращаемое значение

Общее количество импортированных строк

### Примеры

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataViewWithDataViewInt32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Создать пример DataTable
            DataTable table = new DataTable("Products");
            table.Columns.Add("ID", typeof(int));
            table.Columns.Add("Name", typeof(string));
            table.Columns.Add("Price", typeof(decimal));

            // Добавьте примерные данные
            table.Rows.Add(1, "Laptop", 999.99m);
            table.Rows.Add(2, "Smartphone", 699.99m);
            table.Rows.Add(3, "Tablet", 399.99m);

            // Создать DataView из DataTable
            DataView dataView = new DataView(table);

            // Импортировать DataView в лист, начиная с строки 0, столбца 0
            cells.ImportDataView(dataView, 0, 0);

            // Сохраните книгу
            workbook.Save("ImportDataViewOutput.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


