---
title: "Klass LowCodeLoadOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.LowCode.LowCodeLoadOptions-klass. Alternativ för att läsa in mallfil"
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodeloadoptions/
---
## LowCodeLoadOptions class

Alternativ för att ladda mallfil.

```csharp
public class LowCodeLoadOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [LowCodeLoadOptions](lowcodeloadoptions/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [InputFile](../../aspose.cells.lowcode/lowcodeloadoptions/inputfile/) { get; set; } | Hämtar och anger filen (med sökväg om behövs) för mallen. |
| [InputStream](../../aspose.cells.lowcode/lowcodeloadoptions/inputstream/) { get; set; } | Hämtar och anger strömmen för mallen. |

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassLowCodeLoadOptionsDemo
    {
        public static void Run()
        {
            // Skapa ett exempelström (i minnet för demonstrationsändamål)
            using (MemoryStream stream = new MemoryStream())
            {
                // Skapa en ny arbetsbok och spara till strömmen för demonstration
                Workbook workbook = new Workbook();
                workbook.Worksheets.Add("Sheet1");
                workbook.Save(stream, SaveFormat.Xlsx);

                // Återställ strömmens position
                stream.Position = 0;

                // Skapa och använd LowCodeLoadOptions
                var loadOptions = new LowCodeLoadOptions()
                {
                    InputStream = stream
                };

                // Exempel på användning – skulle vanligtvis skickas till en bearbetningsmetod
                Console.WriteLine($"Loading with LowCode options from stream of length: {loadOptions.InputStream.Length}");
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


