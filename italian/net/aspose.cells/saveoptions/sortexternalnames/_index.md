---
title: "SaveOptions.SortExternalNames"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SaveOptions. Indica se ordinare i nomi definiti esternamente prima di salvare il file"
type: docs
url: /it/net/aspose.cells/saveoptions/sortexternalnames/
---
## SaveOptions.SortExternalNames property

Indica se ordinare i nomi definiti esterni prima di salvare il file.

```csharp
public bool SortExternalNames { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SaveOptionsPropertySortExternalNamesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Crea un foglio di lavoro di esempio
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati per rendere l'esempio significativo
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Crea un'istanza di OoxmlSaveOptions che eredita da SaveOptions
                OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();

                // Visualizza il valore predefinito della proprietà SortExternalNames
                Console.WriteLine("Default SortExternalNames value: " + saveOptions.SortExternalNames);

                // Imposta SortExternalNames su true
                saveOptions.SortExternalNames = true;
                Console.WriteLine("SortExternalNames set to: " + saveOptions.SortExternalNames);

                // Salva la cartella di lavoro con le opzioni di salvataggio specificate
                workbook.Save("SortExternalNamesDemo.xlsx", saveOptions);

                Console.WriteLine("Workbook saved with SortExternalNames enabled.");
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

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


