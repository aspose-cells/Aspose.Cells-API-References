---
title: "DifSaveOptions.DifSaveOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DifSaveOptions yapıcı. DIF dosyası kaydetmek için seçenekleri oluşturur"
type: docs
url: /tr/net/aspose.cells/difsaveoptions/difsaveoptions/
---
## DifSaveOptions constructor

DIF dosyası kaydetme seçeneklerini oluşturur.

```csharp
public DifSaveOptions()
```

### Örnekler

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

### Ayrıca Bakınız

* class [DifSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


