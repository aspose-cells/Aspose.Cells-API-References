---
title: "PptxSaveOptions.IgnoreHiddenRows"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PptxSaveOptions. Indica se ignorare le righe nascoste durante la conversione da Excel a PowerPoint"
type: docs
url: /it/net/aspose.cells/pptxsaveoptions/ignorehiddenrows/
---
## PptxSaveOptions.IgnoreHiddenRows property

Indica se ignorare le righe nascoste durante la conversione da Excel a PowerPoint.

```csharp
public bool IgnoreHiddenRows { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PptxSaveOptionsPropertyIgnoreHiddenRowsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio e nascondi alcune righe
            worksheet.Cells["A1"].PutValue("Visible Row 1");
            worksheet.Cells["A2"].PutValue("Hidden Row");
            worksheet.Cells["A3"].PutValue("Visible Row 2");
            
            // Nascondi la riga 2
            worksheet.Cells.Rows[1].IsHidden = true;

            // Imposta le opzioni di salvataggio PPTX con IgnoreHiddenRows
            PptxSaveOptions saveOptions = new PptxSaveOptions();
            saveOptions.IgnoreHiddenRows = true;
            
            // Salva come PPTX
            workbook.Save("output.pptx", saveOptions);
            
            Console.WriteLine("PPTX saved with hidden rows ignored.");
        }
    }
}
```

### Vedi anche

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


