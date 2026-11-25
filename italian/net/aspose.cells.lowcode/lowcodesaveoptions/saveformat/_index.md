---
title: "LowCodeSaveOptions.SaveFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LowCodeSaveOptions. Ottiene e imposta il formato di salvataggio per l'output. In generale, per processi specifici in modalità low‑code sono consentiti solo alcuni formati specifici. Si prega di specificare il formato corretto per il processo corrispondente, altrimenti potrebbero verificarsi risultati inattesi o addirittura eccezioni."
type: docs
url: /it/net/aspose.cells.lowcode/lowcodesaveoptions/saveformat/
---
## LowCodeSaveOptions.SaveFormat property

Ottiene e imposta il formato di salvataggio per l'output. In generale, per processi specifici in modalità low‑code, sono consentiti solo alcuni formati specifici. Si prega di specificare il formato corretto per il processo corrispondente, altrimenti potrebbero verificarsi risultati inattesi o addirittura eccezioni.

```csharp
public virtual SaveFormat SaveFormat { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsPropertySaveFormatDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);

            // Inizializza LowCodeSaveOptions con formati diversi
            LowCodeSaveOptions excelOptions = new LowCodeSaveOptions();
            LowCodeSaveOptions pdfOptions = new LowCodeSaveOptions();

            // Configura le opzioni di salvataggio di Excel
            excelOptions.SaveFormat = SaveFormat.Xlsx;
            excelOptions.OutputFile = "output_excel.xlsx";

            // Configura le opzioni di salvataggio PDF
            pdfOptions.SaveFormat = SaveFormat.Pdf;
            pdfOptions.OutputFile = "output_pdf.pdf";

            // Dimostra il salvataggio nel formato originale
            Console.WriteLine($"Saving as {excelOptions.SaveFormat}");
            workbook.Save(excelOptions.OutputFile, excelOptions.SaveFormat);

            // Dimostra il cambio di formato e il nuovo salvataggio
            Console.WriteLine($"Changing format to {pdfOptions.SaveFormat}");
            Console.WriteLine($"Saving as {pdfOptions.SaveFormat}");
            workbook.Save(pdfOptions.OutputFile, pdfOptions.SaveFormat);

            Console.WriteLine("Files saved successfully with different formats.");
        }
    }
}
```

### Vedi anche

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [LowCodeSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


