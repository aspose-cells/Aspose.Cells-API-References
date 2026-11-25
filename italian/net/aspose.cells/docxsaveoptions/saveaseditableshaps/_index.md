---
title: "DocxSaveOptions.SaveAsEditableShaps"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DocxSaveOptions. Salva tutti gli oggetti di disegno objecgts come forme modificabili nel file Word. Così puoi modificarli in Word"
type: docs
url: /it/net/aspose.cells/docxsaveoptions/saveaseditableshaps/
---
## DocxSaveOptions.SaveAsEditableShaps property

Salva tutti gli oggetti di disegno objecgts come forme modificabili nel file Word. Così puoi modificarli in Word.

```csharp
[Obsolete("Use SaveFormat.SaveAsEditableShapes instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool SaveAsEditableShaps { get; set; }
```

### Osservazioni

NOTE: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà [`SaveAsEditableShapes`](../saveaseditableshapes/). Questa proprietà sarà rimossa 6 mesi dopo, a partire da maggio 2025. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocxSaveOptionsPropertySaveAsEditableShapsDemo
    {
        public static void Run()
        {
            // Crea un oggetto workbook e apri il file Excel modello
            Workbook workbook = new Workbook("example.xlsx");

            // Inizializza DocxSaveOptions
            DocxSaveOptions saveOptions = new DocxSaveOptions();
            
            // Imposta la proprietà SaveAsEditableShaps su true
            saveOptions.SaveAsEditableShaps = true;

            // Salva il workbook come DOCX con le opzioni specificate
            workbook.Save("example.docx", saveOptions);
        }
    }
}
```

### Vedi anche

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


