---
title: "LowCodeSplitOptions.SaveOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LowCodeSplitOptions. Opzioni di salvataggio per salvare le parti suddivise"
type: docs
url: /it/net/aspose.cells.lowcode/lowcodesplitoptions/saveoptions/
---
## LowCodeSplitOptions.SaveOptions property

Opzioni di salvataggio per salvare le parti divise.

```csharp
public LowCodeSaveOptions SaveOptions { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSplitOptionsPropertySaveOptionsDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e aggiungi dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");

            // Crea un'istanza di LowCodeSplitOptions
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();

            // Mostra il valore iniziale di SaveOptions (null per impostazione predefinita)
            Console.WriteLine("Initial SaveOptions value: " + (splitOptions.SaveOptions == null ? "null" : splitOptions.SaveOptions.ToString()));

            // Crea e configura LowCodeSaveOptions per il formato PDF
            LowCodeSaveOptions pdfSaveOptions = new LowCodeSaveOptions();
            pdfSaveOptions.SaveFormat = SaveFormat.Pdf;

            // Assegna le opzioni di salvataggio a SplitOptions
            splitOptions.SaveOptions = pdfSaveOptions;

            // Mostra il valore aggiornato di SaveOptions
            Console.WriteLine("Updated SaveOptions SaveFormat: " + splitOptions.SaveOptions.SaveFormat);

            // Scenario di utilizzo di esempio: la suddivisione della cartella di lavoro salverebbe le parti in PDF
            // (Il codice effettivo di divisione dipenderebbe dall'implementazione dell'API Aspose.Cells.LowCode)
            // LowCodeEngine.Split(workbook, splitOptions, "output_directory/");
            
            // Salva la cartella di lavoro originale per la dimostrazione (non influenzata da SplitOptions)
            workbook.Save("LowCodeSplitOptionsPropertySaveOptionsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [LowCodeSplitOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


