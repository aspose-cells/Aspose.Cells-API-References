---
title: "ICellsDataTable.BeforeFirst"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ICellsDataTable metod. Flytta markören till början av detta objekt precis före den första raden"
type: docs
url: /sv/net/aspose.cells/icellsdatatable/beforefirst/
---
## ICellsDataTable.BeforeFirst method

Flytta markören till början av detta objekt, precis före den första raden.

```csharp
public void BeforeFirst()
```

### Exempel

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

            // Skapa exempeldata
            DataTable sourceTable = new DataTable("Employees");
            sourceTable.Columns.Add("Name", typeof(string));
            sourceTable.Columns.Add("Department", typeof(string));
            sourceTable.Rows.Add("John Doe", "Engineering");
            sourceTable.Rows.Add("Jane Smith", "Marketing");

            // Importera data till kalkylbladet
            ImportTableOptions importOptions = new ImportTableOptions();
            importOptions.IsFieldNameShown = true;
            worksheet.Cells.ImportData(sourceTable, 0, 0, importOptions);

            // Hämta ICellsDataTable genom att exportera data från kalkylbladet
            ICellsDataTable dataTable = (ICellsDataTable)worksheet.Cells.ExportDataTable(0, 0, sourceTable.Rows.Count + 1, sourceTable.Columns.Count);

            try
            {
                // Återställ markören till början av datatabellen
                dataTable.BeforeFirst();

                Console.WriteLine("Reading data from ICellsDataTable:");
                while (dataTable.Next())
                {
                    Console.WriteLine(
                        $"Name: {dataTable[0]}, " +
                        $"Department: {dataTable[1]}");
                }

                // Visa återställning av markör
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

### Se även

* interface [ICellsDataTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


