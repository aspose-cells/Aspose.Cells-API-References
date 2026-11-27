---
title: "LowCodeLoadOptions.InputStream"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LowCodeLoadOptions‑egenskap. Hämtar och anger strömmen för mallen"
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodeloadoptions/inputstream/
---
## LowCodeLoadOptions.InputStream property

Hämtar och anger strömmen för mallen.

```csharp
public Stream InputStream { get; set; }
```

### Anmärkningar

När du anger en icke‑null ström för denna egenskap, kommer det tidigare angivna värdet för [`InputFile`](../inputfile/) att ignoreras.

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeLoadOptionsPropertyInputStreamDemo
    {
        public static void Run()
        {
            // Skapa exempeldata i minnesström
            byte[] data = { 0x48, 0x65, 0x6C, 0x6C, 0x6F }; // "Hello" in bytes
            using (MemoryStream stream = new MemoryStream(data))
            {
                // Skapa laddningsalternativ med InputStream
                var loadOptions = new LowCodeLoadOptions() { InputStream = stream };

                // Skapa en ny arbetsbok med strömmen
                using (Workbook workbook = new Workbook(stream))
                {
                    // Åtkomst till det första kalkylbladet
                    Worksheet worksheet = workbook.Worksheets[0];
                    
                    // Visa att innehållet har lästs in
                    Console.WriteLine("First cell value: " + worksheet.Cells["A1"].Value);
                }
            }
        }
    }
}
```

### Se även

* class [LowCodeLoadOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


