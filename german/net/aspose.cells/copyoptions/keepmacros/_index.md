---
title: "CopyOptions.KeepMacros"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CopyOptions property. Gibt an, ob Makros beibehalten werden"
type: docs
url: /de/net/aspose.cells/copyoptions/keepmacros/
---
## CopyOptions.KeepMacros property

Gibt an, ob Makros beibehalten werden;

```csharp
public bool KeepMacros { get; set; }
```

### Hinweise

Nur beim Kopieren von Arbeitsmappen.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyKeepMacrosDemo
    {
        public static void Run()
        {
            // Erstelle Quellarbeitsmappe mit Makros (unter Verwendung einer Vorlagendatei, die Makros enthält)
            Workbook srcWorkbook = new Workbook("macros_template.xlsm");
            Worksheet srcSheet = srcWorkbook.Worksheets[0];
            srcSheet.Cells["A1"].PutValue("Macro-enabled source");

            // Erstelle Ziel‑Arbeitsbuch
            Workbook destWorkbook = new Workbook();
            
            // Setze Kopieroptionen mit KeepMacros auf true
            CopyOptions options = new CopyOptions();
            options.KeepMacros = true;

            // Kopiere Arbeitsblatt mit Makros
            destWorkbook.Worksheets[0].Copy(srcSheet, options);

            // Ergebnis speichern
            destWorkbook.Save("KeepMacrosExample.xlsm");
        }
    }
}
```

### Siehe auch

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


