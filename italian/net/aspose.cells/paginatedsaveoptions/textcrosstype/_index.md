---
title: "PaginatedSaveOptions.TextCrossType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PaginatedSaveOptions. Ottiene o imposta il tipo di visualizzazione del testo quando la larghezza del testo è maggiore della larghezza della cella"
type: docs
url: /it/net/aspose.cells/paginatedsaveoptions/textcrosstype/
---
## PaginatedSaveOptions.TextCrossType property

Ottiene o imposta il tipo di visualizzazione del testo quando la larghezza del testo supera quella della cella.

```csharp
public TextCrossType TextCrossType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyTextCrossTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta un testo lungo che attraverserà i confini delle celle
            worksheet.Cells["A1"].PutValue("This is a long text that will cross cell boundaries");
            worksheet.Cells["B1"].PutValue("Another cell content");
            
            // Imposta la larghezza della colonna per far attraversare il testo le celle
            worksheet.Cells.SetColumnWidth(0, 5);
            
            // Crea le opzioni di salvataggio PDF
            PdfSaveOptions options = new PdfSaveOptions();
            
            // Dimostra TextCrossType impostandolo su CrossKeep
            options.TextCrossType = TextCrossType.CrossKeep;
            
            // Salva la cartella di lavoro come PDF
            workbook.Save("TextCrossTypeDemo.pdf", options);
            
            Console.WriteLine("PDF saved with TextCrossType.CrossKeep setting");
        }
    }
}
```

### Vedi anche

* enum [TextCrossType](../../textcrosstype/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


