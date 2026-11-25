---
title: "DocxSaveOptions.SaveAsEditableShapes"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DocxSaveOptions. Salva tutti gli oggetti di disegno come forme modificabili nel file Word così da poterli modificare in Word"
type: docs
url: /it/net/aspose.cells/docxsaveoptions/saveaseditableshapes/
---
## DocxSaveOptions.SaveAsEditableShapes property

Salva tutti gli oggetti di disegno come forme modificabili nel file Word, così puoi modificarli in Word.

```csharp
public bool SaveAsEditableShapes { get; set; }
```

### Osservazioni

Solo per i grafici.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DocxSaveOptionsPropertySaveAsEditableShapesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro e aggiungi dati di esempio
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Editable Shapes Demo";

            try
            {
                // Inizializza DocxSaveOptions
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // Visualizza il valore predefinito della proprietà SaveAsEditableShapes
                Console.WriteLine("Default SaveAsEditableShapes value: " + saveOptions.SaveAsEditableShapes);

                // Imposta SaveAsEditableShapes su true per dimostrarne l'uso
                saveOptions.SaveAsEditableShapes = true;
                Console.WriteLine("SaveAsEditableShapes set to: " + saveOptions.SaveAsEditableShapes);

                // Salva la cartella di lavoro come DOCX con le opzioni configurate
                workbook.Save("SaveAsEditableShapesDemo.docx", saveOptions);
                Console.WriteLine("Document saved successfully with SaveAsEditableShapes option.");
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

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


