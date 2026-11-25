---
title: "ImportTableOptions.DateFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImportTableOptions. Ottiene o imposta la stringa di formato data per le celle con valori datetime importati"
type: docs
url: /it/net/aspose.cells/importtableoptions/dateformat/
---
## ImportTableOptions.DateFormat property

Ottiene o imposta la stringa di formato data per le celle con valori datetime importati.

```csharp
public string DateFormat { get; set; }
```

### Esempi

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyDateFormatDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un DataTable di esempio con valori di data
            DataTable dataTable = new DataTable();
            dataTable.Columns.Add("DateColumn", typeof(DateTime));
            dataTable.Rows.Add(new DateTime(2023, 1, 15));
            dataTable.Rows.Add(new DateTime(2023, 2, 20));
            dataTable.Rows.Add(new DateTime(2023, 3, 25));

            // Definisci l'intervallo di importazione
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 10, 1);

            // Importa i dati con formato data personalizzato
            worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions()
            {
                IsFieldNameShown = true,
                DateFormat = "YYYY-MM-DD"
            });

            // Salvare la cartella di lavoro per dimostrare il risultato
            workbook.Save("DateFormatDemoOutput.xlsx");
        }
    }
}
```

### Vedi anche

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


