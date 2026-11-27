---
title: "PasteOptions.IgnoreLinksToOriginalFile"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PasteOptions-egenskap. Ignorerar länkar till originalfilen"
type: docs
url: /sv/net/aspose.cells/pasteoptions/ignorelinkstooriginalfile/
---
## PasteOptions.IgnoreLinksToOriginalFile property

Ignorera länkar till originalfilen.

```csharp
public bool IgnoreLinksToOriginalFile { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertyIgnoreLinksToOriginalFileDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet src = workbook.Worksheets[0];
            
            // Skapa exempeldata med formler som kan länka till originalfilen
            src.Cells["A1"].PutValue("Header1");
            src.Cells["B1"].PutValue("Header2");
            src.Cells["A2"].PutValue(100);
            src.Cells["B2"].PutValue("=A2*2");  // Simple formula
            src.Cells["A3"].PutValue(200);
            src.Cells["B3"].PutValue("=A3*2");

            // Skapa destinationsarbetsblad och område
            Worksheet dst = workbook.Worksheets.Add("Destination");
            Aspose.Cells.Range srcRange = src.Cells.CreateRange("A1:B3");
            Aspose.Cells.Range dstRange = dst.Cells.CreateRange("A1:B3");

            // Konfigurera klistra-in-alternativ för att ignorera länkar till originalfilen
            PasteOptions pasteOptions = new PasteOptions();
            pasteOptions.PasteType = PasteType.All;
            pasteOptions.IgnoreLinksToOriginalFile = true;

            // Kopiera med de angivna klistra-in-alternativen
            dstRange.Copy(srcRange, pasteOptions);

            // Spara arbetsboken
            workbook.Save("PasteOptions_IgnoreLinksToOriginalFile_Output.xlsx");
        }
    }
}
```

### Se även

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


