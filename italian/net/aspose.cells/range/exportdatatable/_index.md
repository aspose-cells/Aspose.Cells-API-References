---
title: "Range.ExportDataTable"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Range. Esporta i dati di questo intervallo in un oggetto DataTable"
type: docs
url: /it/net/aspose.cells/range/exportdatatable/
---
## ExportDataTable() {#exportdatatable}

Esporta i dati di questo intervallo in un oggetto DataTable.

```csharp
public DataTable ExportDataTable()
```

### Valore di ritorno

Oggetto DataTable esportato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class RangeMethodExportDataTableDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea dati di esempio nel foglio di lavoro
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200.50);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(899.99);
            worksheet.Cells["A4"].PutValue("Tablet");
            worksheet.Cells["B4"].PutValue(450.75);

            // Crea un intervallo contenente i dati
            Aspose.Cells.Range dataRange = worksheet.Cells.CreateRange("A1:B4");

            try
            {
                // Esporta l'intervallo in DataTable
                DataTable dataTable = dataRange.ExportDataTable();

                Console.WriteLine("Data exported successfully to DataTable");
                Console.WriteLine($"DataTable contains {dataTable.Rows.Count} rows and {dataTable.Columns.Count} columns");

                // Visualizza i dati esportati
                foreach (DataRow row in dataTable.Rows)
                {
                    Console.WriteLine($"{row[0]}: {row[1]}");
                }

                // Modifica il DataTable e reimportalo se necessario
                dataTable.Rows[0]["Price"] = 1300.00;
                Console.WriteLine("\nModified first product price in DataTable to 1300.00");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error exporting data: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("RangeMethodExportDataTableDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ExportDataTable(ExportTableOptions) {#exportdatatable_1}

Esporta i dati di questo intervallo in un oggetto DataTable.

```csharp
public DataTable ExportDataTable(ExportTableOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| opzioni | ExportTableOptions | Le opzioni per esportare l'intervallo in DataTable. |

### Valore di ritorno

Oggetto DataTable esportato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Data;

namespace AsposeCellsExamples
{
    public class RangeMethodExportDataTableWithExportTableOptionsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea dati di esempio nel foglio di lavoro
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Assegna un nome all'intervallo contenente i nostri dati
            Aspose.Cells.Range namedRange = worksheet.Cells.CreateRange("A1:B3");
            namedRange.Name = "Names";

            // Esporta l'intervallo denominato in DataTable con opzioni
            ExportTableOptions options = new ExportTableOptions();
            options.ExportColumnName = true;
            DataTable dataTable = namedRange.ExportDataTable(options);

            // Visualizza i risultati
            Console.WriteLine("Exported DataTable:");
            foreach (DataRow row in dataTable.Rows)
            {
                Console.WriteLine($"{row["Name"]}, {row["Age"]}");
            }
        }
    }
}
```

### Vedi anche

* class [ExportTableOptions](../../exporttableoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


