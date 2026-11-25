---
title: "Range.ExportDataTableAsString"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Range. Esporta i dati di questo intervallo in un oggetto DataTable"
type: docs
url: /it/net/aspose.cells/range/exportdatatableasstring/
---
## Range.ExportDataTableAsString method

Esporta i dati di questo intervallo in un oggetto DataTable.

```csharp
public DataTable ExportDataTableAsString()
```

### Valore di ritorno

Oggetto DataTable esportato.

### Osservazioni

Tutti i dati nella collezione [`Cells`](../../cells/) sono convertiti in stringhe.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class RangeMethodExportDataTableAsStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(25);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(30);

            // Ottieni l'intervallo che contiene i dati
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");

            try
            {
                // Chiama il metodo ExportDataTableAsString
                DataTable dataTable = range.ExportDataTableAsString();

                // Visualizza i dati esportati
                Console.WriteLine("Exported DataTable:");
                foreach (DataRow row in dataTable.Rows)
                {
                    Console.WriteLine($"{row[0]}, {row[1]}");
                }

                // Salva la cartella di lavoro
                workbook.Save("RangeMethodExportDataTableAsStringDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ExportDataTableAsString method: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


