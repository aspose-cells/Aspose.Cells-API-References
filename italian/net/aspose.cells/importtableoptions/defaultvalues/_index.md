---
title: "ImportTableOptions.DefaultValues"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImportTableOptions. Il valore predefinito per il valore nella tabella è null"
type: docs
url: /it/net/aspose.cells/importtableoptions/defaultvalues/
---
## ImportTableOptions.DefaultValues property

Il valore predefinito per il valore nella tabella è null.

```csharp
public object[] DefaultValues { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class ImportTableOptionsPropertyDefaultValuesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea dati di esempio con valori null
            DataTable dataTable = new DataTable();
            dataTable.Columns.Add("Product", typeof(string));
            dataTable.Columns.Add("Quantity", typeof(int));
            dataTable.Columns.Add("ExpiryDate", typeof(DateTime));
            
            dataTable.Rows.Add("Bread", 10, DateTime.Now.AddDays(7));
            dataTable.Rows.Add(null, null, null); // Will use default values
            dataTable.Rows.Add("Milk", null, DateTime.Now.AddDays(3));

            ImportTableOptions importOptions = new ImportTableOptions();
            
            // Visualizza lo stato iniziale
            Console.WriteLine("Current DefaultValues: " + (importOptions.DefaultValues == null ? "Not set" : "Set"));

            // Configura i valori predefiniti per ogni colonna
            importOptions.DefaultValues = new object[] { "[Unspecified]", 1, DateTime.Today };

            // Importa i dati con gestione dei valori null
            worksheet.Cells.ImportData(dataTable, 0, 0, importOptions);

            // Adatta automaticamente le colonne per una migliore visibilità
            worksheet.AutoFitColumns();

            workbook.Save("DefaultValuesDemo.xlsx");
            Console.WriteLine("Spreadsheet saved with default values applied to null entries.");
        }
    }
}
```

### Vedi anche

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


