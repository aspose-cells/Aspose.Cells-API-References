---
title: "DifSaveOptions.DifSaveOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ DifSaveOptions. ينشئ الخيارات لحفظ ملف DIF"
type: docs
url: /ar/net/aspose.cells/difsaveoptions/difsaveoptions/
---
## DifSaveOptions constructor

ينشئ الخيارات لحفظ ملف DIF.

```csharp
public DifSaveOptions()
```

### أمثلة

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

### انظر أيضًا

* class [DifSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


