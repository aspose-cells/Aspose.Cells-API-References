---
title: "HtmlSaveOptions.DisableDownlevelRevealedComments"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se disabilitare i commenti condizionali Downlevelrevealed durante l'esportazione del file in HTML; il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/disabledownlevelrevealedcomments/
---
## HtmlSaveOptions.DisableDownlevelRevealedComments property

Indica se disabilitare i commenti condizionali Downlevel-revealed durante l'esportazione del file in html, il valore predefinito è false.

```csharp
public bool DisableDownlevelRevealedComments { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyDisableDownlevelRevealedCommentsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di esempio con un commento
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Comment comment = worksheet.Comments[worksheet.Comments.Add("A1")];
            comment.Note = "This is a test comment";

            // Imposta le opzioni di salvataggio HTML con DisableDownlevelRevealedComments
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.DisableDownlevelRevealedComments = true;

            // Salva la cartella di lavoro con le opzioni HTML
            workbook.Save("output.html", options);
            
            Console.WriteLine("Workbook saved with DisableDownlevelRevealedComments=true");
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


