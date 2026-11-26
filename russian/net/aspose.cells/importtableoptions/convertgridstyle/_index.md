---
title: "ImportTableOptions.ConvertGridStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImportTableOptions. Указывает, применять ли стиль представления сетки к ячейкам"
type: docs
url: /ru/net/aspose.cells/importtableoptions/convertgridstyle/
---
## ImportTableOptions.ConvertGridStyle property

Указывает, применять ли стиль представления сетки к ячейкам.

```csharp
public bool ConvertGridStyle { get; set; }
```

### Примеры

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyConvertGridStyleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать примерные данные
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Product", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));
            dataTable.Rows.Add(101, "Laptop", 999.99m);
            dataTable.Rows.Add(102, "Monitor", 249.50m);

            // Установить параметры импорта с включённым ConvertGridStyle
            ImportTableOptions options = new ImportTableOptions();
            options.ConvertGridStyle = true; // This will apply grid styling to the imported data
            options.IsFieldNameShown = true;

            // Импортировать данные со стилем
            worksheet.Cells.ImportData(dataTable, 0, 0, options);

            // Сохранить результат
            workbook.Save("ImportWithGridStyle.xlsx");
        }
    }
}
```

### См. также

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


