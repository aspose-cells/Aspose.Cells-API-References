---
title: "ImportTableOptions.ColumnIndexes"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImportTableOptions. Ottiene o imposta le colonne indicizzate da zero da importare dalla fonte dati. null indica che devono essere importate tutte le colonne"
type: docs
url: /it/net/aspose.cells/importtableoptions/columnindexes/
---
## ImportTableOptions.ColumnIndexes property

Ottiene o imposta le colonne (indice 0) da importare dalla fonte dati. null indica che tutte le colonne devono essere importate.

```csharp
public int[] ColumnIndexes { get; set; }
```

### Esempi

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyColumnIndexesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea un DataTable di esempio
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));
            
            // Aggiungi dati di esempio
            dataTable.Rows.Add(1, "Product A", 19.99m);
            dataTable.Rows.Add(2, "Product B", 29.99m);
            dataTable.Rows.Add(3, "Product C", 39.99m);

            // Imposta le opzioni di importazione per importare solo le colonne agli indici 0 e 2 (ID e Prezzo)
            ImportTableOptions options = new ImportTableOptions();
            options.ColumnIndexes = new int[] { 0, 2 };
            options.IsFieldNameShown = true;

            // Importa i dati con gli indici di colonna specificati
            worksheet.Cells.ImportData(dataTable, 0, 0, options);

            // Salva la cartella di lavoro
            workbook.Save("ColumnIndexesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


