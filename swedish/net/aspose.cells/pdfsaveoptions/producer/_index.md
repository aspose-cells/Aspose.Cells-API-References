---
title: "PdfSaveOptions.Producer"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PdfSaveOptions‑egenskap. Hämtar och anger producenten av det genererade pdf‑dokumentet"
type: docs
url: /sv/net/aspose.cells/pdfsaveoptions/producer/
---
## PdfSaveOptions.Producer property

Hämtar och anger producenten av det genererade pdf‑dokumentet.

```csharp
public string Producer { get; set; }
```

### Anmärkningar

Om värdet är null, eller en giltig LICENSE inte är angiven, kommer strängen Aspose.Cells vVERSION att användas.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet och lägg till exempeldata
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("PDF Producer Property Demo");

            // Skapa PDF-sparalternativ
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Ange Producer‑egenskapen
            pdfSaveOptions.Producer = "Aspose.Cells for .NET";
            
            // Spara till minnesström
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, pdfSaveOptions);
                
                // Verifiera att Producer har angetts
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

### Se även

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


