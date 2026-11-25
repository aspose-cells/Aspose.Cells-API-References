---
title: "DocxSaveOptions.SaveElementType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DocxSaveOptions. Indica quali elementi devono essere salvati"
type: docs
url: /it/net/aspose.cells/docxsaveoptions/saveelementtype/
---
## DocxSaveOptions.SaveElementType property

Indica quali elementi devono essere salvati.

```csharp
public SaveElementType SaveElementType { get; set; }
```

### Esempi

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class DocxSaveOptionsPropertySaveElementTypeDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e aggiungi alcuni dati di esempio
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Demo Data");

            try
            {
                // Inizializza DocxSaveOptions
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // NOTA: La proprietà SaveElementType non è presente nella classe DocxSaveOptions
                // basato sul riflesso API fornito. Se esistesse, la leggeresti così:
                // var elementType = saveOptions.SaveElementType;
                // Console.WriteLine("SaveElementType: " + elementType);

                // Dimostra la lettura di una proprietà esistente: SaveAsEditableShaps
                Console.WriteLine("SaveAsEditableShaps (default): " + saveOptions.SaveAsEditableShaps);

                // Imposta la proprietà su true e visualizza il nuovo valore
                saveOptions.SaveAsEditableShaps = true;
                Console.WriteLine("SaveAsEditableShaps (after set): " + saveOptions.SaveAsEditableShaps);

                // Salva la cartella di lavoro come DOCX utilizzando le opzioni configurate
                workbook.Save("SaveElementTypeDemo.docx", saveOptions);
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### Vedi anche

* enum [SaveElementType](../../../aspose.cells.saving/saveelementtype/)
* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


