---
title: "ImportTableOptions.ShiftFirstRowDown"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImportTableOptions. Indica se spostare verso il basso la prima riga durante l'inserimento delle righe"
type: docs
url: /it/net/aspose.cells/importtableoptions/shiftfirstrowdown/
---
## ImportTableOptions.ShiftFirstRowDown property

Indica se spostare verso il basso la prima riga durante l'inserimento di righe.

```csharp
public bool ShiftFirstRowDown { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Crea un DataTable di esempio
            DataTable table = new DataTable();
            table.Columns.Add("Column1");
            table.Columns.Add("Column2");
            table.Rows.Add("Header1", "Header2");
            table.Rows.Add("Data1", "Data2");
            table.Rows.Add("Data3", "Data4");

            // Importa con ShiftFirstRowDown = false (comportamento predefinito)
            var options1 = new ImportTableOptions
            {
                IsFieldNameShown = false,
                ShiftFirstRowDown = false
            };
            cells.ImportData(table, 0, 0, options1);
            Console.WriteLine("With ShiftFirstRowDown=false, first row starts at A1: " + cells[0, 0].StringValue);

            // Cancella il foglio di lavoro e importa con ShiftFirstRowDown = true
            workbook.Worksheets[0].Cells.Clear();
            var options2 = new ImportTableOptions
            {
                IsFieldNameShown = false,
                ShiftFirstRowDown = true
            };
            cells.ImportData(table, 0, 0, options2);
            Console.WriteLine("With ShiftFirstRowDown=true, first row is shifted down to A2: " + cells[1, 0].StringValue);

            // Salva la cartella di lavoro
            workbook.Save("ShiftFirstRowDownDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


