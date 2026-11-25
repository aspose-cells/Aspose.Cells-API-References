---
title: "PasteOptions.KeepOldTables"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PasteOptions. Mantiene le tabelle nell'intervallo di destinazione"
type: docs
url: /it/net/aspose.cells/pasteoptions/keepoldtables/
---
## PasteOptions.KeepOldTables property

Mantiene le tabelle nell'intervallo di destinazione.

```csharp
public bool KeepOldTables { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PasteOptionsPropertyKeepOldTablesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Crea un foglio di lavoro di esempio con dati
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Source Data";
            worksheet.Cells["B1"].Value = "Table Data";

            try
            {
                // Crea un'istanza di PasteOptions
                PasteOptions pasteOptions = new PasteOptions();

                // Visualizza il valore predefinito della proprietà KeepOldTables
                Console.WriteLine("Default KeepOldTables value: " + pasteOptions.KeepOldTables);

                // Imposta KeepOldTables su true
                pasteOptions.KeepOldTables = true;
                Console.WriteLine("KeepOldTables set to: " + pasteOptions.KeepOldTables);

                // Crea intervalli per l'operazione di copia
                Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1:B1");
                Aspose.Cells.Range targetRange = worksheet.Cells.CreateRange("A3:B3");

                // Copia con l'opzione KeepOldTables
                targetRange.Copy(sourceRange, pasteOptions);

                // Salva la cartella di lavoro
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

### Vedi anche

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


