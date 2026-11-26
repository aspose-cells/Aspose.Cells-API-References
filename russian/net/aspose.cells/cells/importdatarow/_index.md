---
title: "Cells.ImportDataRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Импортирует объект DataRow в файл Excel"
type: docs
url: /ru/net/aspose.cells/cells/importdatarow/
---
## Cells.ImportDataRow method

Импортирует DataRow в файл Excel.

```csharp
public void ImportDataRow(DataRow dataRow, int row, int firstColumn)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| dataRow | DataRow | Объект DataRow. |
| строка | Int32 | Индекс строки. |
| firstColumn | Int32 | Индекс первого столбца. |

### Примеры

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataRowWithDataRowInt32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Создать примерный DataTable
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));

            // Добавьте примерные данные
            dataTable.Rows.Add(1, "Product A", 19.99m);
            dataTable.Rows.Add(2, "Product B", 29.99m);

            // Импортировать первую строку из DataTable в лист, начиная с строки 0, столбца 0
            cells.ImportDataRow(dataTable.Rows[0], 0, 0);

            // Сохраните книгу
            workbook.Save("ImportDataRowDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


