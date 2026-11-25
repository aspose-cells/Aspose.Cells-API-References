---
title: "Classe LowCodePdfSaveOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.LowCode.LowCodePdfSaveOptions. Opzioni per salvare PDF in modalità low‑code"
type: docs
url: /it/net/aspose.cells.lowcode/lowcodepdfsaveoptions/
---
## LowCodePdfSaveOptions class

Opzioni per salvare PDF in modalità low code.

```csharp
public class LowCodePdfSaveOptions : LowCodeSaveOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [LowCodePdfSaveOptions](lowcodepdfsaveoptions/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [OutputFile](../../aspose.cells.lowcode/lowcodesaveoptions/outputfile/) { get; set; } | Ottiene e imposta il file (con percorso se necessario) per salvare i dati generati. Quando si imposta questa proprietà con un valore diverso da null o stringa vuota, [`OutputStream`](../lowcodesaveoptions/outputstream/) verrà ignorato. (Ereditato da [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| [OutputStream](../../aspose.cells.lowcode/lowcodesaveoptions/outputstream/) { get; set; } | Ottiene e imposta lo Stream per scrivere i dati generati. Quando si imposta questa proprietà con un valore diverso da null, [`OutputFile`](../lowcodesaveoptions/outputfile/) verrà ignorato. (Ereditato da [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| [PdfOptions](../../aspose.cells.lowcode/lowcodepdfsaveoptions/pdfoptions/) { get; set; } | Le opzioni per salvare il file PDF. |
| override [SaveFormat](../../aspose.cells.lowcode/lowcodepdfsaveoptions/saveformat/) { get; set; } | Il formato di salvataggio per l'output. Per la conversione in PDF, può essere solo PDF. |

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class LowCodeClassLowCodePdfSaveOptionsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");

            // Crea le opzioni di salvataggio PDF
            PdfSaveOptions pdfOptions = new PdfSaveOptions();
            pdfOptions.Compliance = PdfCompliance.PdfA1b;

            // Crea opzioni di salvataggio PDF low‑code
            LowCodePdfSaveOptions lowCodePdfOptions = new LowCodePdfSaveOptions()
            {
                OutputFile = "output.pdf",
                PdfOptions = pdfOptions
            };

            // Salva usando le opzioni low‑code
            workbook.Save(lowCodePdfOptions.OutputFile, lowCodePdfOptions.PdfOptions);

            Console.WriteLine("File saved successfully with LowCodePdfSaveOptions");
        }
    }
}
```

### Vedi anche

* class [LowCodeSaveOptions](../lowcodesaveoptions/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


