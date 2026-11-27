---
title: "CopyOptions.KeepMacros"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CopyOptions property. Anger om makron ska behållas"
type: docs
url: /sv/net/aspose.cells/copyoptions/keepmacros/
---
## CopyOptions.KeepMacros property

Anger om makron ska behållas;

```csharp
public bool KeepMacros { get; set; }
```

### Anmärkningar

Endast för att kopiera arbetsbok.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyKeepMacrosDemo
    {
        public static void Run()
        {
            // Skapa källarbok med makron (använd en mallfil som innehåller makron)
            Workbook srcWorkbook = new Workbook("macros_template.xlsm");
            Worksheet srcSheet = srcWorkbook.Worksheets[0];
            srcSheet.Cells["A1"].PutValue("Macro-enabled source");

            // Skapa målarbetsbok
            Workbook destWorkbook = new Workbook();
            
            // Ställ in kopieringsalternativ med KeepMacros true
            CopyOptions options = new CopyOptions();
            options.KeepMacros = true;

            // Kopiera kalkylblad med makron
            destWorkbook.Worksheets[0].Copy(srcSheet, options);

            // Spara resultatet
            destWorkbook.Save("KeepMacrosExample.xlsm");
        }
    }
}
```

### Se även

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


