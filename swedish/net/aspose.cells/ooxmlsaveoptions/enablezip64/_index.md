---
title: "OoxmlSaveOptions.EnableZip64"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OoxmlSaveOptions-egenskap. Använd ZIP64-utökningar när zip-arkiv skrivs vid behov"
type: docs
url: /sv/net/aspose.cells/ooxmlsaveoptions/enablezip64/
---
## OoxmlSaveOptions.EnableZip64 property

Använd ZIP64‑tillägg när du skriver zip‑arkiv, vid behov.

```csharp
public bool EnableZip64 { get; set; }
```

### Exempel

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

### Se även

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


