---
title: "PptxSaveOptions.AsFlatOpc"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PptxSaveOptions. Indica se salvare come file OPC piatto che può essere generato da Open XML SDK"
type: docs
url: /it/net/aspose.cells/pptxsaveoptions/asflatopc/
---
## PptxSaveOptions.AsFlatOpc property

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

    public class PptxSaveOptionsPropertyAsFlatOpcDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Crea un foglio di lavoro di esempio
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati per rendere l'esempio significativo
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["A2"].Value = "Flat OPC Demo";

            try
            {
                // Crea un'istanza di PptxSaveOptions
                PptxSaveOptions saveOptions = new PptxSaveOptions();

                // Mostra il valore predefinito di AsFlatOpc
                Console.WriteLine("Default AsFlatOpc value: " + saveOptions.AsFlatOpc);

                // Imposta la proprietà su true per dimostrarne l'uso
                saveOptions.AsFlatOpc = true;
                Console.WriteLine("AsFlatOpc set to: " + saveOptions.AsFlatOpc);

                // Salva la cartella di lavoro come PPTX con l'opzione abilitata
                workbook.Save("AsFlatOpcDemo.pptx", saveOptions);

                Console.WriteLine("PPTX saved with AsFlatOpc enabled");
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

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


