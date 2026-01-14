---
title: PasteOptions.KeepOldTables
second_title: Aspose.Cells for .NET API Reference
description: PasteOptions property. Keeps the tables in the destination range
type: docs
url: /net/aspose.cells/pasteoptions/keepoldtables/
---
## PasteOptions.KeepOldTables property

Keeps the tables in the destination range.

```csharp
public bool KeepOldTables { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PasteOptionsPropertyKeepOldTablesDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Create a sample worksheet with data
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Source Data";
            worksheet.Cells["B1"].Value = "Table Data";

            try
            {
                // Create a PasteOptions instance
                PasteOptions pasteOptions = new PasteOptions();

                // Display the default value of KeepOldTables property
                Console.WriteLine("Default KeepOldTables value: " + pasteOptions.KeepOldTables);

                // Set KeepOldTables to true
                pasteOptions.KeepOldTables = true;
                Console.WriteLine("KeepOldTables set to: " + pasteOptions.KeepOldTables);

                // Create ranges for copy operation
                Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1:B1");
                Aspose.Cells.Range targetRange = worksheet.Cells.CreateRange("A3:B3");

                // Copy with KeepOldTables option
                targetRange.Copy(sourceRange, pasteOptions);

                // Save the workbook
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

### See Also

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


