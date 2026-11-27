---
title: "DbfLoadOptions.DbfLoadOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DbfLoadOptions‑konstruktor. Alternativen"
type: docs
url: /sv/net/aspose.cells.loading/dbfloadoptions/dbfloadoptions/
---
## DbfLoadOptions constructor

Alternativen.

```csharp
public DbfLoadOptions()
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Loading;
    using System;

    public class DbfLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            try
            {
                // Skapa en DbfLoadOptions‑instans med #ctor‑metoden
                DbfLoadOptions loadOptions = new DbfLoadOptions();

                // Skapa arbetsbok med DBF-laddningsalternativ
                Workbook workbook = new Workbook("sample.dbf", loadOptions);

                // Åtkomst till det första kalkylbladet
                Worksheet worksheet = workbook.Worksheets[0];

                // Visa viss data från den inlästa DBF‑filen
                Console.WriteLine("Data loaded from DBF file:");
                Console.WriteLine(worksheet.Cells["A1"].StringValue);

                // Spara arbetsboken i Excel-format
                workbook.Save("DbfLoadOptionsCtorDemo.xlsx", SaveFormat.Xlsx);
                Console.WriteLine("File saved successfully with DBF data");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing DbfLoadOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [DbfLoadOptions](../)
* namespace [Aspose.Cells.Loading](../../../aspose.cells.loading/)
* assembly [Aspose.Cells](../../../)


