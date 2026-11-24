---
title: "DifSaveOptions.DifSaveOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DifSaveOptions-Konstruktor. Erstellt die Optionen zum Speichern einer DIF-Datei"
type: docs
url: /de/net/aspose.cells/difsaveoptions/difsaveoptions/
---
## DifSaveOptions constructor

Erstellt die Optionen zum Speichern einer DIF-Datei.

```csharp
public DifSaveOptions()
```

### Beispiele

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

### Siehe auch

* class [DifSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


