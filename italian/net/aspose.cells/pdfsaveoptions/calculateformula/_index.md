---
title: "PdfSaveOptions.CalculateFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PdfSaveOptions. Indica se calcolare le formule prima di salvare il file pdf"
type: docs
url: /it/net/aspose.cells/pdfsaveoptions/calculateformula/
---
## PdfSaveOptions.CalculateFormula property

Indica se calcolare le formule prima di salvare il file pdf.

```csharp
public bool CalculateFormula { get; set; }
```

### Osservazioni

Il valore predefinito è false.

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyCalculateFormulaDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio e formule
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta valori e formule
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // Crea le opzioni di salvataggio PDF con il calcolo delle formule
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.CalculateFormula = true;

            // Salva su stream di memoria
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, pdfSaveOptions);
                
                // Reimposta la posizione dello stream e verifica il contenuto
                stream.Position = 0;
                using (StreamReader reader = new StreamReader(stream))
                {
                    string content = reader.ReadToEnd();
                    Console.WriteLine("PDF contains formula results: " + content.Contains("30"));
                }
            }
        }
    }
}
```

### Vedi anche

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


