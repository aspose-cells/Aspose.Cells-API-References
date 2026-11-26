---
title: "WorkbookDesigner.SortDataSource"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookDesigner. Указывает, сортировать ли источник данных"
type: docs
url: /ru/net/aspose.cells/workbookdesigner/sortdatasource/
---
## WorkbookDesigner.SortDataSource property

Указывает, сортировать ли источник данных.

```csharp
[EditorBrowsable(EditorBrowsableState.Never)]
public bool SortDataSource { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Это свойство будет удалено через 12 месяцев, начиная с октября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать. Источник данных Json будет отсортирован, если смарт‑маркер содержит параметры возрастания и убывания.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class WorkbookDesignerPropertySortDataSourceDemo
    {
        public static void Run()
        {
            // Создать пример DataTable с неотсортированными данными
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ProductID", typeof(int));
            dataTable.Columns.Add("ProductName", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));

            // Добавить примерные данные в неотсортированном порядке
            dataTable.Rows.Add(3, "Product C", 15.99m);
            dataTable.Rows.Add(1, "Product A", 10.50m);
            dataTable.Rows.Add(2, "Product B", 12.75m);

            // Создать книгу со смарт‑маркировками
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Настроить умные маркеры в листе
            worksheet.Cells["A1"].PutValue("&=$ProductID");
            worksheet.Cells["B1"].PutValue("&=$ProductName");
            worksheet.Cells["C1"].PutValue("&=$Price");

            try
            {
                // Создать экземпляр WorkbookDesigner
                WorkbookDesigner designer = new WorkbookDesigner(workbook);

                // Отобразить начальное значение SortDataSource
                Console.WriteLine($"Initial SortDataSource value: {designer.SortDataSource}");

                // Установить источник данных без сортировки
                designer.SortDataSource = false;
                designer.SetDataSource(dataTable);
                designer.Process();

                // Сохранить неотсортированный результат
                workbook.Save("UnsortedOutput.xlsx");
                Console.WriteLine("Unsorted data saved to UnsortedOutput.xlsx");

                // Создать новую книгу для демонстрации сортировки
                Workbook sortedWorkbook = new Workbook();
                Worksheet sortedSheet = sortedWorkbook.Worksheets[0];
                sortedSheet.Cells["A1"].PutValue("&=$ProductID");
                sortedSheet.Cells["B1"].PutValue("&=$ProductName");
                sortedSheet.Cells["C1"].PutValue("&=$Price");

                // Создать новый дизайнер с включённой сортировкой
                WorkbookDesigner sortedDesigner = new WorkbookDesigner(sortedWorkbook);
                sortedDesigner.SortDataSource = true;
                sortedDesigner.SetDataSource(dataTable);
                sortedDesigner.Process();

                // Сохранить отсортированный результат
                sortedWorkbook.Save("SortedOutput.xlsx");
                Console.WriteLine("Sorted data saved to SortedOutput.xlsx");
                Console.WriteLine($"Final SortDataSource value: {sortedDesigner.SortDataSource}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


