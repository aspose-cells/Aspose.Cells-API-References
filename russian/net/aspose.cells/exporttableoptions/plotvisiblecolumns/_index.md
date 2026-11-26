---
title: "ExportTableOptions.PlotVisibleColumns"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExportTableOptions. Экспортирует только видимые столбцы"
type: docs
url: /ru/net/aspose.cells/exporttableoptions/plotvisiblecolumns/
---
## ExportTableOptions.PlotVisibleColumns property

Экспортирует только видимые столбцы.

```csharp
public bool PlotVisibleColumns { get; set; }
```

### Примеры

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyPlotVisibleColumnsDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные и скрыть некоторые столбцы
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["B1"].PutValue("Column2");
            worksheet.Cells["C1"].PutValue("Column3");
            worksheet.Cells["D1"].PutValue("Column4");
            
            for (int i = 2; i <= 5; i++)
            {
                worksheet.Cells[$"A{i}"].PutValue($"Data{i-1}_1");
                worksheet.Cells[$"B{i}"].PutValue($"Data{i-1}_2");
                worksheet.Cells[$"C{i}"].PutValue($"Data{i-1}_3");
                worksheet.Cells[$"D{i}"].PutValue($"Data{i-1}_4");
            }
            
            // Скрыть столбец C
            worksheet.Cells.HideColumn(2);

            // Экспортировать данные с PlotVisibleColumns, установленным в true
            ExportTableOptions options = new ExportTableOptions();
            options.ExportColumnName = true;
            options.PlotVisibleColumns = true;

            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 6, 4, options);
            
            // Выведите результаты
            Console.WriteLine("Exported DataTable Columns:");
            foreach (DataColumn column in dataTable.Columns)
            {
                Console.WriteLine(column.ColumnName);
            }
        }
    }
}
```

### См. также

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


