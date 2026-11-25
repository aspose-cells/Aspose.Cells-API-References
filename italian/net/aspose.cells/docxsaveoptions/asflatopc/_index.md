---
title: "DocxSaveOptions.AsFlatOpc"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DocxSaveOptions. Indica se il salvataggio avviene come file flat opc che può essere generato da Open XML SDK"
type: docs
url: /it/net/aspose.cells/docxsaveoptions/asflatopc/
---
## DocxSaveOptions.AsFlatOpc property

Indica se salvare come file OPC piatto che può essere generato da Open XML SDK

```csharp
public bool AsFlatOpc { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DocxSaveOptionsPropertyAsFlatOpcDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro e aggiungi dati di esempio
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Flat OPC Demo";

            try
            {
                // Inizializza DocxSaveOptions
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // Visualizza il valore predefinito della proprietà AsFlatOpc
                Console.WriteLine("Default AsFlatOpc value: " + saveOptions.AsFlatOpc);

                // Imposta AsFlatOpc su true per dimostrare il suo utilizzo
                saveOptions.AsFlatOpc = true;
                Console.WriteLine("AsFlatOpc set to: " + saveOptions.AsFlatOpc);

                // Salva la cartella di lavoro come DOCX con le opzioni configurate
                workbook.Save("AsFlatOpcDemo.docx", saveOptions);
                Console.WriteLine("Document saved successfully with AsFlatOpc option.");
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


