---
title: "DbfSaveOptions.DbfSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DbfSaveOptions‑konstruktor. Alternativen för att spara .dbf‑fil"
type: docs
url: /sv/net/aspose.cells.saving/dbfsaveoptions/dbfsaveoptions/
---
## DbfSaveOptions constructor

Alternativen för att spara .dbf‑fil.

```csharp
public DbfSaveOptions()
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class DbfSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            try
            {
                // Skapa en DbfSaveOptions‑instans med hjälp av konstruktorn
                DbfSaveOptions saveOptions = new DbfSaveOptions();
                
                // Ställ in egenskaper för sparalternativen
                saveOptions.ExportAsString = true;
                
                // Spara arbetsboken med DBF‑sparalternativ
                workbook.Save("DbfSaveOptionsDemo.dbf", saveOptions);
                
                Console.WriteLine("DBF file saved successfully with ExportAsString option set to true");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving DBF file: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [DbfSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


