---
title: "ImportTableOptions.ConvertNumericData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImportTableOptions. Ottiene o imposta un valore che indica se il valore stringa deve essere convertito in valore numerico o data"
type: docs
url: /it/net/aspose.cells/importtableoptions/convertnumericdata/
---
## ImportTableOptions.ConvertNumericData property

Ottiene o imposta un valore che indica se la stringa deve essere convertita in valore numerico o data.

```csharp
public bool ConvertNumericData { get; set; }
```

### Esempi

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyConvertNumericDataDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Crea una tabella dati di esempio con valori numerici e stringa
            DataTable dt = new DataTable();
            dt.Columns.Add("Numbers");
            dt.Columns.Add("Text");
            dt.Rows.Add("123", "456");
            dt.Rows.Add("ABC", "DEF");

            // Ottieni le celle del primo foglio di lavoro
            Cells cells = workbook.Worksheets[0].Cells;

            // Crea opzioni di importazione con ConvertNumericData impostato su true
            ImportTableOptions options = new ImportTableOptions();
            options.ConvertNumericData = true;
            options.IsFieldNameShown = true;

            // Importa i dati con conversione numerica
            cells.ImportData(dt, 0, 0, options);

            // Visualizza i risultati
            Console.WriteLine("A2 (numeric converted): " + cells["A2"].Value + " - Type: " + cells["A2"].Type);
            Console.WriteLine("B2 (string remains): " + cells["B2"].StringValue + " - Type: " + cells["B2"].Type);
        }
    }
}
```

### Vedi anche

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


