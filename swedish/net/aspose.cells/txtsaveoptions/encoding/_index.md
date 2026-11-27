---
title: "TxtSaveOptions.Encoding"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TxtSaveOptions egenskap. Hämtar och anger standardkodning"
type: docs
url: /sv/net/aspose.cells/txtsaveoptions/encoding/
---
## TxtSaveOptions.Encoding property

Hämtar och anger standardkodningen.

```csharp
public Encoding Encoding { get; set; }
```

### Exempel

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyEncodingDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");
            
            // Skapa TXT-sparalternativ med ASCII‑kodning
            TxtSaveOptions saveOptions = new TxtSaveOptions
            {
                Encoding = Encoding.ASCII,
                Separator = '\t'
            };
            
            // Spara arbetsboken med angiven kodning
            workbook.Save("output.txt", saveOptions);
            
            Console.WriteLine("File saved with ASCII encoding");
        }
    }
}
```

### Se även

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


