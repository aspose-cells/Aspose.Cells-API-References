---
title: "OoxmlSaveOptions.EnableZip64"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OoxmlSaveOptions-Eigenschaft. Verwendet ZIP64-Erweiterungen beim Schreiben von ZIP-Archiven, falls erforderlich"
type: docs
url: /de/net/aspose.cells/ooxmlsaveoptions/enablezip64/
---
## OoxmlSaveOptions.EnableZip64 property

Verwenden Sie ZIP64-Erweiterungen beim Schreiben von ZIP-Archiven, falls erforderlich.

```csharp
public bool EnableZip64 { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OoxmlSaveOptionsPropertyEnableZip64Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("Sample data for Zip64 demonstration");
            
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.EnableZip64 = true;
            
            workbook.Save("output_with_zip64.xlsx", saveOptions);
        }
    }
}
```

### Siehe auch

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


