---
title: "PdfSaveOptions.Producer"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PdfSaveOptions property. Ottiene e imposta il produttore del documento pdf generato"
type: docs
url: /it/net/aspose.cells/pdfsaveoptions/producer/
---
## PdfSaveOptions.Producer property

Ottiene o imposta il produttore del documento pdf generato.

```csharp
public string Producer { get; set; }
```

### Osservazioni

Se il valore è null, o una LICENSE valida non è impostata, verrà utilizzata la stringa Aspose.Cells vVERSION.

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyProducerDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro e aggiungi dati di esempio
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("PDF Producer Property Demo");

            // Crea le opzioni di salvataggio PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Imposta la proprietà Producer
            pdfSaveOptions.Producer = "Aspose.Cells for .NET";
            
            // Salva su stream di memoria
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, pdfSaveOptions);
                
                // Verifica che la proprietà Producer sia stata impostata
                stream.Position = 0;
                using (StreamReader reader = new StreamReader(stream))
                {
                    string content = reader.ReadToEnd();
                    Console.WriteLine(content.Contains("/Producer (Aspose.Cells for .NET)") 
                        ? "Producer property set successfully" 
                        : "Failed to set Producer property");
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


