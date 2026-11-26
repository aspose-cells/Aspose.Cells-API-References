---
title: "SpreadsheetML2003SaveOptions.ExportColumnIndexOfCell"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SpreadsheetML2003SaveOptions. Значение по умолчанию — false, что означает, что индекс столбца будет игнорироваться, если ячейка смежна с предыдущей."
type: docs
url: /ru/net/aspose.cells/spreadsheetml2003saveoptions/exportcolumnindexofcell/
---
## SpreadsheetML2003SaveOptions.ExportColumnIndexOfCell property

Значение по умолчанию — false, это означает, что индекс столбца будет игнорироваться, если ячейка смежна с предыдущей.

```csharp
public bool ExportColumnIndexOfCell { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpreadsheetML2003SaveOptionsPropertyExportColumnIndexOfCellDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в ячейки
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            
            // Создайте параметры сохранения с включённым ExportColumnIndexOfCell.
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions();
            saveOptions.ExportColumnIndexOfCell = true;
            
            // Сохраните книгу с информацией об индексе столбца.
            workbook.Save("output_with_column_index.xml", saveOptions);
            
            Console.WriteLine("File saved with column index information.");
        }
    }
}
```

### См. также

* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


