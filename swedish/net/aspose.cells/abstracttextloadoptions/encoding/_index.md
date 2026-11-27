---
title: "AbstractTextLoadOptions.Encoding"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AbstractTextLoadOptions‑egenskap. Hämtar och anger standardkodning. Gäller endast för csv‑fil"
type: docs
url: /sv/net/aspose.cells/abstracttextloadoptions/encoding/
---
## AbstractTextLoadOptions.Encoding property

Hämtar och anger standardkodningen. Gäller endast för csv-fil.

```csharp
public Encoding Encoding { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AbstractTextLoadOptionsPropertyEncodingDemo
    {
        public static void Run()
        {
            // Skapa exempel‑CSV‑data i ASCII‑kodning
            MemoryStream ms = new MemoryStream();
            byte[] data = Encoding.ASCII.GetBytes("Name,Age\nJohn,30\nJane,25");
            ms.Write(data, 0, data.Length);
            ms.Seek(0, SeekOrigin.Begin);

            // Läs in arbetsbok med specificerad ASCII‑kodning
            Workbook wb = new Workbook(ms, new TxtLoadOptions() { Encoding = Encoding.ASCII });
            Cells cells = wb.Worksheets[0].Cells;

            // Visa inläst data
            Console.WriteLine($"A1: {cells[0, 0].StringValue}");
            Console.WriteLine($"B1: {cells[0, 1].StringValue}");
            Console.WriteLine($"A2: {cells[1, 0].StringValue}");
            Console.WriteLine($"B2: {cells[1, 1].IntValue}");

            // Lägg till lite Unicode‑text
            cells[2, 0].PutValue("日本語のテキスト");
            
            // Spara med UTF-8‑kodning
            MemoryStream outputStream = new MemoryStream();
            wb.Save(outputStream, new TxtSaveOptions() { Encoding = Encoding.UTF8 });
            
            // Visa de första några byte för att visa UTF-8‑BOM
            byte[] outputBytes = outputStream.ToArray();
            Console.WriteLine($"First 3 bytes: {BitConverter.ToString(outputBytes, 0, 3)}");
        }
    }
}
```

### Se även

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


