---
title: "PdfSaveOptions.Producer"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PdfSaveOptions-Eigenschaft. Gibt den Ersteller des erzeugten PDF-Dokuments zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells/pdfsaveoptions/producer/
---
## PdfSaveOptions.Producer property

Liest und setzt den Ersteller des erzeugten PDF-Dokuments.

```csharp
public string Producer { get; set; }
```

### Hinweise

Wenn der Wert null ist oder keine gültige LICENSE gesetzt ist, wird die Zeichenkette Aspose.Cells vVERSION verwendet.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greifen Sie auf das erste Arbeitsblatt zu und fügen Sie Beispieldaten hinzu
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("PDF Producer Property Demo");

            // PDF-Speicheroptionen erstellen
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Legen Sie die Producer-Eigenschaft fest
            pdfSaveOptions.Producer = "Aspose.Cells for .NET";
            
            // In den Speicherstream speichern
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, pdfSaveOptions);
                
                // Überprüfen Sie, ob die Producer-Eigenschaft gesetzt wurde
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

### Siehe auch

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


