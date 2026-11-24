---
title: "LowCodeLoadOptions.InputStream"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LowCodeLoadOptions-Eigenschaft. Liest und setzt den Stream der Vorlage"
type: docs
url: /de/net/aspose.cells.lowcode/lowcodeloadoptions/inputstream/
---
## LowCodeLoadOptions.InputStream property

Liest und setzt den Stream der Vorlage.

```csharp
public Stream InputStream { get; set; }
```

### Hinweise

Wenn für diese Eigenschaft ein nicht‑null Stream festgelegt wird, wird der zuvor gesetzte Wert für [`InputFile`](../inputfile/) ignoriert.

### Beispiele

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
            // Erstelle Beispieldaten im Memory‑Stream
            byte[] data = { 0x48, 0x65, 0x6C, 0x6C, 0x6F }; // "Hello" in bytes
            using (MemoryStream stream = new MemoryStream(data))
            {
                // Erstelle Ladeoptionen mit InputStream
                var loadOptions = new LowCodeLoadOptions() { InputStream = stream };

                // Erstelle eine neue Arbeitsmappe mit dem Stream
                using (Workbook workbook = new Workbook(stream))
                {
                    // Greife auf das erste Arbeitsblatt zu
                    Worksheet worksheet = workbook.Worksheets[0];
                    
                    // Demonstriere, dass der Inhalt geladen wurde
                    Console.WriteLine("First cell value: " + worksheet.Cells["A1"].Value);
                }
            }
        }
    }
}
```

### Siehe auch

* class [LowCodeLoadOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


