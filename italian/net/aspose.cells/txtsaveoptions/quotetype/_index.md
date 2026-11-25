---
title: "TxtSaveOptions.QuoteType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TxtSaveOptions. Ottiene o imposta come racchiudere tra virgolette i valori nel file di testo esportato"
type: docs
url: /it/net/aspose.cells/txtsaveoptions/quotetype/
---
## TxtSaveOptions.QuoteType property

Ottiene o imposta come citare i valori nel file di testo esportato.

```csharp
public TxtValueQuoteType QuoteType { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyQuoteTypeDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di esempio con dati di test
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Text");
            worksheet.Cells["B1"].PutValue("123");
            worksheet.Cells["A2"].PutValue("Another text");
            worksheet.Cells["B2"].PutValue("=1+2");

            // Salva con QuoteType.Normal (predefinito)
            MemoryStream stream1 = new MemoryStream();
            workbook.Save(stream1, new TxtSaveOptions()
            {
                Encoding = Encoding.ASCII
            });
            
            // Salva con QuoteType.Always
            MemoryStream stream2 = new MemoryStream();
            workbook.Save(stream2, new TxtSaveOptions()
            {
                Encoding = Encoding.ASCII,
                QuoteType = TxtValueQuoteType.Always
            });

            // Visualizza l'output di esempio
            Console.WriteLine("Normal QuoteType:");
            Console.WriteLine(Encoding.ASCII.GetString(stream1.ToArray()));
            
            Console.WriteLine("\nAlways QuoteType:");
            Console.WriteLine(Encoding.ASCII.GetString(stream2.ToArray()));
        }
    }
}
```

### Vedi anche

* enum [TxtValueQuoteType](../../txtvaluequotetype/)
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


