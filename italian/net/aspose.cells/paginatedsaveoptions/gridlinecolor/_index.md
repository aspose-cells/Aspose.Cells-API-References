---
title: "PaginatedSaveOptions.GridlineColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PaginatedSaveOptions. Ottiene o imposta il colore della linea della griglia"
type: docs
url: /it/net/aspose.cells/paginatedsaveoptions/gridlinecolor/
---
## PaginatedSaveOptions.GridlineColor property

Ottiene o imposta il colore della griglia.

```csharp
public Color GridlineColor { get; set; }
```

### Osservazioni

Ignorerà le impostazioni del colore della linea della griglia nel file di origine.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class PaginatedSaveOptionsPropertyGridlineColorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            worksheet.Cells["A1"].Value = "Gridline Color Demo";
            worksheet.Cells["A2"].Value = "Sample Data";

            try
            {
                // Crea le opzioni di salvataggio PDF
                PdfSaveOptions options = new PdfSaveOptions();

                // Visualizza il valore predefinito di GridlineColor
                Console.WriteLine("Default GridlineColor: " + options.GridlineColor);

                // Imposta un nuovo colore della linea della griglia
                options.GridlineColor = Color.Red;

                // Visualizza il valore aggiornato di GridlineColor
                Console.WriteLine("Updated GridlineColor: " + options.GridlineColor);

                // Salva la cartella di lavoro con l'impostazione del colore della linea della griglia
                workbook.Save("GridlineColorDemo.pdf", options);

                Console.WriteLine("PDF saved with custom gridline color.");
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

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


