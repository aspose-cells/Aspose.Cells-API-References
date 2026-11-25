---
title: "HtmlSaveOptions.EmbeddedFontType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Ottiene o imposta il tipo di incorporamento del file di carattere nel file html. Il valore predefinito è None, il che indica che nessun carattere sarà incorporato nell'html"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/embeddedfonttype/
---
## HtmlSaveOptions.EmbeddedFontType property

Ottiene o imposta il tipo di incorporamento del file font nel file html. Il valore predefinito è None, il che indica che nessun font sarà incorporato nell'html.

```csharp
public HtmlEmbeddedFontType EmbeddedFontType { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class HtmlSaveOptionsPropertyEmbeddedFontTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            worksheet.Cells["A1"].PutValue("Sample Text with Font");
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            worksheet.Cells["A1"].SetStyle(style);

            try
            {
                // Crea opzioni di salvataggio HTML
                HtmlSaveOptions options = new HtmlSaveOptions();

                // Visualizza il valore predefinito di EmbeddedFontType
                Console.WriteLine("Default EmbeddedFontType: " + options.EmbeddedFontType);

                // Imposta EmbeddedFontType su Woff
                options.EmbeddedFontType = HtmlEmbeddedFontType.Woff;
                Console.WriteLine("EmbeddedFontType set to: " + options.EmbeddedFontType);

                // Salva la cartella di lavoro con incorporamento del carattere WOFF
                workbook.Save("EmbeddedFontType_Woff.html", options);

                // Reimposta su None
                options.EmbeddedFontType = HtmlEmbeddedFontType.None;
                Console.WriteLine("EmbeddedFontType set to: " + options.EmbeddedFontType);

                // Salva la cartella di lavoro senza incorporamento del carattere
                workbook.Save("EmbeddedFontType_None.html", options);

                Console.WriteLine("EmbeddedFontType demonstration completed successfully.");
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

* enum [HtmlEmbeddedFontType](../../../aspose.cells.rendering/htmlembeddedfonttype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


