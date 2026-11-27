---
title: "PasteOptions.KeepOldTables"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PasteOptions-egenskap. Behåller tabellerna i destinationsområdet"
type: docs
url: /sv/net/aspose.cells/pasteoptions/keepoldtables/
---
## PasteOptions.KeepOldTables property

Behåller tabellerna i målintervallet.

```csharp
public bool KeepOldTables { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PasteOptionsPropertyKeepOldTablesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Skapa ett exempelark med data
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Source Data";
            worksheet.Cells["B1"].Value = "Table Data";

            try
            {
                // Skapa en PasteOptions-instans
                PasteOptions pasteOptions = new PasteOptions();

                // Visa standardvärdet för KeepOldTables-egenskapen
                Console.WriteLine("Default KeepOldTables value: " + pasteOptions.KeepOldTables);

                // Ställ in KeepOldTables till true
                pasteOptions.KeepOldTables = true;
                Console.WriteLine("KeepOldTables set to: " + pasteOptions.KeepOldTables);

                // Skapa områden för kopieringsoperationen
                Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1:B1");
                Aspose.Cells.Range targetRange = worksheet.Cells.CreateRange("A3:B3");

                // Kopiera med KeepOldTables-alternativet
                targetRange.Copy(sourceRange, pasteOptions);

                // Spara arbetsboken
                workbook.Save("KeepOldTablesDemo.xlsx");
                Console.WriteLine("Workbook saved with KeepOldTables option applied.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


