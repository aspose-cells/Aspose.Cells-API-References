---
title: "Cells.ImportGridView"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Импортирует представление сетки в эти ячейки"
type: docs
url: /ru/net/aspose.cells/cells/importgridview/
---
## Cells.ImportGridView method

Импортирует представление сетки в эти ячейки.

```csharp
public int ImportGridView(GridView gridView, int firstRow, int firstColumn, 
    ImportTableOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| gridView | GridView | Объект представления сетки. |
| firstRow | Int32 | Номер строки первой ячейки для импорта. |
| firstColumn | Int32 | Номер столбца первой ячейки для импорта. |
| опции | ImportTableOptions | параметры импорта. |

### Возвращаемое значение

Номер строки.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class CellsMethodImportGridViewWithGridViewInt32Int32ImportTableOptiDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте DataTable для имитации данных GridView
            DataTable dataTable = new DataTable();
            dataTable.Columns.Add("Name");
            dataTable.Columns.Add("Price");
            dataTable.Columns.Add("Stock");

            dataTable.Rows.Add("Product A", 100.5, 50);
            dataTable.Rows.Add("Product B", 200.75, 30);
            dataTable.Rows.Add("Product C", 150.25, 75);

            try
            {
                // Создайте ImportTableOptions
                ImportTableOptions options = new ImportTableOptions();
                options.IsFieldNameShown = true;
                options.InsertRows = true;

                // Импортируйте данные DataTable, начиная с ячейки B3 (строка 2, столбец 1)
                worksheet.Cells.ImportData(dataTable, 2, 1, options);

                Console.WriteLine("Data imported successfully starting at cell B3");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing data: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("CellsMethodImportGridViewWithGridViewInt32Int32ImportTableOptiDemo.xlsx");
        }
    }
}
```

### См. также

* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


