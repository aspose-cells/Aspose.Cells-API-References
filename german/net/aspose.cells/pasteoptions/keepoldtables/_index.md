---
title: "PasteOptions.KeepOldTables"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PasteOptions-Eigenschaft. Behält die Tabellen im Zielbereich bei"
type: docs
url: /de/net/aspose.cells/pasteoptions/keepoldtables/
---
## PasteOptions.KeepOldTables property

Behält die Tabellen im Zielbereich bei.

```csharp
public bool KeepOldTables { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PasteOptionsPropertyKeepOldTablesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Erstelle ein Beispielarbeitsblatt mit Daten
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Source Data";
            worksheet.Cells["B1"].Value = "Table Data";

            try
            {
                // Erstelle eine PasteOptions‑Instanz
                PasteOptions pasteOptions = new PasteOptions();

                // Zeige den Standardwert der KeepOldTables‑Eigenschaft an
                Console.WriteLine("Default KeepOldTables value: " + pasteOptions.KeepOldTables);

                // Setze KeepOldTables auf true
                pasteOptions.KeepOldTables = true;
                Console.WriteLine("KeepOldTables set to: " + pasteOptions.KeepOldTables);

                // Erstelle Bereiche für die Kopieroperation
                Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1:B1");
                Aspose.Cells.Range targetRange = worksheet.Cells.CreateRange("A3:B3");

                // Kopiere mit der KeepOldTables‑Option
                targetRange.Copy(sourceRange, pasteOptions);

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


