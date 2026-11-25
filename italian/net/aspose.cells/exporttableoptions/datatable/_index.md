---
title: "ExportTableOptions.DataTable"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ExportTableOptions proprietà. Ottiene e imposta il DataTable a cui è assegnato il tipo di dati delle colonne"
type: docs
url: /it/net/aspose.cells/exporttableoptions/datatable/
---
## ExportTableOptions.DataTable property

Ottiene e imposta la DataTable a cui è assegnato il tipo di dati delle colonne.

```csharp
public DataTable DataTable { get; set; }
```

### Esempi

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyDataTableDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Aggiungi dati di esempio alle celle
            cells["A1"].PutValue("Column1");
            cells["B1"].PutValue("Column2");
            cells["A2"].PutValue(100);
            cells["B2"].PutValue("Text1");
            cells["A3"].PutValue(200);
            cells["B3"].PutValue("Text2");

            // Crea DataTable e definisci le colonne
            DataTable dt = new DataTable();
            dt.Columns.Add("NumericData", typeof(double));
            dt.Columns.Add("TextData", typeof(string));

            // Configura le opzioni di esportazione
            ExportTableOptions options = new ExportTableOptions();
            options.ExportColumnName = true;
            options.Indexes = new int[] { 0, 1 }; // Export both columns
            options.DataTable = dt;

            // Esporta i dati in DataTable
            cells.ExportDataTable(0, 0, 3, 2, options);

            // Visualizza i dati esportati
            Console.WriteLine("Exported DataTable:");
            foreach (DataRow row in dt.Rows)
            {
                Console.WriteLine($"{row["NumericData"]}, {row["TextData"]}");
            }
        }
    }
}
```

### Vedi anche

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


