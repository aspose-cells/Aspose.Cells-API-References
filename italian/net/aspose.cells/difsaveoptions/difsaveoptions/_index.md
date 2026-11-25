---
title: "DifSaveOptions.DifSaveOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore DifSaveOptions. Crea le opzioni per il salvataggio di file DIF"
type: docs
url: /it/net/aspose.cells/difsaveoptions/difsaveoptions/
---
## DifSaveOptions constructor

Crea le opzioni per il salvataggio del file DIF.

```csharp
public DifSaveOptions()
```

### Esempi

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

### Vedi anche

* class [DifSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


