---
title: "TxtSaveOptions.QuoteType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TxtSaveOptions‑egenskap. Hämtar eller anger hur värden ska citeras i den exporterade textfilen"
type: docs
url: /sv/net/aspose.cells/txtsaveoptions/quotetype/
---
## TxtSaveOptions.QuoteType property

Hämtar eller anger hur värden ska citeras i den exporterade textfilen.

```csharp
public TxtValueQuoteType QuoteType { get; set; }
```

### Exempel

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
            // Skapa en exempelarbetsbok med testdata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Text");
            worksheet.Cells["B1"].PutValue("123");
            worksheet.Cells["A2"].PutValue("Another text");
            worksheet.Cells["B2"].PutValue("=1+2");

            // Spara med QuoteType.Normal (standard)
            MemoryStream stream1 = new MemoryStream();
            workbook.Save(stream1, new TxtSaveOptions()
            {
                Encoding = Encoding.ASCII
            });
            
            // Spara med QuoteType.Always
            MemoryStream stream2 = new MemoryStream();
            workbook.Save(stream2, new TxtSaveOptions()
            {
                Encoding = Encoding.ASCII,
                QuoteType = TxtValueQuoteType.Always
            });

            // Visa exempelutdata
            Console.WriteLine("Normal QuoteType:");
            Console.WriteLine(Encoding.ASCII.GetString(stream1.ToArray()));
            
            Console.WriteLine("\nAlways QuoteType:");
            Console.WriteLine(Encoding.ASCII.GetString(stream2.ToArray()));
        }
    }
}
```

### Se även

* enum [TxtValueQuoteType](../../txtvaluequotetype/)
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


