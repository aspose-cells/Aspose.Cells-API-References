---
title: "DifSaveOptions.DifSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DifSaveOptions-konstruktor. Skapar alternativen för att spara DIF-fil"
type: docs
url: /sv/net/aspose.cells/difsaveoptions/difsaveoptions/
---
## DifSaveOptions constructor

Skapar alternativen för att spara DIF-fil.

```csharp
public DifSaveOptions()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DifSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Data");

            DifSaveOptions saveOptions = new DifSaveOptions()
            {
                ClearData = true,
                CreateDirectory = true,
                RefreshChartCache = true
            };

            workbook.Save("DifSaveOptionsOutput.dif", saveOptions);
        }
    }
}
```

### Se även

* class [DifSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


