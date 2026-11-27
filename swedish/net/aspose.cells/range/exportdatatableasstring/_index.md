---
title: "Range.ExportDataTableAsString"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range-metod. Exporterar data i detta område till ett DataTable-objekt"
type: docs
url: /sv/net/aspose.cells/range/exportdatatableasstring/
---
## Range.ExportDataTableAsString method

Exporterar data i detta område till ett DataTable-objekt.

```csharp
public DataTable ExportDataTableAsString()
```

### Returvärde

Exporterad DataTable‑objekt.

### Anmärkningar

All data i [`Cells`](../../cells/) samlingen konverteras till strängar.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(25);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(30);

            // Hämta området som innehåller data
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");

            try
            {
                // Anropa metoden ExportDataTableAsString
                DataTable dataTable = range.ExportDataTableAsString();

                // Visa den exporterade datan
                Console.WriteLine("Exported DataTable:");
                foreach (DataRow row in dataTable.Rows)
                {
                    Console.WriteLine($"{row[0]}, {row[1]}");
                }

                // Spara arbetsboken
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

### Se även

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


