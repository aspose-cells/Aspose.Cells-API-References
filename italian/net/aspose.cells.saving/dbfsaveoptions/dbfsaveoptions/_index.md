---
title: "DbfSaveOptions.DbfSaveOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore DbfSaveOptions. Le opzioni per salvare il file .dbf"
type: docs
url: /it/net/aspose.cells.saving/dbfsaveoptions/dbfsaveoptions/
---
## DbfSaveOptions constructor

Le opzioni per il salvataggio del file .dbf.

```csharp
public DbfSaveOptions()
```

### Esempi

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
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            try
            {
                // Crea un'istanza di DbfSaveOptions usando il costruttore
                DbfSaveOptions saveOptions = new DbfSaveOptions();
                
                // Imposta le proprietà delle opzioni di salvataggio
                saveOptions.ExportAsString = true;
                
                // Salva la cartella di lavoro con le opzioni di salvataggio DBF
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

### Vedi anche

* class [DbfSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


