---
title: "ImportTableOptions.ShiftFirstRowDown"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImportTableOptions. Указывает, следует ли сдвигать первую строку вниз при вставке строк."
type: docs
url: /ru/net/aspose.cells/importtableoptions/shiftfirstrowdown/
---
## ImportTableOptions.ShiftFirstRowDown property

Указывает, сдвигать ли первую строку вниз при вставке строк.

```csharp
public bool ShiftFirstRowDown { get; set; }
```

### Примеры

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyShiftFirstRowDownDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Создать пример DataTable
            DataTable table = new DataTable();
            table.Columns.Add("Column1");
            table.Columns.Add("Column2");
            table.Rows.Add("Header1", "Header2");
            table.Rows.Add("Data1", "Data2");
            table.Rows.Add("Data3", "Data4");

            // Импортировать с ShiftFirstRowDown = false (поведение по умолчанию).
            var options1 = new ImportTableOptions
            {
                IsFieldNameShown = false,
                ShiftFirstRowDown = false
            };
            cells.ImportData(table, 0, 0, options1);
            Console.WriteLine("With ShiftFirstRowDown=false, first row starts at A1: " + cells[0, 0].StringValue);

            // Очистить лист и импортировать с ShiftFirstRowDown = true.
            workbook.Worksheets[0].Cells.Clear();
            var options2 = new ImportTableOptions
            {
                IsFieldNameShown = false,
                ShiftFirstRowDown = true
            };
            cells.ImportData(table, 0, 0, options2);
            Console.WriteLine("With ShiftFirstRowDown=true, first row is shifted down to A2: " + cells[1, 0].StringValue);

            // Сохраните книгу
            workbook.Save("ShiftFirstRowDownDemo.xlsx");
        }
    }
}
```

### См. также

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


