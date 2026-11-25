---
title: "PptxSaveOptions.AdjustFontSizeForRowType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PptxSaveOptions. Rappresenta il tipo di linea il cui dimensione del carattere deve essere regolata se l'altezza della riga è piccola"
type: docs
url: /it/net/aspose.cells/pptxsaveoptions/adjustfontsizeforrowtype/
---
## PptxSaveOptions.AdjustFontSizeForRowType property

Rappresenta il tipo di linea di cui è necessario regolare la dimensione del carattere se l'altezza della riga è piccola.

```csharp
public AdjustFontSizeForRowType AdjustFontSizeForRowType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slides;

namespace AsposeCellsExamples
{
    public class PptxSaveOptionsPropertyAdjustFontSizeForRowTypeDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcuni dati e righe vuote
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data 1");
            worksheet.Cells["A3"].PutValue(""); // Empty row
            worksheet.Cells["A4"].PutValue("Data 2");
            
            // Crea le opzioni di salvataggio PPTX
            PptxSaveOptions saveOptions = new PptxSaveOptions();
            saveOptions.AdjustFontSizeForRowType = AdjustFontSizeForRowType.EmptyRows;
            
            // Salva in PPTX
            workbook.Save("output.pptx", saveOptions);
            
            Console.WriteLine("File saved with AdjustFontSizeForRowType setting");
        }
    }
}
```

### Vedi anche

* enum [AdjustFontSizeForRowType](../../../aspose.cells.slides/adjustfontsizeforrowtype/)
* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


