---
title: "ICellsDataTable.BeforeFirst"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ICellsDataTable. Sposta il cursore all'inizio di questo oggetto, appena prima della prima riga"
type: docs
url: /it/net/aspose.cells/icellsdatatable/beforefirst/
---
## ICellsDataTable.BeforeFirst method

Sposta il cursore all'inizio di questo oggetto, appena prima della prima riga.

```csharp
public void BeforeFirst()
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class ICellsDataTableMethodBeforeFirstDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea dati di esempio
            DataTable sourceTable = new DataTable("Employees");
            sourceTable.Columns.Add("Name", typeof(string));
            sourceTable.Columns.Add("Department", typeof(string));
            sourceTable.Rows.Add("John Doe", "Engineering");
            sourceTable.Rows.Add("Jane Smith", "Marketing");

            // Importa dati nel foglio di lavoro
            ImportTableOptions importOptions = new ImportTableOptions();
            importOptions.IsFieldNameShown = true;
            worksheet.Cells.ImportData(sourceTable, 0, 0, importOptions);

            // Ottieni ICellsDataTable esportando i dati dal foglio di lavoro
            ICellsDataTable dataTable = (ICellsDataTable)worksheet.Cells.ExportDataTable(0, 0, sourceTable.Rows.Count + 1, sourceTable.Columns.Count);

            try
            {
                // Reimposta il cursore all'inizio della tabella dati
                dataTable.BeforeFirst();

                Console.WriteLine("Reading data from ICellsDataTable:");
                while (dataTable.Next())
                {
                    Console.WriteLine(
                        $"Name: {dataTable[0]}, " +
                        $"Department: {dataTable[1]}");
                }

                // Dimostra il reset del cursore
                dataTable.BeforeFirst();
                Console.WriteLine("\nCursor reset. Reading data again:");
                while (dataTable.Next())
                {
                    Console.WriteLine(
                        $"Name: {dataTable["Name"]}, " +
                        $"Department: {dataTable["Department"]}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing BeforeFirst method: {ex.Message}");
            }

            workbook.Save("ICellsDataTableBeforeFirstDemo.xlsx");
        }
    }
}
```

### Vedi anche

* interface [ICellsDataTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


