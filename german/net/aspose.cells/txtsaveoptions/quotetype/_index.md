---
title: "TxtSaveOptions.QuoteType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TxtSaveOptions-Eigenschaft. Gibt an, wie Werte in der exportierten Textdatei zitiert werden, oder legt dies fest"
type: docs
url: /de/net/aspose.cells/txtsaveoptions/quotetype/
---
## TxtSaveOptions.QuoteType property

Liest oder setzt, wie Werte in der exportierten Textdatei in Anführungszeichen gesetzt werden.

```csharp
public TxtValueQuoteType QuoteType { get; set; }
```

### Beispiele

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
            // Erstelle eine Beispielarbeitsmappe mit Testdaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Text");
            worksheet.Cells["B1"].PutValue("123");
            worksheet.Cells["A2"].PutValue("Another text");
            worksheet.Cells["B2"].PutValue("=1+2");

            // Speichern mit QuoteType.Normal (Standard)
            MemoryStream stream1 = new MemoryStream();
            workbook.Save(stream1, new TxtSaveOptions()
            {
                Encoding = Encoding.ASCII
            });
            
            // Speichern mit QuoteType.Always
            MemoryStream stream2 = new MemoryStream();
            workbook.Save(stream2, new TxtSaveOptions()
            {
                Encoding = Encoding.ASCII,
                QuoteType = TxtValueQuoteType.Always
            });

            // Beispielausgabe anzeigen
            Console.WriteLine("Normal QuoteType:");
            Console.WriteLine(Encoding.ASCII.GetString(stream1.ToArray()));
            
            Console.WriteLine("\nAlways QuoteType:");
            Console.WriteLine(Encoding.ASCII.GetString(stream2.ToArray()));
        }
    }
}
```

### Siehe auch

* enum [TxtValueQuoteType](../../txtvaluequotetype/)
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


