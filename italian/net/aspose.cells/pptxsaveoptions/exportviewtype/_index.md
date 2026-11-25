---
title: "PptxSaveOptions.ExportViewType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PptxSaveOptions. Ottiene e imposta il tipo di visualizzazione durante l'esportazione in PowerPoint. Il tipo di esportazione predefinito funziona come stampa"
type: docs
url: /it/net/aspose.cells/pptxsaveoptions/exportviewtype/
---
## PptxSaveOptions.ExportViewType property

Ottiene e imposta il tipo di visualizzazione durante l'esportazione in PowerPoint. Il tipo di esportazione predefinito funziona come stampa.

```csharp
public SlideViewType ExportViewType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slides;

namespace AsposeCellsExamples
{
    public class PptxSaveOptionsPropertyExportViewTypeDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // Imposta le opzioni di salvataggio PPTX con ExportViewType
            PptxSaveOptions saveOptions = new PptxSaveOptions();
            saveOptions.ExportViewType = SlideViewType.View;
            
            // Salva la cartella di lavoro come PPTX
            workbook.Save("output.pptx", saveOptions);
            
            Console.WriteLine("Workbook saved as PPTX with ExportViewType set to View");
        }
    }
}
```

### Vedi anche

* enum [SlideViewType](../../../aspose.cells.slides/slideviewtype/)
* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


