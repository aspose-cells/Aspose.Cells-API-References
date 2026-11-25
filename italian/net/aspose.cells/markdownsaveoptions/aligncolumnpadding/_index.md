---
title: "MarkdownSaveOptions.AlignColumnPadding"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MarkdownSaveOptions. Indica se l'allineamento delle colonne è abilitato per le tabelle Markdown generate. Quando abilitato, le colonne sono allineate riempiendo il contenuto delle celle con il carattere specificato, tipicamente uno spazio. Impostare a 0 per disabilitare l'allineamento delle colonne (valore predefinito)."
type: docs
url: /it/net/aspose.cells/markdownsaveoptions/aligncolumnpadding/
---
## MarkdownSaveOptions.AlignColumnPadding property

Indica se l'allineamento delle colonne è abilitato per le tabelle Markdown generate. Quando abilitato, le colonne sono allineate riempiendo il contenuto delle celle con il carattere specificato (tipicamente ' ' per gli spazi). Impostare su '\0' per disabilitare l'allineamento delle colonne (predefinito).

```csharp
public char AlignColumnPadding { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyAlignColumnPaddingDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per dimostrare l'allineamento delle colonne
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["C1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = "1.99";
            worksheet.Cells["C2"].Value = "10";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["B3"].Value = "0.99";
            worksheet.Cells["C3"].Value = "20";

            // Crea un'istanza di MarkdownSaveOptions
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

            try
            {
                // Visualizza il valore predefinito di AlignColumnPadding
                Console.WriteLine("Default AlignColumnPadding value: '" +
                    saveOptions.AlignColumnPadding + "'");

                // Imposta AlignColumnPadding sul carattere spazio per l'allineamento delle colonne
                saveOptions.AlignColumnPadding = ' ';

                // Visualizza il valore aggiornato
                Console.WriteLine("Updated AlignColumnPadding value: '" +
                    saveOptions.AlignColumnPadding + "'");

                // Salva la cartella di lavoro come markdown con allineamento delle colonne
                workbook.Save("AlignColumnPaddingDemo.md", saveOptions);
                Console.WriteLine("Markdown file saved with column alignment enabled.");
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

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


