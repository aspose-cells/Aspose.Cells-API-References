---
title: "HtmlSaveOptions.ExportCommentsType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Rappresenta il tipo di esportazione dei commenti nei file HTML."
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/exportcommentstype/
---
## HtmlSaveOptions.ExportCommentsType property

Rappresenta il tipo di esportazione dei commenti nei file html.

```csharp
public PrintCommentsType ExportCommentsType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportCommentsTypeDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi un commento di esempio usando il nome della cella.
            Comment comment = worksheet.Comments["A1"];
            comment.Note = "This is a test comment";
            
            // Imposta le opzioni di salvataggio HTML con ExportCommentsType.
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportCommentsType = PrintCommentsType.PrintInPlace;
            
            // Salva in HTML
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML file with comments exported successfully.");
        }
    }
}
```

### Vedi anche

* enum [PrintCommentsType](../../printcommentstype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


