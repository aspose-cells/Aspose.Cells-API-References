---
title: DifSaveOptions.DifSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: DifSaveOptions constructor. Creates the options for saving DIF file
type: docs
url: /net/aspose.cells/difsaveoptions/difsaveoptions/
---
## DifSaveOptions constructor

Creates the options for saving DIF file.

```csharp
public DifSaveOptions()
```

### Examples

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

### See Also

* class [DifSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


