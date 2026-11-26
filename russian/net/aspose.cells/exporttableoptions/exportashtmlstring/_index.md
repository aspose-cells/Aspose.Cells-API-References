---
title: "ExportTableOptions.ExportAsHtmlString"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExportTableOptions. Экспортирует HTML-строку значения ячеек в DataTable"
type: docs
url: /ru/net/aspose.cells/exporttableoptions/exportashtmlstring/
---
## ExportTableOptions.ExportAsHtmlString property

Экспортирует строковое значение HTML ячеек в DataTable.

```csharp
public bool ExportAsHtmlString { get; set; }
```

### Примеры

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyExportAsHtmlStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Установить значение ячейки с форматированием
            cells["A1"].PutValue("abc");
            Style style = cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 10;
            style.Font.Color = System.Drawing.Color.Black;
            cells["A1"].SetStyle(style);

            // Экспортировать с ExportAsHtmlString
            ExportTableOptions etOpt = new ExportTableOptions();
            etOpt.ExportColumnName = false;
            etOpt.ExportAsHtmlString = true;
            
            DataTable dt = cells.ExportDataTable(0, 0, 1, 1, etOpt);
            
            Console.WriteLine("HTML String: " + dt.Rows[0][0].ToString());
            Console.WriteLine("Expected Format: " + cells["A1"].HtmlString);
        }
    }
}
```

### См. также

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


