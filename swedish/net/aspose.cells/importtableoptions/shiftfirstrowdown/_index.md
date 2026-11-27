---
title: "ImportTableOptions.ShiftFirstRowDown"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImportTableOptions egenskap. Anger om den första raden ska flyttas nedåt vid infogning av rader"
type: docs
url: /sv/net/aspose.cells/importtableoptions/shiftfirstrowdown/
---
## ImportTableOptions.ShiftFirstRowDown property

Anger om den första raden ska flyttas nedåt vid infogning av rader.

```csharp
public bool ShiftFirstRowDown { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Skapa exempel på DataTable
            DataTable table = new DataTable();
            table.Columns.Add("Column1");
            table.Columns.Add("Column2");
            table.Rows.Add("Header1", "Header2");
            table.Rows.Add("Data1", "Data2");
            table.Rows.Add("Data3", "Data4");

            // Importera med ShiftFirstRowDown = false (standardbeteende)
            var options1 = new ImportTableOptions
            {
                IsFieldNameShown = false,
                ShiftFirstRowDown = false
            };
            cells.ImportData(table, 0, 0, options1);
            Console.WriteLine("With ShiftFirstRowDown=false, first row starts at A1: " + cells[0, 0].StringValue);

            // Rensa kalkylbladet och importera med ShiftFirstRowDown = true
            workbook.Worksheets[0].Cells.Clear();
            var options2 = new ImportTableOptions
            {
                IsFieldNameShown = false,
                ShiftFirstRowDown = true
            };
            cells.ImportData(table, 0, 0, options2);
            Console.WriteLine("With ShiftFirstRowDown=true, first row is shifted down to A2: " + cells[1, 0].StringValue);

            // Spara arbetsboken
            workbook.Save("ShiftFirstRowDownDemo.xlsx");
        }
    }
}
```

### Se även

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


