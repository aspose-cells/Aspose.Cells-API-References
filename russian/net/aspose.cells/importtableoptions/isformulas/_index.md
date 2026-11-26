---
title: "ImportTableOptions.IsFormulas"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImportTableOptions. Указывает, являются ли данные формулами"
type: docs
url: /ru/net/aspose.cells/importtableoptions/isformulas/
---
## ImportTableOptions.IsFormulas property

Указывает, являются ли данные формулами.

```csharp
public bool[] IsFormulas { get; set; }
```

### Примеры

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyIsFormulasDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Создать пример таблицы данных с формульным содержимым
            DataTable dt = new DataTable();
            dt.Columns.Add("Column1");
            dt.Rows.Add("=SUM(1,2,3)");
            dt.Rows.Add("=AVERAGE(4,5,6)");

            // Установить параметры импорта с свойством IsFormulas
            ImportTableOptions options = new ImportTableOptions();
            options.IsFormulas = new bool[] { true }; // Treat first column as formulas
            
            // Импортировать данные с формулами
            workbook.Worksheets[0].Cells.ImportData(dt, 0, 0, options);

            // Проверить, что формулы были импортированы корректно
            Console.WriteLine("Cell A1 formula: " + workbook.Worksheets[0].Cells["A1"].Formula);
            Console.WriteLine("Cell A2 formula: " + workbook.Worksheets[0].Cells["A2"].Formula);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


