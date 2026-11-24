---
title: "PdfSaveOptions.CalculateFormula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PdfSaveOptions Eigenschaft. Gibt an, ob Formeln vor dem Speichern der PDF-Datei berechnet werden sollen"
type: docs
url: /de/net/aspose.cells/pdfsaveoptions/calculateformula/
---
## PdfSaveOptions.CalculateFormula property

Gibt an, ob Formeln vor dem Speichern der PDF‑Datei berechnet werden sollen.

```csharp
public bool CalculateFormula { get; set; }
```

### Hinweise

Der Standardwert ist false.

### Beispiele

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
            // Erstelle ein Arbeitsbuch mit Beispieldaten und Formeln
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Werte und Formeln festlegen
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // Erstelle PDF-Speicheroptionen mit Formelberechnung
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.CalculateFormula = true;

            // In den Speicherstream speichern
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, pdfSaveOptions);
                
                // Setze die Stream-Position zurück und überprüfe den Inhalt
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

### Siehe auch

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


