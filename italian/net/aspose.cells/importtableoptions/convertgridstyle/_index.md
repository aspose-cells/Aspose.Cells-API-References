---
title: "ImportTableOptions.ConvertGridStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImportTableOptions. Indica se applicare lo stile della visualizzazione a griglia alle celle"
type: docs
url: /it/net/aspose.cells/importtableoptions/convertgridstyle/
---
## ImportTableOptions.ConvertGridStyle property

Indica se applicare lo stile della visualizzazione a griglia alle celle.

```csharp
public bool ConvertGridStyle { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea dati di esempio
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Product", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));
            dataTable.Rows.Add(101, "Laptop", 999.99m);
            dataTable.Rows.Add(102, "Monitor", 249.50m);

            // Imposta le opzioni di importazione con ConvertGridStyle abilitato
            ImportTableOptions options = new ImportTableOptions();
            options.ConvertGridStyle = true; // This will apply grid styling to the imported data
            options.IsFieldNameShown = true;

            // Importa dati con stile
            worksheet.Cells.ImportData(dataTable, 0, 0, options);

            // Salva il risultato
            workbook.Save("ImportWithGridStyle.xlsx");
        }
    }
}
```

### Vedi anche

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


