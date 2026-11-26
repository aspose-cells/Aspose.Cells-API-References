---
title: "ExportTableOptions.CheckMixedValueType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExportTableOptions. False Aspose.Cells установит тип DataColumns по типу значения первой строки для повышения производительности. True Aspose.Cells проверит, смешаны ли типы значений в столбце, прежде чем установить тип DataColumns. И если типы значений смешаны, тип DataColumns будет string."
type: docs
url: /ru/net/aspose.cells/exporttableoptions/checkmixedvaluetype/
---
## ExportTableOptions.CheckMixedValueType property

False: Aspose.Cells установит тип DataColumn по типу значения первой строки для повышения производительности. True: Aspose.Cells проверит, смешаны ли типы значений в столбце, перед установкой типа DataColumn, и если типы смешаны, тип DataColumn будет string.

```csharp
public bool CheckMixedValueType { get; set; }
```

### Примеры

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyCheckMixedValueTypeDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить заголовки
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Value Date");

            // Добавить примерные данные со смешанными типами
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(DateTime.Now);
            worksheet.Cells["A3"].PutValue(2.5);
            worksheet.Cells["B3"].PutValue("2023-01-15");
            worksheet.Cells["A4"].PutValue("3");
            worksheet.Cells["B4"].PutValue(DateTime.Now.AddDays(1));

            // Создать параметры экспорта с включённым CheckMixedValueType
            ExportTableOptions options = new ExportTableOptions
            {
                CheckMixedValueType = true,
                ExportColumnName = true
            };

            // Экспортировать данные в DataTable
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 4, 2, options);

            // Отобразить результаты
            Console.WriteLine("Columns: " + dataTable.Columns.Count);
            Console.WriteLine("Rows: " + dataTable.Rows.Count);
            Console.WriteLine("ID column type: " + dataTable.Columns["ID"].DataType);
            Console.WriteLine("Value Date column type: " + dataTable.Columns["Value Date"].DataType);
        }
    }
}
```

### См. также

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


