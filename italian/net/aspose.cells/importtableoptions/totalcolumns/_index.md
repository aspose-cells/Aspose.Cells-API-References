---
title: "ImportTableOptions.TotalColumns"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImportTableOptions. Ottiene o imposta il conteggio totale delle colonne da importare dalla fonte dati. 1 significa tutte le righe della fonte dati fornita"
type: docs
url: /it/net/aspose.cells/importtableoptions/totalcolumns/
---
## ImportTableOptions.TotalColumns property

Ottiene o imposta il conteggio totale delle colonne da importare dalla fonte dati. -1 indica tutte le righe della fonte dati fornita.

```csharp
public int TotalColumns { get; set; }
```

### Esempi

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyTotalColumnsDemo
    {
        public static void Run()
        {
            // Crea un DataTable di esempio
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));
            
            // Aggiungi dati di esempio
            dataTable.Rows.Add(1, "Product A", 19.99m);
            dataTable.Rows.Add(2, "Product B", 29.99m);

            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta le opzioni di importazione con TotalColumns = 2 (importerà solo le prime 2 colonne)
            ImportTableOptions importOptions = new ImportTableOptions
            {
                IsFieldNameShown = true,
                TotalColumns = 2 // Only import first 2 columns (ID and Name)
            };

            // Importa dati a partire dalla cella A1
            cells.ImportData(dataTable, 0, 0, importOptions);

            // Salva la cartella di lavoro
            workbook.Save("ImportWithTotalColumns.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("Data imported with TotalColumns=2. Only first 2 columns were imported.");
        }
    }
}
```

### Vedi anche

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


