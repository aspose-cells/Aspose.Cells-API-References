---
title: "Range.ExportDataTable"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range-metod. Exporterar data i detta område till ett DataTable-objekt"
type: docs
url: /sv/net/aspose.cells/range/exportdatatable/
---
## ExportDataTable() {#exportdatatable}

Exporterar data i detta område till ett DataTable-objekt.

```csharp
public DataTable ExportDataTable()
```

### Returvärde

Exporterad DataTable‑objekt.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200.50);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(899.99);
            worksheet.Cells["A4"].PutValue("Tablet");
            worksheet.Cells["B4"].PutValue(450.75);

            // Skapa ett område som innehåller data
            Aspose.Cells.Range dataRange = worksheet.Cells.CreateRange("A1:B4");

            try
            {
                // Exportera området till DataTable
                DataTable dataTable = dataRange.ExportDataTable();

                Console.WriteLine("Data exported successfully to DataTable");
                Console.WriteLine($"DataTable contains {dataTable.Rows.Count} rows and {dataTable.Columns.Count} columns");

                // Visa den exporterade datan
                foreach (DataRow row in dataTable.Rows)
                {
                    Console.WriteLine($"{row[0]}: {row[1]}");
                }

                // Modifiera DataTable och importera tillbaka om det behövs
                dataTable.Rows[0]["Price"] = 1300.00;
                Console.WriteLine("\nModified first product price in DataTable to 1300.00");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error exporting data: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("RangeMethodExportDataTableDemo.xlsx");
        }
    }
}
```

### Se även

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ExportDataTable(ExportTableOptions) {#exportdatatable_1}

Exporterar data i detta område till ett DataTable-objekt.

```csharp
public DataTable ExportDataTable(ExportTableOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| alternativ | ExportTableOptions | Alternativen för att exportera område till DataTable. |

### Returvärde

Exporterad DataTable‑objekt.

### Exempel

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
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Namnge området som innehåller vår data
            Aspose.Cells.Range namedRange = worksheet.Cells.CreateRange("A1:B3");
            namedRange.Name = "Names";

            // Exportera det namngivna området till DataTable med alternativ
            ExportTableOptions options = new ExportTableOptions();
            options.ExportColumnName = true;
            DataTable dataTable = namedRange.ExportDataTable(options);

            // Visa resultaten
            Console.WriteLine("Exported DataTable:");
            foreach (DataRow row in dataTable.Rows)
            {
                Console.WriteLine($"{row["Name"]}, {row["Age"]}");
            }
        }
    }
}
```

### Se även

* class [ExportTableOptions](../../exporttableoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


