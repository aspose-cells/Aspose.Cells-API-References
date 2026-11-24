---
title: "ICellsDataTable.BeforeFirst"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ICellsDataTable-Methode. Bewegt den Cursor an den Anfang dieses Objekts, direkt vor die erste Zeile"
type: docs
url: /de/net/aspose.cells/icellsdatatable/beforefirst/
---
## ICellsDataTable.BeforeFirst method

Bewege den Cursor an den Anfang dieses Objekts, direkt vor die erste Zeile.

```csharp
public void BeforeFirst()
```

### Beispiele

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

            // Erstelle Beispieldaten
            DataTable sourceTable = new DataTable("Employees");
            sourceTable.Columns.Add("Name", typeof(string));
            sourceTable.Columns.Add("Department", typeof(string));
            sourceTable.Rows.Add("John Doe", "Engineering");
            sourceTable.Rows.Add("Jane Smith", "Marketing");

            // Daten in Arbeitsblatt importieren
            ImportTableOptions importOptions = new ImportTableOptions();
            importOptions.IsFieldNameShown = true;
            worksheet.Cells.ImportData(sourceTable, 0, 0, importOptions);

            // ICellsDataTable durch Exportieren der Daten aus dem Arbeitsblatt erhalten
            ICellsDataTable dataTable = (ICellsDataTable)worksheet.Cells.ExportDataTable(0, 0, sourceTable.Rows.Count + 1, sourceTable.Columns.Count);

            try
            {
                // Cursor auf den Anfang der Datentabelle zurücksetzen
                dataTable.BeforeFirst();

                Console.WriteLine("Reading data from ICellsDataTable:");
                while (dataTable.Next())
                {
                    Console.WriteLine(
                        $"Name: {dataTable[0]}, " +
                        $"Department: {dataTable[1]}");
                }

                // Cursor-Reset demonstrieren
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

### Siehe auch

* interface [ICellsDataTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


