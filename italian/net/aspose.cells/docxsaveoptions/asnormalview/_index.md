---
title: "DocxSaveOptions.AsNormalView"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DocxSaveOptions. Esporta il file Excel in docx fiel come visualizzazione normale. Se questa proprietà è true, verrà generata un'Area e nessuna scala avrà effetto. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/docxsaveoptions/asnormalview/
---
## DocxSaveOptions.AsNormalView property

Esportazione del file Excel in file docx in visualizzazione normale. Se questa proprietà è true, verrà generata un'Area e nessuna scala avrà effetto. Il valore predefinito è false.

```csharp
public bool AsNormalView { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DocxSaveOptionsPropertyAsNormalViewDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro e aggiungi dati di esempio
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Normal View Demo";

            try
            {
                // Inizializza DocxSaveOptions
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // Visualizza il valore predefinito della proprietà AsNormalView
                Console.WriteLine("Default AsNormalView value: " + saveOptions.AsNormalView);

                // Imposta AsNormalView su true per dimostrarne l'uso
                saveOptions.AsNormalView = true;
                Console.WriteLine("AsNormalView set to: " + saveOptions.AsNormalView);

                // Salva la cartella di lavoro come DOCX con le opzioni configurate
                workbook.Save("AsNormalViewDemo.docx", saveOptions);
                Console.WriteLine("Document saved successfully with AsNormalView option.");
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


